---
title: The Jigsaw–Pack Architecture
---

# The Jigsaw–Pack Architecture

Every topic in this vault has exactly two notes. They hold the same material, organised for two different jobs.

> [!tip] 🧩 Jigsaw — *what could be asked*
> The syllabus, rebuilt bullet by bullet, with every tested angle mapped onto it. Read it to find out **where the marks live** and **what has never been asked**.

> [!tip] 🎯 Pack — *answering it under timed conditions*
> The same concepts turned into exam questions with full mark-scheme answers, collapsed so you can self-test. Use it to **rehearse**.

---

## Why two notes and not one

A revision note that mixes "here is the content" with "here is a question on it" does neither job well. You cannot skim it for coverage, and you cannot test yourself on it without seeing the answers.

Splitting them means the **Jigsaw is a map** and the **Pack is a drill**. They mirror each other section by section, so any concept can be followed from one to the other.

---

## The Jigsaw

The Jigsaw walks the syllabus in order — 8.1.1, 8.1.2, 8.1.3 and so on — and under each bullet places every distinct concept that has been, or could be, examined. Each concept gets **one callout**, and the callout's **type tells you its exam status**.

> [!success] Already examined in 9618
> Tested in a 9618 paper, 2021 onwards. The mark-scheme points are given, followed by the **question ID of the most recent appearance**, in the format the Legend PDFs use: `9618_w25_qp_13_sc_5.b`.

> [!warning] 9608 only — not yet in 9618
> Tested under the **old 9608 syllabus** (pre-2021), but the wording is still inside the current 9618 syllabus. Fair game — and often a genuine content gap rather than just a format one. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In the syllabus, but never asked in **either** series — or only ever asked in a much narrower form. Every one carries a **justification** for why it is a plausible question, and a suggested tariff.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question covers. Useful for understanding; weigh it against the mark schemes before trusting it in an answer.

> [!danger] No old-syllabus safety net
> Flags a sub-topic that is **new in 9618** with no 9608 questions at all, so there is nothing to fall back on. Currently: AI (7), embedded systems (3), PROM/EPROM/EEPROM (3), bit manipulation (all of 4.3) and IDE features (5.2.4).

> [!note] Reading notes
> Occasional notes about the **shape** of a question rather than its content — fixed tariffs, block marking, command-word traps.

### How to read the question IDs

`9618_w25_qp_13_sc_5.b` →  syllabus `9618` · session `w25` (Winter 2025) · `qp_13` (paper 13) · `sc_5.b` (question 5b).
`s` = summer (May/June), `w` = winter (Oct/Nov).

---

## The Pack

The Pack mirrors the Jigsaw. Every concept becomes a `!question` callout containing a **collapsible** answer, so the question can be attempted before the answer is revealed.

```markdown
> [!question] 9618 | Describe the purpose of an OS in a computer [5]
> Describe the purpose of an Operating System in a computer system.
>
>> [!success]- Answer — 7 points for 5 marks
>> - To provide a **user interface** … so the user can communicate with the hardware
>> - To **manage memory** … so data can be stored and multitasking is possible
>> - …
>>
>> *Latest: `9618_s25_qp_11_sc_6.b`*
```

### The title line

`prefix | rewritten question [marks]`

- **9618 |** — the **highest tariff this concept has ever carried** in a 9618 paper. If November 2025 asked it for 2 marks and June 2022 for 4, the Pack uses **4**.
- **9608 |** — the same rule applied to 9608 tariffs.
- **Inferred |** — never tested; the tariff is estimated from how 9618 marks comparable questions.
- **SME |** — drawn from the Save My Exams notes, tariff estimated the same way.

The wording is **rewritten generic exam-style**, not the original past-paper scenario — so you are testing the concept rather than remembering one particular context.

### The answer

Answers aim for the **maximum tariff plus two spare points**, because mark schemes routinely list more credit-worthy points than the tariff allows. The newest mark scheme leads; older ones fill the gaps.

- **One bullet = one mark.**
- A bullet beginning `…` is an **expansion** of the point above it, not a separate mark — this is how Cambridge marks "point plus expansion" questions.
- Capping rules are stated wherever they exist: *max 2 for each*, *mark in pairs*, *no mark for the choice*.
- The question ID at the foot is the paper the answer was built from.

---

## How to actually use them

1. **Map first.** Read a Jigsaw section and note which callouts are `!success` — those are the questions that keep coming back.
2. **Drill.** Open the matching Pack section, cover the answer, write a full answer to the tariff, then expand the callout and mark yourself against the bullets.
3. **Mind the `!info` entries.** They are the untested corners of the syllabus. In a subject where examiners cycle through bullets, these are where next year's unfamiliar question is most likely to come from.
4. **Treat `!warning` entries as real.** 9608 questions are the same syllabus content in an older format. Chapter 6 has 31 of them; chapter 4 has none at all.

> [!danger] What memorising a Pack will *not* do
> Learning every Pack answer by heart does **not** guarantee full marks. Mark schemes award **contextual application** — points tied to the scenario in front of you — and the same concept is set at different tariffs with different command words. The Pack teaches you the content and the shape of the answer; timed past papers teach you to apply it. Use both.

---

## Conventions used throughout

| Convention | Meaning |
|---|---|
| **Bold** inside an answer | The exact word or phrase the mark scheme requires |
| `//` | "or" — an equally acceptable alternative wording |
| `…` starting a bullet | An expansion of the bullet above, not a separate mark |
| `[n]` in a title | The mark tariff being answered to |
| *Latest: `id`* | The most recent paper this concept appeared in |

---

## Source material

Everything traces back to the [[03_Resources/index|Legend archive]] — the full 9618 and 9608 question banks sorted by syllabus bullet — plus the 2026 syllabus PDF and the Save My Exams notes. Where a claim is an inference rather than a mark-scheme point, the note says so explicitly.
