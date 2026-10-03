---
title: Jigsaw — 6 Security, privacy and data integrity (AS Level)
syllabus: 9618 (2026)
topics: 6.1 Data Security · 6.2 Data Integrity
---

# Jigsaw — 6 Security, privacy and data integrity

Syllabus content for **9618 Topic 6**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording. Fair game — just untested in the current series. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers. Weigh it against the mark schemes — SME sometimes goes beyond what Cambridge credits.

---

# 6.1 Data Security

## 6.1.1 Explain the difference between the terms security, privacy and integrity of data

> [!success] Describe the difference between security and privacy of data
> Security protects data against **loss** (accidental or malicious damage); privacy protects data against **unauthorised access** / keeps it confidential. `9618_w23_qp_12_sc_5.a`

> [!success] Describe the difference between security and integrity of data
> Security = keeping data safe from loss/unauthorised access; integrity = data is **accurate, consistent and up to date**, and what was received is the same as what was sent. `9618_w23_qp_12_sc_5.b`

> [!success] Identify the correct term from a description
> "Ensures data is accurate and up to date" → integrity · "prevents accidental or malicious data loss" → security · "prevents unauthorised access" → privacy. `9618_w21_qp_12_sc_1`

> [!success] Apply the terms to a scenario (why privacy matters here)
> `9618_s23_qp_11_sc_2.a.ii`

> [!warning] Give an example of an application where privacy of data is a key concern
> e.g. personal data of students / staff. 9618 defines the terms but has never asked for a **context example** of privacy. `9608_w17_qp_12_sc_3.a.ii`

> [!warning] Describe *two* differences between integrity and security in one answer
> Integrity deals with validity / freedom from errors; security deals with protection from illegal access or loss; integrity is about data not being corrupted, e.g. after transmission. `9608_s15_qp_13_sc_3.b`

> [!warning] Give an example of how a database manager can ensure data integrity
> Validation rules, referential integrity, verification, input masks, setting data types, removing redundant data, backup, access controls, **audit trail**. `9608_s18_qp_13_sc_2.b`

> [!info] A three-way question in one part
> 9618 has asked security-vs-privacy and security-vs-integrity as separate 2-markers, and the tick-table has all three. A single "explain the difference between all three terms, with an example of each" (the 9608 4-mark shape) has not appeared in the current series.

> [!abstract] The three terms as a one-line contrast
> **Security** = keeping data safe from threats (hackers) · **Privacy** = making sure data is collected and used fairly and with consent · **Integrity** = making sure data stays accurate and unchanged. Note SME's privacy framing adds **consent** — asking the user before collecting or sharing personal data — which no mark scheme in this topic uses but is a defensible expansion of "restrict access to personal data".

---

## 6.1.2 Show appreciation of the need for both the security of data and the security of the computer system

> [!warning] Explain how data backup and disk-mirroring allow recovery from data loss
> **Backup:** a copy of the data is made and stored elsewhere; if the original is lost it can be restored. **Disk-mirroring:** data is stored on two disks simultaneously; if the first drive fails the data is read from the second. **This whole bullet has no 9618 question at all.** `9608_s19_qp_11_sc_4.b`

> [!warning] Describe methods of preventing *accidental* loss of data
> Frequent backup (to secondary media, a third-party server, the cloud, removable devices, or stored remotely); disk-mirroring / RAID; **UPS (uninterruptable power supply) or backup generator**. `9608_s15_qp_11_sc_6.b.i`

> [!warning] Explain why a stated security claim is wrong ("encryption prevents hackers breaking in")
> Hackers can still access the data (and corrupt, change or delete it); encryption only makes the data **incomprehensible** without the decryption key. This "explain why this answer is incorrect" format is pure 9608 and tests exactly this bullet — the distinction between protecting the **system** and protecting the **data**. `9608_w16_qp_13_sc_7.c.i`

> [!warning] Explain why "passwords will always prevent unauthorised access" is wrong
> A password does not prevent access, it makes it harder; passwords can be guessed if weak, or stolen. `9608_w16_qp_11_sc_7.c.iii`

> [!info] The distinction itself
> The Legend has **zero** 9618 questions under this bullet. The concept — that securing the *machine* (physical locks, firewall, OS accounts) and securing the *data* (encryption, access rights, backup) are different jobs — sits behind several 9618 questions but has never been asked directly. A "state why a company needs both" or the 9608-style misconception question is entirely available.

> [!abstract] Why passwords are stored encrypted
> Passwords are held as **encrypted / ciphered text in a database**, so even a hacker who gains access to the database cannot read individual users' passwords. The neatest illustration of "the system may fall, but the data is still protected".

---

## 6.1.3 Describe security measures designed to protect computer systems, from stand-alone PC to network

> [!success] Identify a security measure protecting a server from hackers, and describe how it works
> **Firewall:** checks incoming connections against criteria, blocks data entering specific ports, blocks data that does not meet a whitelist / meets a blacklist. **Proxy server:** prevents devices accessing the web server directly, intercepts requests, forwards them using its own IP address, screens returning data. `9618_s24_qp_12_sc_3.a.i`

> [!success] Identify and describe two types of software installed to prevent threats over a network
> **Antivirus / antimalware:** scans the computer against a stored database of known signatures that must be updated regularly, deletes or quarantines; compares downloaded files to the database and stops the download. **Antispyware:** the same for spyware. **Firewall:** monitors **incoming and outgoing** traffic against user-set criteria (whitelist/blacklist, allowed/blocked IP addresses). `9618_s23_qp_13_sc_6.b`

> [!success] Identify one software-based measure to restrict access to data
> Two-factor authentication, biometric passwords, key card access, firewall. `9618_s21_qp_12_sc_8.b`

> [!success] Describe how access rights protect data from unauthorised access
> Different accounts / logins with different rights (read-only // no access // read-write); specific **views** can be assigned so a user sees only their own data. `9618_w21_qp_11_sc_5.b`

> [!success] Identify methods a DBMS can use to protect data, and explain each
> Access rights (permissions to read or edit a table), a password for the database or the table, encrypting the database, **views** that exclude the protected table. `9618_s25_qp_12_sc_5.c.i`

> [!success] Digital signatures / authentication as a protective measure
> `9618_w25_qp_12_sc_10.c`, `9618_w22_qp_12_sc_6.a.i`

> [!warning] Describe what is meant by a digital signature
> A mathematical algorithm // encrypted data, **attached to an electronically transmitted document**, to verify its content and that it comes from a trusted source. 9618 uses digital signatures inside broader questions; the stand-alone 2-mark definition is 9608's. `9608_s21_qp_12_sc_8.b`

> [!warning] Define firewall *and* authentication together and explain how each helps
> **Firewall:** sits between the computer/LAN and the internet/WAN, permits or blocks traffic to and from the network; can be hardware and/or software; a software firewall can detect illegal attempts by specific software to connect to the internet. **Authentication:** the process of determining whether somebody is who they claim to be; usually log-on passwords or biometrics; because passwords can be stolen or cracked, digital certification is used. `9608_s15_qp_13_sc_3.a`

> [!warning] Describe two **non-physical** methods of improving system security, with expansion
> User accounts · firewall (all traffic passes through it, blocks signals that do not meet requirements, **keeps a log of signals**, application network access can be restricted) · anti-malware (scans, quarantines or deletes, scheduled scans, kept up to date) · **auditing** (logging all actions/changes to the system to identify unauthorised use) · **application security** (regular updates/patches, finding and fixing vulnerabilities). Auditing and application security appear in **no 9618 mark scheme**. `9608_s19_qp_13_sc_2.b`

> [!warning] Give examples of when a virus checker should perform a check
> Boot-sector check when the machine is first turned on · when an external storage device is connected · when a file or web page is accessed or downloaded. `9608_w15_qp_13_sc_10.b`

> [!warning] Complete a table of security measure ↔ description (disk mirroring / encryption / backup)
> `9608_s20_qp_11_sc_1.b`

> [!warning] Identify a term from a description (router / server / gateway / firewall)
> "Monitors and controls incoming and outgoing network traffic based on set criteria" → firewall. Links this topic to Chapter 2. `9608_s21_qp_11_sc_9.b`

> [!info] Physical security measures
> The syllabus says measures "ranging from the stand-alone PC to a network", and physical methods (locked rooms, CCTV, secure entry devices, swipe cards) appear only as **accepted alternatives** inside 9618 mark schemes (`s25_qp_13_sc_3.b` allows "the computer storing the data cannot be accessed without the key to the room"). A question that asks specifically for physical measures, or contrasts physical with non-physical, is untested in 9618.

> [!info] Biometrics described rather than named
> "Biometric passwords" is accepted as a one-word answer in `s21_qp_12_sc_8.b`, but no 9618 question asks candidates to **describe** biometric authentication or say why it is more secure than a password.

> [!abstract] Biometrics, listed
> Personal characteristics used to identify an individual: **fingerprints, iris/retina scans, voice recognition**. Very secure, and common on mobile devices for access. The named list is the missing detail behind the one-word mark point above — and note facial recognition links straight to the AI bullet in Chapter 7.

> [!abstract] Why authentication exists at all
> Authentication asks the user to complete a task to prove they are an authorised user — partly because **bots can submit data in online forms**. A framing no mark scheme gives, and a clean justification for CAPTCHA-style measures.

> [!abstract] Symmetric vs asymmetric encryption
> **Symmetric:** the same key encrypts and decrypts — fast, but the key must be shared securely. **Asymmetric:** a **public key** encrypts and a **private key** decrypts — more secure for sending data. Neither term appears in the 9618 syllabus for this topic or in any mark scheme here (encryption is always credited as "a key is needed to decode"), so know it for understanding and answer in the syllabus's own words.

> [!abstract] Hardware vs software firewalls
> A **hardware** firewall protects the whole network and blocks unauthorised traffic; a **software** firewall protects individual devices, monitoring data to and from each computer. Often used together. The 9618 mark schemes never split the two.

---

## 6.1.4 Show understanding of the threats posed by networks and the internet

> [!success] Identify a threat, describe it, and give a method of prevention (table)
> **Malware/virus** — malicious code that can alter/delete files → anti-virus/anti-malware/firewall. **Spyware** — records keystrokes which are sent to a third party → anti-spyware/firewall/anti-malware. **Hacking** — gaining unauthorised access to a computer network/device → authentication/firewall. **Phishing** — emails supposedly from reputable companies sent to trick people into revealing personal information → spam filter / do not open emails from unknown sources. **Pharming** — users are directed to a bogus **website** that looks legitimate to obtain personal information → VPN / anti-malware / do not open links or download attachments. `9618_w25_qp_12_sc_5.e`

> [!success] Describe a threat posed by networks and the internet in a scenario
> `9618_w25_qp_11_sc_8.a`, `9618_w23_qp_13_sc_8.b`, `9618_w23_qp_12_sc_5.c`

> [!warning] Explain the term computer virus
> Malicious code / software / program **that replicates or copies itself**; can cause loss or corruption of data; can cause the computer to crash or run slowly; **can fill up the hard disk with data**. The self-replication point is the defining feature and appears in **no 9618 mark scheme** — 9618 only ever says "malicious code that can alter/delete files". `9608_w15_qp_13_sc_10.a`

> [!info] The distinction between virus, worm, trojan and spyware
> The syllabus notes name only *virus* and *spyware*, and 9618 credits them as a single "malware" family. A question asking candidates to distinguish two named types of malware is a natural extension but sits at the edge of the syllabus wording.

> [!info] Why the *network and internet* make these threats possible
> Every question so far names a threat and asks for a description. The bullet's actual wording — threats **posed by networks and the internet** — invites "explain why connecting to the internet increases the risk to a stand-alone PC", which has not been asked in either series.

> [!abstract] Trojan
> Sometimes called a Trojan Horse: software that **disguises itself as legitimate software** but contains malicious code running in the background. Not named in the 9618 syllabus notes (which list only virus and spyware) — know it, but do not offer it where a syllabus-named example is wanted.

> [!abstract] How hackers actually get in
> Hackers look for vulnerabilities: **unpatched software** (missing security updates), **out-of-date anti-malware**, and **weak or reused passwords**. This is the "why" behind the credited prevention points (keep software up to date, update anti-malware, use strong passwords).

> [!abstract] Effects of a successful attack
> Data breaches (information leaked or stolen) · further malware installation · data loss (files deleted or corrupted) · **identity theft** · financial loss (bank access or ransom demands). Useful for the "describe the impact" half of a threat question.

> [!abstract] Phishing as social engineering, and how it is prevented
> Phishing is a form of **social engineering**: fraudulent, legitimate-looking emails sent to a large number of addresses, usually coaxing the user to click a login button. Prevention: anti-spam filters, **training staff to recognise fraudulent emails**, and **user access levels that stop staff opening executable (.exe) or batch (.bat) files**. The staff-training and file-type points are not in any mark scheme here but are well within "methods to restrict the risks".

> [!abstract] How pharming works technically
> The attacker **alters DNS settings or the user's browser settings** so that typing a legitimate address redirects to a fraudulent site. Prevention: keep anti-malware up to date, check URLs, look for the padlock icon. The DNS-alteration mechanism ties this bullet to the DNS content in Chapter 2 and is absent from the 9618 mark scheme, which says only "users are directed to a bogus website".

---

## 6.1.5 Describe methods that can be used to restrict the risks posed by threats

> [!success] Explain how the data security risks of malware can be restricted
> Download programs from reputable sources (less likely to contain malware) · back up / archive systems (so data can be restored after a malware installation) · install and run an anti-malware program (regular scans, quarantine or removal, definitions regularly updated) · firewall blocking unused ports (so malware cannot enter) · **deny administrator privileges to everyday users** (so malware cannot be downloaded) · **avoid the use of removable devices**. `9618_w23_qp_13_sc_8.c`

> [!success] Identify and describe one method of restricting the risk of interception during transfer
> **Encryption:** data is encoded/scrambled using a key to create cipher text; if intercepted it cannot be understood without being decrypted using a key. `9618_s25_qp_11_sc_7.a`

> [!success] Identify and describe a prevention method for a named threat
> `9618_w25_qp_12_sc_5.e`, `9618_s23_qp_13_sc_6.b`

> [!info] Restricting risk by *user behaviour* rather than software
> The `w23_qp_13_sc_8.c` mark scheme is unusually behavioural (reputable sources, deny admin rights, avoid removable devices) and is the only 9618 question of its kind. Staff training, acceptable-use policies and being alert to suspicious emails are natural extensions the current series has not asked for.

> [!info] Two-factor authentication
> Accepted as a one-word answer in `s21_qp_12_sc_8.b` and named in SME, but never **described** ("something you know plus something you have"; a code sent to a separate device) in either series.

---

## 6.1.6 Describe security methods designed to protect the security of data

> [!success] Explain how encryption protects data during transmission
> Encodes/scrambles the data … so if it is intercepted it cannot be **understood** … an algorithm/key is required to decode it. `9618_s24_qp_13_sc_7.f.ii`

> [!success] Identify one method of keeping files secure *during transmission* and one *on the computer*
> During transmission → encryption (incl. by example such as a **VPN**). On the computer → firewall/proxy (filter incoming transmissions and stop attempted unauthorised access) // anti-malware (find and delete or quarantine malware) // encryption // a physical method (the computer cannot be accessed without the key to the room). `9618_s25_qp_13_sc_3.b`

> [!success] Identify a security method to protect program code during email transfer
> Encryption: file contents converted to cipher text; if intercepted the data cannot be understood without the decryption key. `9618_w24_qp_12_sc_4.c`

> [!success] Describe how access rights protect data
> Different accounts with read-only / no access / read-write; views restricting what each user sees. `9618_w21_qp_11_sc_5.b`

> [!warning] Explain how encrypting *source code stored on a laptop* keeps it secure
> Encryption scrambles the source code so it is meaningless, using an encryption key/algorithm; if accessed without authorisation it is meaningless; a decryption key is needed to unscramble. Same content, but 9618 has only ever asked about encryption **in transit** or as a table entry, never about a stored file on a stand-alone machine. `9608_s20_qp_13_sc_5.a`

> [!warning] Describe three security measures a bank could implement to protect electronic data (paired points)
> Firewall (and ensuring it is switched on) → stops hackers accessing the network · authentication with strong passwords/biometrics · encryption → data is meaningless without the decryption key · access rights → stops users reading or editing data they are not permitted to · up-to-date anti-malware → detects, removes or quarantines viruses and key-loggers · **regular backups to a separate or off-site device** → enables recovery · physical security, by example. `9608_s16_qp_13_sc_7.b`

> [!info] Backup as a data-*security* method
> Backup appears as a mark point inside the 9618 malware question (`w23_qp_13_sc_8.c`) but has **never** been the subject of a 9618 question, despite being the classic answer to "protect data against loss". Both 9608 questions above lean on it heavily. Given the syllabus splits security into protecting *against loss* and *against unauthorised access*, the loss half is thinly examined in the current series.

> [!abstract] Access rights, described properly
> Access rights control what users can see or do, assigned by **role, responsibility or security clearance**. Three levels: **full access** (open, create, edit, delete) · **read-only** (open and view, cannot edit or delete) · **no access** (cannot see or interact with the file at all). Users can be **grouped** ("Year 11", "Staff", "Admin") and given rights as a group, and rights can be applied to files, folders or whole systems. The grouping point is the one 9618 mark schemes do not make.

> [!abstract] How wireless data is encrypted — the master key
> The network's **SSID plus a password** creates a **master key**; devices joining with the SSID and password receive a copy. The master key encrypts data into **cipher text** before transmission and the receiver decrypts it back to **plain text**. Crucially, **the master key is never transmitted**, so intercepted data is useless. Wireless uses dedicated protocols such as **WPA2**. Wired networks work the same way, except encryption is often left to individual applications — e.g. **HTTPS**. This is the fullest version of the "a key is required" mark point and ties the topic to wireless networks in Chapter 2.

---

# 6.2 Data Integrity

## 6.2.1 Describe how data validation and data verification help protect the integrity of data

> [!success] State the difference between data verification and data validation
> Verification checks whether input data is **the same as the original**; validation checks that the data is **reasonable / sensible**. `9618_w22_qp_12_sc_4.a`

> [!success] Describe how data validation helps protect integrity, with an example
> Validation checks that data is reasonable/sensible and within specified bounds; example — checking data is the right number or type of characters. `9618_w21_qp_11_sc_2.b.i`

> [!success] Describe how data verification helps protect integrity, with an example
> Verification checks that data is the same as the original; example — double entry. `9618_w21_qp_11_sc_2.b.ii`

> [!success] Describe one *other* method of protecting integrity when given verification
> Validation (named or described) … protects the data by ensuring it is reasonable/sensible and within specified bounds. `9618_w23_qp_13_sc_8.a`

> [!success] State why data might still be incorrect even after validation and verification
> The value on the original document may be in the correct format but simply be the **wrong value** for that record. `9618_s23_qp_13_sc_4.d.iii`

> [!warning] Explain why "validation makes sure data keyed in is the same as the original" is wrong
> That is a description of **verification**; validation ensures data is reasonable/sensible or within given criteria; **original data may have been entered correctly but still not be reasonable (e.g. age 210)**. The misconception format is 9608's, and it is the sharpest test of the distinction. `9608_w16_qp_13_sc_7.c.ii`

> [!warning] State ways of maintaining integrity at the **input stage** vs **during transfer**, with examples
> Input: validation (range, type, length checks) and verification (double entry, visual check). Transfer: parity checking and checksum. 9618 splits these across separate questions; the "two ways at each stage, with examples" framing is 9608's. `9608_s15_qp_13_sc_3.c.i`, `9608_s15_qp_13_sc_3.c.ii`

> [!warning] Give a brief description of each of the terms validation and verification (definition only)
> Validation — check whether data is reasonable / meets given criteria. Verification — a method to ensure data which is copied or transferred is the same as the original; entering data twice and the computer comparing; checking entered data against the original document. `9608_w15_qp_13_sc_9.a`

> [!info] Why validation and verification together are needed
> Every question tests one, the other, or the difference. "Explain why a system uses both validation and verification" — validation catches unreasonable data, verification catches mis-keying, and neither alone catches both — is the synthesis question neither series has set, and `s23_qp_13_sc_4.d.iii` is the closest Cambridge has come.

> [!abstract] The clean definitions
> **Validation** is an *automated* process where the computer checks that input is sensible and meets the program's requirements. **Verification** is checking that data is *accurate* when transferred or entered. Note SME's placement of the methods: parity check and checksum belong to **transfer**; double entry and visual check belong to **entry** — exactly the split `9618_w25_qp_12_sc_1` tests.

> [!abstract] More than one validation check per field
> A single field often carries several checks at once — e.g. a password field with a **length, presence and type** check. Explains why 9618 questions routinely ask for "two other ways the field can be validated" on one field.

---

## 6.2.2 Describe and use methods of data validation

> [!success] Identify the validation method performed by a pseudocode algorithm
> `IF x < 1 OR x > 26` → **range check** · `IF x <> 'R' AND x <> 'G' AND x <> 'B'` → **existence check** · a loop searching for "@" using MID/LENGTH → **format check** · `IF x = ""` → **presence check**. `9618_w25_qp_13_sc_7.e`

> [!success] Describe two ways a car registration number can be validated
> **Length check** (must be 6 characters) · **format check** (letter-digit-digit-digit-letter-letter) · **type check** (must be alphanumeric). `9618_s23_qp_13_sc_4.d.i`

> [!success] Describe two methods of validating a field with a fixed set of values
> **Presence check** (the value is entered) · **look-up / existence check** (only Beginner, Intermediate or Advanced) · **length check** (8 or 12 characters) · **type check** (alphanumeric). `9618_s23_qp_12_sc_2.c.i`

> [!success] Describe two validation methods for **non-numeric** data
> Required format / only expected characters allowed · data already present in the system · correct number of characters · ensuring non-numeric data is entered. `9618_w22_qp_12_sc_4.c`

> [!warning] Write the validation **type** for each validation description in a table
> "A name must be entered" → presence · "entered as dd/mm/yyyy" → format · "a limit of 15 characters" → length · "only values between 1 and 5" → range. 9618 asks candidates to read pseudocode or invent checks; the plain description→type table is 9608's. `9608_s21_qp_13_sc_1.a`

> [!warning] **Check digit: the calculation.** Compute a modulus-11 check digit
> Multiply each digit by its weighting, total, divide by 11, take the remainder, subtract from 11 to get the check digit (e.g. 786531 → total 128 → 128 MOD 11 = 7 → 11 − 7 = **4** → 7865314). **Check digit is named in the 9618 syllabus notes and has NEVER been examined in the 9618 series — in any form.** `9608_w17_qp_13_sc_3.b.i`

> [!warning] Uniqueness check
> "Each PatientID must be unique" — credited as a named validation check alongside length, format and presence. Not in the 9618 syllabus list of seven, but accepted in 9608 for a database key. `9608_w17_qp_13_sc_3.b.ii`

> [!warning] Tick table: is this measure validation or verification?
> Checksum → verification · format check → validation · range check → validation · double entry → verification · **check digit → validation**. `9608_s18_qp_12_sc_3.c`

> [!warning] Name and describe two validation checks appropriate for a data-capture form
> Range check (number between 1 and 100) · format check (digit characters only) · length check (exactly five characters) · existence check (the product code has been assigned). `9608_s17_qp_13_sc_7.c.v`

> [!info] Check digit — the biggest gap in Chapter 6
> The syllabus notes list seven methods: *range, format, length, presence, existence, limit, check digit*. 9618 has examined range, format, length, presence, existence and type. **Check digit has never appeared in 9618 at all**, and 9608 examined it as both a definition and a full modulus-11 calculation. Treat it as overdue and be ready to *calculate* one, not just name it.

> [!info] Limit check
> Also named in the syllabus notes and **never distinguished from a range check** in any 9618 question. A limit check bounds one end (no more than 5 items); a range check bounds both (0–100). A question that requires the correct one of the two is available and would catch most candidates.

> [!info] Type check is not on the syllabus list — but is credited
> `s23_qp_13_sc_4.d.i` and `s23_qp_12_sc_2.c.i` both credit "type check", yet it is **not** one of the seven named in the notes. Safe to use, but lead with a syllabus-named check where the question allows only two.

> [!info] Writing validation as pseudocode rather than reading it
> `w25_qp_13_sc_7.e` and `s21_qp_11_sc_6` give you the algorithm and ask for the name. The syllabus says "describe **and use** methods of data validation" — being asked to *write* the IF statement that performs a stated check is the untested direction, and links directly to Paper 2.

> [!abstract] The seven checks with worked examples
> **Range** — a number falls within a set range (a percentage between 0 and 100) · **Limit** — a value does not exceed a maximum (no more than 5 items in an offer) · **Length** — a string's length (a PIN is exactly 4 digits) · **Type** — the correct data type (age is a whole number) · **Presence** — the field is not blank · **Existence** — a referenced value exists in a database or list (a student ID that exists in the school records) · **Format** — data matches a pattern (an email contains '@' and '.com').

> [!abstract] What a check digit actually catches
> The last digit of a code, calculated from the others by a standardised algorithm, used to detect **incorrect digits entered, omitted or extra digits, and phonetic errors**. Used in **ISBNs** (the final digit makes the weighted total divide exactly, with no remainder) and **barcodes** (the final digit validates the scanned item). The error-types list and the ISBN/barcode contexts are the framing behind the 9608 calculation above.

---

## 6.2.3 Describe and use methods of data verification during data entry and data transfer

> [!success] Match each verification method to data transfer or data entry
> Parity byte check → transfer · checksum → transfer · **visual check → entry** · parity block check → transfer. `9618_w25_qp_12_sc_1`

> [!success] Identify and describe one verification method for data transfer
> **Parity byte check:** a parity bit is added to each byte to make the number of 1s match the agreed parity, odd or even; each byte is checked on receipt and a resend requested if it does not match. **Parity block check:** a bit is added to each byte *and* a parity byte is set for each block; the location of an error can be found using vertical and horizontal parity. **Checksum:** a calculation is made from the data and transmitted with it; the receiver repeats the calculation and compares. `9618_w25_qp_13_sc_7.c`

> [!success] Complete the missing parity bit for a byte using even parity
> `9618_w25_qp_12_sc_6.c.i`

> [!success] Circle the altered bit in a parity block
> Cross-reference the row with incorrect parity against the column with incorrect parity; the intersection is the error. `9618_w25_qp_12_sc_6.c.ii`

> [!success] Explain how data can be verified using a checksum
> The data is put through an algorithm to create a checksum value → data and checksum are sent to the receiver → the receiver performs the same algorithm on the data → if both checksums match, the data is verified. `9618_s25_qp_11_sc_7.c`

> [!success] Complete a description of parity check (cloze)
> Sender and receiver agree **odd or even** parity; data is divided into groups of **7 bits**; if parity is **odd** and the group has an even number of 1s, a parity bit of 1 is appended. In a parity **block** check, the bits in each column are counted and transmitted as a parity **byte**. `9618_s24_qp_11_sc_5.b`

> [!success] Explain how data verification is used when an identifier is entered
> **Visual check:** the administrator checks by eye that the input matches the identifier on the **original document**. **Double entry:** the administrator (or a second person) enters it a second time and **the system** compares it with the first entry. `9618_w23_qp_13_sc_3.c`

> [!success] Describe two ways data can be verified on entry
> Visual check (manually compare with the source document) · double entry (enter twice and the computer compares). `9618_s23_qp_13_sc_4.d.ii`

> [!warning] Describe how a parity **block** check identifies a corrupted bit, in full
> Each byte has a parity bit (horizontal parity) · an additional **parity byte** is sent carrying the vertical parity · each row and column must have an even/odd number of 1s · identify the incorrect row and the incorrect column · **the intersection is the error**. 9618 asks you to *circle* the bit; the 4-mark "describe how it works" is 9608's. `9608_s19_qp_13_sc_2.c.i`

> [!warning] Give a situation where a parity block check **cannot** identify corrupted bits
> Errors in an **even number of bits** (in the same row or column) — they cancel each other out, so the error is not identified and the data could appear correct. **The single most important limitation of parity, and it has never been asked in 9618.** `9608_s19_qp_13_sc_2.c.ii`

> [!warning] Identify **two** bits that must be changed to remove errors in a block, and explain the method
> Consider each row in sequence → identify any row with incorrect parity → repeat for each column → identify where a row and column with incorrect parity intersect. 9618's version has exactly one error; the two-error variant is harder and 9608-only. `9608_s17_qp_13_sc_5.b.ii`

> [!warning] Describe how a sender **calculates** the parity bit for each byte
> Count the number of 1 bits in the **first seven** bit positions; add a 0 or 1 to bit position 0 to make the count of 1 bits match the agreed parity. `9608_s17_qp_13_sc_5.a.i`

> [!warning] Explain what is meant by a parity check, with an example
> Parity can be even or odd; it uses the number of 1s in a binary pattern; after transmission the parity of each byte is re-checked; a parity bit is used to make the pattern have the correct parity — plus a worked example. `9608_w15_qp_13_sc_9.b`

> [!warning] Hash total
> A total of several fields of data, **including fields not usually used in calculations**, transmitted with the data, recalculated at the receiving end and compared. Named as an alternative to checksum in 9608; **not in the 9618 syllabus notes**, so treat as background. `9608_s18_qp_11_sc_6.d`

> [!warning] Proof reading
> Credited as a **verification** method alongside visual check and double entry in 9608 matching questions. Not named in the 9618 notes, which say only "visual check, double entry". `9608_s18_qp_13_sc_4.c`

> [!info] The limitation of a plain parity check
> Both the "even number of errors" point and the fact that a parity check **detects that an error occurred but not where** are absent from every 9618 mark scheme. Given that `w25_qp_12_sc_6.c.ii` asks candidates to locate an error with a parity *block*, a follow-up asking why a single parity bit could not do that is the obvious next step.

> [!info] Automatic repeat request / resend
> "Request to be resent if the byte does not match parity" appears once, inside the `w25_qp_13_sc_7.c` mark scheme. What actually happens after an error is detected — a retransmission request — is never the subject of a question in either series.

> [!info] Calculating a checksum rather than describing one
> Both series only ever ask for the *process*. 9608's hash-total wording ("adds up the bytes in the data being sent") shows a numeric version is possible, and "use methods of data verification" invites it.

> [!abstract] Parity — why errors happen
> Bits get **flipped by interference** — on a wire, or wirelessly through weather or other signals. The physical cause behind "an error has occurred", and it links this topic to transmission media in Chapter 2.

> [!abstract] The parity check's blind spot, stated plainly
> Parity checks are quick and easy to implement but **fail to detect bit swaps that leave the parity unchanged**, and they show only *that* an error occurred, not *where*. This is why parity blocks and bytes exist — a parity block totals the 1s **horizontally and vertically**, and cross-referencing the two pinpoints the faulty cell, which can then be corrected automatically or trigger a retransmission request.

> [!abstract] Checksum, in one line
> A value calculated from the data by an algorithm and added to the transmission; the receiver recalculates and compares. Like parity, it indicates that data **differs from its original form but not where** — the same limitation, worth saying explicitly.

> [!abstract] The two entry-verification methods, precisely
> **Double entry** — the data is entered twice in separate input boxes and compared; an error message is shown if they differ. **Visual check** — the user reads the data on screen and a prompt asks whether it is correct before proceeding; if not, it is entered again. Note the mark schemes are strict about *who* compares: for double entry **the system/computer** compares, for a visual check **the person** compares against the original document.
