---
title: Setting up kyber-of-computer (Quartz + GitHub Pages + Porkbun)
---

# Setting up `kyber-of-computer`

A step-by-step guide to stand up a third Quartz site for Computer Science at
**computer.pushthecar.com**, matching the existing `kyber-of-physics` setup exactly.

**Target end state**

| Thing | Value |
| --- | --- |
| Quartz repo folder | `C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer` |
| Content source (vault) | `C:\Users\HP\OneDrive\Documents\A-Level\Obsidian\Computer` |
| Link between them | `content` directory symlink |
| GitHub repo | `Pushkar-Gooljar/kyber-of-computer` (public) |
| Deploy branch | `v4` |
| Live URL | `https://computer.pushthecar.com` |

---

## Why copy the physics folder instead of cloning Quartz fresh

Your physics and chemistry sites are on **Quartz v4** (branch `v4`, Node 22), and they
contain a custom transformer that stock Quartz does not ship:
`quartz/plugins/transformers/caption.ts` (the `ImageCaption` plugin imported at the top of
`quartz.config.ts`).

Upstream Quartz has since moved to **v5**, which has a different layout, a
`quartz.lock.json`, a `npx quartz plugin install` step and Node 24. Cloning upstream today
would give you a site that does not match the other two and would break the
`ImageCaption` import.

So: **copy your existing physics folder** as the starting point. That guarantees identical
theme, layout, plugins and build behaviour. Only the config values, the content symlink and
the git remote change.

---

## Step 1 — Create the folder by copying physics

Open **PowerShell** (normal, non-admin is fine) and run:

```powershell
cd "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals"

robocopy "kyber-of-physics" "kyber-of-computer" /E `
  /XD ".git" "content" "node_modules" "public" ".quartz-cache" "docs" `
  /XF ".gitignore"

# robocopy exits with code 1 on success — that is normal, not an error.
```

Then copy `.gitignore` back in explicitly (robocopy's `/XF` skipped it because the physics
`.gitignore` ignores itself, which we do want to keep):

```powershell
Copy-Item "kyber-of-physics\.gitignore" "kyber-of-computer\.gitignore"
```

> **Note on `.gitignore`:** your physics repo's `.gitignore` contains the line `.gitignore`
> — it ignores itself. That is inherited from upstream Quartz and is harmless; keep it so
> the three repos stay consistent.

`docs/` is excluded because it is upstream Quartz's own documentation and it would get
picked up as content noise — physics keeps it only because it came with the original clone.
If you want the repos byte-identical, drop `"docs"` from the `/XD` list.

Verify:

```powershell
dir "kyber-of-computer"
```

You should see `quartz\`, `quartz.config.ts`, `quartz.layout.ts`, `package.json`,
`package-lock.json`, `.github\`, `.node-version`, `.npmrc`, `.prettierrc`, `tsconfig.json`,
`globals.d.ts`, `index.d.ts`, `Dockerfile`.

---

## Step 2 — Create the `content` symlink to the Computer vault

This is the step that makes the Obsidian vault *be* the site content, exactly as physics does.

`mklink /D` needs either an **Administrator** Command Prompt, or Windows **Developer Mode**
turned on (Settings → System → For developers → Developer Mode).

Open **Command Prompt as Administrator** (`cmd.exe`, right-click → Run as administrator):

```cmd
cd /d "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer"

mklink /D content "C:\Users\HP\OneDrive\Documents\A-Level\Obsidian\Computer"
```

Expected output: `symbolic link created for content <<===>> C:\Users\HP\...\Obsidian\Computer`

**If you cannot get an admin prompt**, use a directory junction instead — it needs no
elevation and Git treats it the same way:

```cmd
mklink /J content "C:\Users\HP\OneDrive\Documents\A-Level\Obsidian\Computer"
```

Verify it resolves:

```cmd
dir content
```

You should see `00_Templates`, `01_Concepts`, `03_Resources`, `04_Excalidraw`, `.obsidian`.

> **Why this works with Git:** your repos have `core.symlinks = false` (Git for Windows sets
> this when symlink support is off). With that setting Git cannot represent a symlink, so it
> walks *into* the linked directory and commits the real files. That is how your physics
> content ends up in the GitHub repo and is available to the build runner. Step 5 verifies this.

---

## Step 3 — Give the vault a root `index.md`

Quartz needs `content/index.md` as the site's landing page. Your **Physics vault has one;
the Computer vault does not** — so the build would produce a site with no home page.

Create `C:\Users\HP\OneDrive\Documents\A-Level\Obsidian\Computer\index.md`. Here is the
physics one for reference:

```markdown
---
title: PushTheCar Physics
---
# Notes
## [[02_Notes/14. Temperature/index|14. Temperature]]
## [[02_Notes/15. Ideal Gases/index|15. Ideal Gases]]

---
# Worksheets
Topical worksheets with past paper questions + Mark schemes having examiners reports
## [[Topical Worksheets|A Level Worksheets]]

---
# Definition Banks
Mark scheme question/answers for physics definitions.
## [[9702-P2_definition_bank|AS Level]]
## [[9702-P4_definition_bank|A Level]]
```

A starting point for Computer:

```markdown
---
title: PushTheCar Computer Science
---
# Notes
## [[01_Concepts/Paper_1_Theory/index|Paper 1 — Theory]]
## [[01_Concepts/Paper_2_Problem_solving/index|Paper 2 — Problem Solving]]

---
# Resources
## [[03_Resources/index|Resources]]
```

Adjust the wikilinks to whatever index notes actually exist in those folders.

---

## Step 4 — Edit `quartz.config.ts`

Open `kyber-of-computer\quartz.config.ts` and change exactly these lines in the
`configuration` block:

```ts
    pageTitle: "Computer Science",        // was: "Physics"
    baseUrl: "computer.pushthecar.com",   // was: "physics.pushthecar.com"
    ignorePatterns: ["private", "templates", ".obsidian", "00_Templates"],
```

Three notes:

1. **`ignorePatterns` capitalisation.** Physics uses `00_templates` (lowercase t) because its
   vault folder is `00_templates`. Your **Computer vault uses `00_Templates`** (capital T), so
   the pattern must match it or your template notes will be published.
2. **`baseUrl` has no `https://` and no trailing slash.** This is what Quartz uses for RSS,
   the sitemap and OG images. Getting it wrong silently breaks those.
3. **Analytics.** The file currently carries the *physics* GA4 tag:
   ```ts
   analytics: { provider: "google", tagId: "G-0HNPY2WW4Q" },
   ```
   Leaving it would fold Computer's traffic into the Physics property. Either create a new
   GA4 property for `computer.pushthecar.com` and paste its `G-XXXXXXXXXX` measurement ID,
   or disable analytics entirely:
   ```ts
   analytics: null,
   ```

Leave `quartz.layout.ts` untouched — that is what keeps the explorer, graph, backlinks,
reader mode and footer identical to physics.

---

## Step 5 — Modernise the deploy workflow

Open `kyber-of-computer\.github\workflows\deploy.yml`. It is inherited from physics and
pins `runs-on: ubuntu-22.04`.

**The Ubuntu 22.04 runner image begins deprecation on 17 September 2026 and is fully
unsupported from 17 April 2027.** Change that one line now so the new site does not break
in a few months:

```yaml
jobs:
  build:
    runs-on: ubuntu-latest      # was: ubuntu-22.04
```

The rest of the file stays as-is. For reference, the complete file should read:

```yaml
name: Deploy Quartz site to GitHub Pages

on:
  push:
    branches:
      - v4

permissions:
  contents: read
  pages: write
  id-token: write

concurrency:
  group: "pages"
  cancel-in-progress: false

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
        with:
          fetch-depth: 0

      - uses: actions/setup-node@v4
        with:
          node-version: 22

      - name: Install Dependencies
        run: npm ci

      - name: Build Quartz
        run: npx quartz build

      - name: Upload artifact
        uses: actions/upload-pages-artifact@v3
        with:
          path: public

  deploy:
    needs: build
    environment:
      name: github-pages
      url: ${{ steps.deployment.outputs.page_url }}
    runs-on: ubuntu-latest
    steps:
      - name: Deploy to GitHub Pages
        id: deployment
        uses: actions/deploy-pages@v4
```

> Also worth doing the same one-line edit in `kyber-of-physics` and `kyber-of-chemistry`
> while you are at it — they are on the same deprecated image.

Also delete the workflows you do not use, so GitHub doesn't run them or email you about
failures. Physics inherited five workflow files from upstream Quartz:

```powershell
cd "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer\.github\workflows"
Remove-Item "build-preview.yaml","ci.yaml","deploy-preview.yaml","docker-build-push.yaml"
```

(Optional — physics still has them. Skip if you want an exact mirror.)

---

## Step 6 — Build locally before touching GitHub

Never push an untested Quartz build; a bad wikilink or a missing `index.md` is much easier
to diagnose locally.

```powershell
cd "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer"

npm ci
npx quartz build --serve
```

`npm ci` installs from the copied `package-lock.json`, so you get exactly the dependency
versions physics builds with. Open <http://localhost:8080> and check:

- the home page renders (that's your new `index.md`),
- the left explorer shows `01_Concepts`, `03_Resources` and **not** `00_Templates`,
- the title in the sidebar says "Computer Science",
- notes and images load.

Press `Ctrl+C` to stop. If the build errors, fix it here — the GitHub Action runs the
identical command.

---

## Step 7 — Create the GitHub repository

On <https://github.com/new>:

- **Owner:** `Pushkar-Gooljar`
- **Repository name:** `kyber-of-computer`
- **Visibility:** **Public** (GitHub Pages on a free account requires public; private Pages
  needs GitHub Pro)
- **Do not** add a README, `.gitignore` or licence — leave the repo completely empty.

Click **Create repository** and leave the page open.

---

## Step 8 — Initialise Git and push to the `v4` branch

Back in PowerShell, in `kyber-of-computer`:

```powershell
cd "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer"

git init
git config core.symlinks false
git checkout -b v4

git remote add origin   https://github.com/Pushkar-Gooljar/kyber-of-computer.git
git remote add upstream https://github.com/jackyzha0/quartz.git
```

`git config core.symlinks false` is the line that makes Git commit the *contents* of the
`content` link rather than the link itself — matching physics and chemistry.

**Verify the content is actually staged before committing:**

```powershell
git add -A
git status --short | Select-String "content/" | Select-Object -First 10
```

You must see real files listed, e.g. `A  content/01_Concepts/...`. If you instead see a
single entry `A  content` (and nothing under it), the symlink was not followed — redo
Step 2 using `mklink /J`, then `git rm -r --cached content` and `git add -A` again.

Then commit and push:

```powershell
git commit -m "Initial commit: Quartz site for A-Level Computer Science"
git push -u origin v4
```

Set `v4` as the repo's default branch so the GitHub UI and future clones behave like your
other two: **repo → Settings → General → Default branch → switch to `v4`**.

---

## Step 9 — Turn on GitHub Pages

In the repo: **Settings → Pages**.

- **Build and deployment → Source:** select **GitHub Actions**.

That's the whole setting — do not pick "Deploy from a branch". Your `deploy.yml` is a custom
Actions workflow and it publishes the artifact itself.

Now check **Actions** tab. The push from Step 8 should already have triggered
*Deploy Quartz site to GitHub Pages*. Wait for both the `build` and `deploy` jobs to go green
(typically 2–4 minutes). The `deploy` job prints the live URL, which at this point is
`https://pushkar-gooljar.github.io/kyber-of-computer/`.

> If the deploy job fails with a protection-rule / environment error, go to
> **Settings → Environments → github-pages** and remove any branch protection rule that
> doesn't include `v4`.

---

## Step 10 — Add the DNS record at Porkbun

You only need **one new record** — a CNAME for the `computer` host. Do **not** use Porkbun's
"Quick DNS Config → GitHub" button: that rewrites your whole zone and would disturb the
records already serving `pushthecar.com`, `physics.` and `chemistry.`.

1. Log in at <https://porkbun.com> → **ACCOUNT → Domain Management**.
2. Find `pushthecar.com`, click **Details**, then the **DNS** / edit icon to open
   **Manage DNS Records**.
3. First, look at how your existing `physics` record is set up and copy its shape — that is
   your ground truth. It should be a `CNAME` with host `physics` answering
   `pushkar-gooljar.github.io`.
4. Add a new record:

   | Field | Value |
   | --- | --- |
   | **Type** | `CNAME` |
   | **Host** | `computer` |
   | **Answer** | `pushkar-gooljar.github.io` |
   | **TTL** | `600` |

   Notes: the Host field is just the label — enter `computer`, **not**
   `computer.pushthecar.com`. The Answer has **no** repository name, **no** `https://`, and
   **no** trailing dot.

5. Click **Add**.

> **Do not** point `computer` at `pushthecar.com` or at another subdomain. GitHub explicitly
> warns that chaining a subdomain to an apex domain breaks HTTPS enforcement.

Verify propagation from PowerShell (usually within minutes, but allow up to 24 h):

```powershell
nslookup -type=CNAME computer.pushthecar.com 8.8.8.8
```

You want to see it resolve to `pushkar-gooljar.github.io`.

---

## Step 11 — Attach the custom domain in GitHub

Back in the repo: **Settings → Pages → Custom domain**.

1. Enter `computer.pushthecar.com` and click **Save**.
2. GitHub runs a DNS check. A green tick means the CNAME resolved. A red "DNS check in
   progress / unsuccessful" usually just means propagation hasn't finished — wait and hit
   **Check again**.
3. Once the check passes, GitHub provisions a Let's Encrypt certificate (a few minutes up to
   an hour). When the **Enforce HTTPS** checkbox becomes selectable, **tick it**.

> Because you publish via a custom GitHub Actions workflow, GitHub does **not** create a
> `CNAME` file in your repo, and any existing one is ignored. The domain lives purely in this
> setting. This is why `kyber-of-physics` has no `CNAME` file either — nothing is missing.

Visit <https://computer.pushthecar.com>. Done.

---

## Step 12 — Verification checklist

Work through these before calling it finished:

- [ ] `https://computer.pushthecar.com` loads over HTTPS with a valid certificate.
- [ ] `http://computer.pushthecar.com` redirects to HTTPS (Enforce HTTPS ticked).
- [ ] Home page is your `index.md`, not a 404 or a folder listing.
- [ ] Left sidebar title reads "Computer Science"; explorer shows `01_Concepts` /
      `03_Resources` and hides `00_Templates` and `.obsidian`.
- [ ] Search, dark mode toggle, graph view, backlinks and table of contents all work
      (confirms `quartz.layout.ts` copied cleanly).
- [ ] `https://computer.pushthecar.com/index.xml` returns the RSS feed and
      `https://computer.pushthecar.com/sitemap.xml` returns the sitemap, both with
      `computer.pushthecar.com` URLs inside (confirms `baseUrl`).
- [ ] Physics and chemistry sites still load — you didn't disturb the Porkbun zone.
- [ ] Actions tab shows a green run on the latest push.

---

## Day-to-day: publishing new notes

Write in Obsidian in the `Computer` vault as usual, then:

```powershell
cd "C:\Users\HP\OneDrive\Documents\A-Level\KyberCrystals\kyber-of-computer"
npx quartz sync
```

`npx quartz sync` stages, commits and pushes `content` in one go, which triggers the Action
and redeploys. Same command you use for physics.

Useful flags: `-v` (verbose), `--no-pull` (skip pulling first), `--no-push` (commit only),
`-m "message"` (custom commit message).

To preview before publishing: `npx quartz build --serve`.

---

## Pulling upstream Quartz updates (optional, later)

You added `upstream` in Step 8 for parity with the other repos, but be careful: upstream's
default branch is now **v5**, which is a breaking change from your v4 setup. Don't casually
`git pull upstream`. If you ever want v4 bugfixes only:

```powershell
git fetch upstream
git merge upstream/v4
```

and expect to re-apply the `ImageCaption` import and your config changes if they conflict.
Upgrading all three sites to Quartz v5 is a separate project — worth doing eventually, but
do it deliberately and to all three at once so they stay consistent.

---

## Quick reference — what differs from physics

| File | Physics | Computer |
| --- | --- | --- |
| `quartz.config.ts` → `pageTitle` | `Physics` | `Computer Science` |
| `quartz.config.ts` → `baseUrl` | `physics.pushthecar.com` | `computer.pushthecar.com` |
| `quartz.config.ts` → `ignorePatterns` | `...,"00_templates"` | `...,"00_Templates"` |
| `quartz.config.ts` → `analytics.tagId` | `G-0HNPY2WW4Q` | new GA4 ID, or `analytics: null` |
| `.github/workflows/deploy.yml` → `runs-on` | `ubuntu-22.04` | `ubuntu-latest` |
| `content` symlink target | `...\Obsidian\Physics` | `...\Obsidian\Computer` |
| `git remote origin` | `.../kyber-of-physics.git` | `.../kyber-of-computer.git` |
| Porkbun CNAME host | `physics` | `computer` |

Everything else — `quartz.layout.ts`, the theme colours, typography, the plugin list, the
`ImageCaption` transformer, `.node-version`, `package.json` — stays byte-identical.
