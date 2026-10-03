---
title: Pack — 6 Security, privacy and data integrity (AS Level)
syllabus: 9618 (2026)
topics: 6.1 Data Security · 6.2 Data Integrity
pairs with: Jigsaw
---

# Pack — 6 Security, privacy and data integrity

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **9608 |** — same rule, using 9608 tariffs. In the 9618 syllabus, untested in the current series.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way. Weigh against the mark schemes.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

---

# 6.1 Data Security

## 6.1.1 Security, privacy and integrity of data

> [!question] 9618 | State the meaning of privacy of data [1]
> State the meaning of **privacy of data**.
>
>> [!success]- Answer — 3 points for 1 mark
>> - Ensuring data can only be accessed by / disclosed to **authorised** persons
>> - **OR** ensuring data cannot be accessed by / disclosed to **unauthorised** persons
>> - Keeping data confidential
>>
>> *Latest: `9618_w23_qp_12_sc_5.a`*

> [!question] 9618 | State the meaning of integrity of data [1]
> State the meaning of **integrity of data**.
>
>> [!success]- Answer — 3 points for 1 mark
>> - Ensuring the accuracy / completeness / consistency of data (during or after processing)
>> - Ensuring the data is up to date
>> - Ensuring the data received is the same as the data sent
>>
>> *Latest: `9618_w23_qp_12_sc_5.b`*

> [!question] 9618 | Explain the difference between data security and data integrity [2]
> Explain the difference between **data security** and **data integrity**.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Security is protecting data from loss / corruption
>> - Integrity is ensuring the consistency / accuracy of the data
>> - Security also covers protection from unauthorised access
>> - Integrity also covers ensuring the data is up to date
>>
>> *Latest: `9618_w21_qp_11_sc_2.a`*

> [!question] 9618 | Describe the difference between security and privacy of data [2]
> Describe the difference between the **security** and **privacy** of data.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Security protects data against **loss**
>> - Privacy protects data against **unauthorised access**
>> - Security covers accidental or malicious damage
>> - Privacy keeps data confidential, so only authorised personnel see it
>>
>> *Latest: `9618_s21_qp_12_sc_8.a`*

> [!question] 9618 | Sort measures into data security or data integrity [2]
> Draw one line from each measure (firewall, double entry, presence check, access rights, password) to indicate whether it keeps data secure or protects the integrity of data.
>
>> [!success]- Answer — 5 lines for 2 marks (1 mark for the 3 security lines, 1 mark for the 2 integrity lines)
>> - Firewall → **Data Security**
>> - Double entry → **Data Integrity**
>> - Presence check → **Data Integrity**
>> - Access rights → **Data Security**
>> - Password → **Data Security**
>>
>> *Latest: `9618_w21_qp_12_sc_1`*

> [!question] 9618 | State what is meant by data integrity and give a database example [2]
> State what is meant by **data integrity** and give **one** example of how this is implemented in a database.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Definition: methods of making sure the data is consistent
>> - Example: enforcing **referential integrity**
>> - Example: if data in one table is deleted or edited, all tables are updated // cascading update/delete
>> - Example: validation / verification rules
>>
>> *Latest: `9618_s23_qp_11_sc_2.a.ii`*

> [!question] 9608 | Describe the difference between security and integrity of data [4]
> Describe the difference between the **security** and **integrity** of data.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Security is keeping the data safe
>> - Security is the prevention of data **loss**
>> - Integrity is making sure that the data is correct / valid
>> - Integrity ensures that the data received is the same as the data sent // the data copied is the same as the original
>> - Example of ensuring security, e.g. usernames and passwords, firewalls
>> - Example of ensuring integrity, e.g. parity checks, double entry
>>
>> *Latest: `9608_s16_qp_13_sc_7.a`. `9608_s15_qp_13_sc_3.b` adds: integrity deals with the validity of data / freedom from errors; integrity means data is not corrupted after, for example, being transmitted.*

> [!question] 9608 | Explain the difference between security and privacy of data [3]
> Explain the difference between the **security** and **privacy** of data.
>
>> [!success]- Answer — 6 points for 3 marks
>> - Security is keeping the data safe
>> - … from accidental / malicious damage or loss
>> - … by example of the need for security
>> - Privacy is the need to restrict access to **personal** data
>> - … to avoid it being seen by unauthorised people
>> - … by example of the need for privacy
>>
>> *Latest: `9608_w17_qp_12_sc_3.a.i`*

> [!question] 9608 | Give an example where privacy of data is a key concern [1]
> Give **one** example, for a school LAN, where privacy of data is a key concern.
>
>> [!success]- Answer — 2 points for 1 mark
>> - The personal data of students
>> - The personal data of staff
>>
>> *Latest: `9608_w17_qp_12_sc_3.a.ii`*

> [!question] 9608 | Identify the term from a description [3]
> Complete the table by identifying the most appropriate term for each description. Each term must be different.
>
>> [!success]- Answer — 3 rows for 3 marks
>> - Ensures data is accurate and up to date → **Data integrity**
>> - Prevents accidental or malicious data loss → **Data security**
>> - Prevents unauthorised access to data → **Data privacy**
>>
>> *Latest: `9608_s21_qp_12_sc_8.a`*

> [!question] 9608 | How a database manager can ensure data integrity [2]
> State what is meant by **data integrity** and give an example of how a database manager can ensure it.
>
>> [!success]- Answer — 6 points for 2 marks (1 description + 1 example)
>> - Description: ensure data is consistent / accurate
>> - Example: validation rules
>> - Example: referential integrity
>> - Example: verification // input masks // setting data types
>> - Example: removing redundant data // backup data
>> - Example: access controls // **audit trail**
>>
>> *Latest: `9608_s18_qp_13_sc_2.b`*

> [!question] Inferred | Explain all three terms with an example of each [4]
> Explain the difference between the security, privacy and integrity of data. Give an example of each.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Security protects data from loss or corruption, accidental or malicious … e.g. backup, firewall
>> - Privacy restricts access to personal data to authorised people … e.g. access rights, passwords
>> - Integrity ensures data is accurate, consistent and up to date … e.g. validation, parity check
>> - Security is about **keeping the data safe**
>> - Privacy is about **who is allowed to see it**
>> - Integrity is about **whether it is correct**
>>
>> *9618 asks two-way comparisons only. Tariff set to 4 to match `9608_s16_qp_13_sc_7.a`.*

> [!question] SME | Privacy and consent [2]
> Explain what data privacy requires of an organisation collecting personal data.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Data must be collected, stored and shared in a way that respects the user's rights
>> - The user's **consent** must be obtained before collecting or sharing personal information
>> - Only authorised people may access the data
>> - The organisation controls who can access and use the personal data
>>
>> *Tariff set to 2. The consent framing is not in any mark scheme in this topic.*

---

## 6.1.2 The need for both security of data and security of the computer system

> [!question] 9608 | How backup and disk-mirroring allow recovery from data loss [4]
> Explain how **data backup** and **disk-mirroring** allow a company to recover from data loss. *(Max 2 marks each.)*
>
>> [!success]- Answer — 6 points for 4 marks
>> - Backup: a copy of the data will have been made …
>> - … and stored elsewhere / in another location
>> - … if the original is lost, the backup can be used to restore the data
>> - Disk-mirroring: the data is stored on two disks simultaneously
>> - … if the first disk drive fails, the data is accessed from the second disk
>> - … so there is no interruption to service
>>
>> *Latest: `9608_s19_qp_11_sc_4.b`. **This bullet has no 9618 question at all.***

> [!question] 9608 | Methods of preventing accidental loss of data [2]
> Describe **two** methods of preventing accidental loss of data.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Frequent backup — to secondary media, a third-party server, the cloud, or removable devices, or stored remotely
>> - Continuous backup
>> - Disk-mirroring strategy / **RAID**
>> - **UPS (uninterruptable power supply)** / backup generator
>>
>> *Latest: `9608_s15_qp_11_sc_6.b.i`*

> [!question] 9608 | Why "encryption prevents hackers breaking in" is wrong [2]
> An employee states: *"Encryption prevents hackers breaking into the company's computers."* Explain why this answer is incorrect.
>
>> [!success]- Answer — 3 points for 2 marks
>> - Hackers can still **access** the data (and corrupt it, change it or delete it)
>> - Encryption simply makes the data **incomprehensible**
>> - … without the decryption key / algorithm
>>
>> *Latest: `9608_w16_qp_13_sc_7.c.i`. This is the sharpest test of "security of the **system**" vs "security of the **data**".*

> [!question] 9608 | Why "passwords always prevent unauthorised access" is wrong [2]
> An employee states: *"The use of passwords will always prevent unauthorised access to the data stored on the computers."* Explain why this answer is incorrect.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A password does not **prevent** unauthorised access, it makes it more **difficult**
>> - A password can be guessed, if it is weak
>> - A password can be stolen
>> - A relevant example of misappropriation of a password
>>
>> *Latest: `9608_w16_qp_11_sc_7.c.iii`*

> [!question] Inferred | Why a company needs both [3]
> Explain why a company needs to secure both its data **and** its computer system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Securing the system stops unauthorised people gaining access in the first place … e.g. firewall, user accounts, physical locks
>> - Securing the data means that even if the system is breached, the data itself is protected … e.g. encryption, access rights
>> - Encryption alone does not stop a hacker deleting or corrupting the data
>> - A firewall alone does not protect data that is intercepted in transit
>> - Backup protects against loss, which neither a firewall nor encryption addresses
>>
>> *The Legend has **zero** 9618 questions under this bullet. Tariff set to 3.*

> [!question] SME | Why passwords are stored encrypted [2]
> Explain why passwords are stored in encrypted form in a database.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Passwords are stored as encrypted / ciphered text
>> - So even if a hacker gains unauthorised access to the database …
>> - … they cannot read the individual users' passwords
>> - … so they cannot use them to log in to the accounts
>>
>> *Tariff set to 2.*

---

## 6.1.3 Security measures for computer systems

> [!question] 9618 | Explain how a digital signature authenticates a document [5]
> Explain how a digital signature is used to authenticate a digital document during transmission over a network.
>
>> [!success]- Answer — 8 points for 5 marks
>> - The sender **hashes** the document / message
>> - … to produce a **digest**
>> - The sender **encrypts** the digest to create the digital signature
>> - The message and the signature are sent to the receiver
>> - The receiver **decrypts** the signature to reproduce the digest
>> - The receiver uses the **same** hashing algorithm on the document received to produce a second digest
>> - The receiver compares this digest with the one from the digital signature
>> - If both digests are the same, the document is authentic / has not been changed
>>
>> *Latest: `9618_s23_qp_13_sc_6.a`; `9618_s25_qp_11_sc_7.b` is the identical 5-marker asking whether the data has **not been changed**. `9618_w22_qp_12_sc_6.a.i` (2 marks) adds: the digest is encrypted with the **sender's private key**, and the signature can only be decrypted with the matching **sender's public key**.*

> [!question] 9618 | Draw lines from each security feature to its description [4]
> Draw one line from each security feature (firewall, pharming, anti-virus software, encryption) to its most appropriate description.
>
>> [!success]- Answer — 4 lines for 4 marks
>> - Firewall → accepts or rejects incoming and outgoing packets based on criteria
>> - Pharming → redirects a user to a false website
>> - Anti-virus software → scans files on the hard drive for malicious software
>> - Encryption → converts data to an alternative form
>> - *Unused distractor:* verifies the authenticity of data (that is a digital signature)
>>
>> *Latest: `9618_w22_qp_11_sc_2`*

> [!question] 9618 | Describe how a firewall protects the data on a computer [3]
> Describe how a firewall protects the data on a computer.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Monitors** incoming and outgoing packets / traffic
>> - **Checks against** an allow list / deny list of IP addresses // checks against a set of rules for acceptable data, ports etc.
>> - **Blocks** transmissions that do not meet the criteria / rules // **allows** through those that satisfy the criteria
>> - Blocks data entering from specific ports
>> - Blocks unauthorised or unknown internal software from transmitting data
>>
>> *Latest: `9618_w22_qp_12_sc_6.a.ii`; `9618_s24_qp_11_sc_5.c.i` is the customer-data version.*

> [!question] 9618 | Identify one other security measure protecting a server from hackers, and describe how it works [3]
> Authentication methods help protect a server against hackers. Identify **one other** security measure and describe how it works. *(1 mark measure + max 2 description.)*
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Firewall** … checks **incoming** connections against criteria
>> - … blocks data from entering specific ports
>> - … blocks data that does not meet a whitelist / that meets a blacklist
>> - **Proxy server** … prevents devices accessing the web server directly, intercepting any requests
>> - … forwards the request using its own IP address, and screens returning data before sending it to the user
>>
>> *Latest: `9618_s24_qp_12_sc_3.a.i`*

> [!question] 9618 | State how firewall, encryption and passwords protect computer systems [3]
> State how each of the following security measures can be used to protect computer systems: firewall, encryption, passwords.
>
>> [!success]- Answer — 3 points for 3 marks (1 each)
>> - **Firewall**: monitors incoming and outgoing traffic and rejects any traffic that does not meet the set rules
>> - **Encryption**: ensures that if data is intercepted or obtained it cannot be understood without the decryption key
>> - **Passwords**: ensures only users with the correct password can access the resources // prevents unauthorised access
>>
>> *Latest: `9618_w23_qp_13_sc_3.a.iii`*

> [!question] 9618 | Identify and describe two types of software that prevent threats over a network [2]
> Complete the table by identifying **and** describing **two** types of software that can be installed on a computer to prevent threats over a network.
>
>> [!success]- Answer — 4 options for 2 marks (1 mark per identification **and** matching description)
>> - **Antivirus** — scans the computer for viruses, checking against a stored database of virus signatures that must be updated regularly, then deletes or quarantines them; compares downloaded files to the database and prevents the download continuing
>> - **Antispyware** — the same process, for spyware
>> - **Antimalware** — the same process, for malware generally
>> - **Firewall** — monitors **incoming and outgoing traffic** and compares it to criteria set by the user, such as a whitelist/blacklist or allowed/blocked IP addresses, blocking those that do not match
>>
>> *Latest: `9618_s23_qp_13_sc_6.b`*

> [!question] 9618 | Identify one software-based measure to restrict access to data [1]
> Employees have a username and password, and access rights set to read-only or read/write. Identify **one other** software-based measure that could restrict access to the data.
>
>> [!success]- Answer — 4 points for 1 mark
>> - Two-factor authentication
>> - Biometric passwords
>> - Key card access
>> - Firewall
>>
>> *Latest: `9618_s21_qp_12_sc_8.b`*

> [!question] 9618 | What makes a downloaded program authentic [1]
> A user downloads a computer program from the internet. State what should be included as part of the download to make sure the program is authentic.
>
>> [!success]- Answer — 1 point for 1 mark
>> - A digital signature
>>
>> *Latest: `9618_w25_qp_12_sc_10.c`*

> [!question] 9608 | Describe two non-physical methods of improving system security [6]
> Computer systems can be protected by physical methods such as locks. Describe **two non-physical** methods used to improve the security of computer systems. *(1 mark for the method + 2 for description, ×2.)*
>
>> [!success]- Answer — 8 points for 6 marks
>> - **User accounts** — each user has a username and password; access to resources can be limited to specific accounts; a user cannot access the system without a valid username and password
>> - **Firewall** — all incoming and outgoing traffic goes through the firewall; blocks signals that do not meet requirements; **keeps a log of signals**; application network access can be restricted
>> - **Anti-malware** — scans for malicious software; quarantines or deletes anything found; scans can be scheduled at regular intervals; should be kept up to date
>> - **Auditing** — logging all actions / changes to the system, in order to identify any unauthorised use
>> - **Application security** — applying regular updates and patches; finding, fixing and preventing security vulnerabilities in installed applications
>> - Encryption — scrambles the data so it is meaningless without the key
>> - Access rights — different users are given different permissions
>> - Two-step / biometric authentication
>>
>> *Latest: `9608_s19_qp_13_sc_2.b`. **Auditing and application security appear in no 9618 mark scheme.***

> [!question] 9608 | Define firewall and authentication, and explain how they help [3]
> Give the definition of the terms **firewall** and **authentication**. Explain how they can help with the security of data. *(Max 2 marks each.)*
>
>> [!success]- Answer — 8 points for 3 marks
>> - **Firewall**: sits between the computer or LAN and the internet / WAN
>> - … and permits or blocks traffic to and from the network
>> - … can be software and/or hardware
>> - … a software firewall can make precise decisions about what to allow or block, as it can detect illegal attempts by specific software to connect to the internet
>> - … can help to block hacking or viruses reaching a computer
>> - **Authentication**: the process of determining whether somebody or something is who or what they claim to be
>> - … frequently done through log-on passwords or biometrics
>> - … because passwords can be stolen or cracked, digital certification is used; helps prevent unauthorised access to data
>>
>> *Latest: `9608_s15_qp_13_sc_3.a`*

> [!question] 9608 | Describe what is meant by a digital signature [2]
> Describe what is meant by a **digital signature**.
>
>> [!success]- Answer — 3 points for 2 marks
>> - A mathematical algorithm // encrypted data
>> - Attached to an **electronically transmitted document**
>> - … to verify its content and that it comes from a trusted source
>>
>> *Latest: `9608_s21_qp_12_sc_8.b`*

> [!question] 9608 | When should a virus checker perform a check [2]
> Give **two** examples of when a virus checker should perform a check.
>
>> [!success]- Answer — 3 points for 2 marks
>> - Checks for **boot sector** viruses when the machine is first turned on
>> - When an external storage device is connected
>> - Checks a file or web page when it is accessed or downloaded
>>
>> *Latest: `9608_w15_qp_13_sc_10.b`*

> [!question] 9608 | Complete a table of security measure and description [3]
> Complete the table of security measures and descriptions.
>
>> [!success]- Answer — 3 entries for 3 marks
>> - **Disk mirroring** — data are written on two or more disks simultaneously
>> - Encryption — **contents are scrambled so they cannot be understood without a decryption key**
>> - **Backup** — a copy of the data is taken and stored in another location
>>
>> *Latest: `9608_s20_qp_11_sc_1.b`*

> [!question] 9608 | Identify the networking term from its description [4]
> Complete the table by identifying the most appropriate term for each description. Each term must be different.
>
>> [!success]- Answer — 4 rows for 4 marks
>> - Receives data packets from a network and forwards them onto a similar network → **Router**
>> - Manages access to a centralised resource → **Server**
>> - Joins networks that use different sets of rules to transmit data → **Gateway**
>> - **Monitors and controls incoming and outgoing network traffic based on set criteria** → **Firewall**
>>
>> *Latest: `9608_s21_qp_11_sc_9.b`. Links this topic to Chapter 2.*

> [!question] Inferred | Physical security measures [2]
> Give **two** physical security measures that protect a computer system, and state what each prevents.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Locked rooms / secure entry devices — prevent unauthorised people reaching the machines
>> - Swipe cards or keypads on server-room doors — restrict entry to authorised staff
>> - CCTV — deters and records unauthorised access
>> - Physically securing devices to desks — prevents theft of the hardware and the data on it
>>
>> *Accepted only as an alternative inside 9618 mark schemes; never the subject of a 9618 question. Tariff set to 2.*

> [!question] Inferred | Describe biometric authentication [2]
> Describe what is meant by biometric authentication and state why it is more secure than a password.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Uses a person's unique physical characteristics to identify them
>> - … for example a fingerprint, iris or retina scan, or voice recognition
>> - The characteristic cannot be guessed or shared, unlike a password
>> - The user must be physically present to gain access
>>
>> *"Biometric passwords" is accepted as a one-word answer but never described. Tariff set to 2.*

> [!question] SME | Symmetric and asymmetric encryption [2]
> State the difference between symmetric and asymmetric encryption.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Symmetric**: the same key is used to encrypt and decrypt
>> - … fast, but the key must be shared securely
>> - **Asymmetric**: a **public key** encrypts and a **private key** decrypts
>> - … more secure for sending data, as the private key is never shared
>> - **Caution:** neither term is in the 9618 syllabus for this topic or in any mark scheme here — encryption is always credited as "a key is needed to decode". The exception is `w22_qp_12_sc_6.a.i`, where the digital-signature answer uses the sender's private and public keys.
>>
>> *Tariff set to 2.*

> [!question] SME | Hardware and software firewalls [2]
> State the difference between a hardware firewall and a software firewall.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **hardware** firewall protects the whole network
>> - … and blocks unauthorised traffic entering the network
>> - A **software** firewall protects an individual device
>> - … monitoring the data going to and from that computer
>> - They are often used together for stronger security
>>
>> *Tariff set to 2. The 9618 mark schemes never split the two.*

---

## 6.1.4 Threats posed by networks and the internet

> [!question] 9618 | Describe two named threats to a computer system [4]
> Describe the following threats to a computer system: a **phishing email** and **spyware**. *(Max 2 marks each.)*
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Phishing**: the email pretends to be from an official body
>> - … persuading individuals to disclose private information // by example, such as bank details
>> - … or requesting authentication by redirecting to an unofficial website // inviting a user to click a link
>> - **Spyware**: malware downloaded **without the user's knowledge**
>> - … which secretly records the user's actions / keystrokes on the computer
>> - … and sends logs of the actions to a third party
>>
>> *Latest: `9618_w23_qp_12_sc_5.c`*

> [!question] 9618 | Identify a threat, describe it, and give a prevention method [3]
> Complete the table by identifying **one** threat to computer and data security posed by networks and the internet. Describe the threat and give a method of prevention. *(1 mark threat + 1 description + 1 prevention.)*
>
>> [!success]- Answer — 5 options for 3 marks
>> - **Malware / Virus** — malicious code that can alter or delete files → anti-virus // anti-malware // firewall
>> - **Spyware** — records keystrokes which are sent to a third party → anti-spyware // firewall // anti-malware
>> - **Hacking** — gaining **unauthorised** access to a computer network or device → authentication // firewall
>> - **Phishing** — **emails** supposedly from reputable companies are sent to trick people into revealing personal information → spam filter // do not open emails from unknown sources
>> - **Pharming** — users are directed to a bogus **website** that looks legitimate to obtain personal information → VPN // anti-malware // do not open links or download attachments
>>
>> *Latest: `9618_w25_qp_12_sc_5.e`*

> [!question] 9618 | Explain what is meant by a virus and by pharming [2]
> Explain what is meant by a **virus** and by **pharming**.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Virus: **malicious** program / software that replicates or copies itself
>> - … and deletes or alters files / data stored on a computer
>> - Pharming: malicious code / software installed on a computer
>> - … which redirects the user to a fake website to obtain personal data
>>
>> *Latest: `9618_w25_qp_11_sc_8.a`*

> [!question] 9618 | One difference and one similarity between pharming and phishing [2]
> State **one** difference and **one** similarity between pharming and phishing.
>
>> [!success]- Answer — 5 points for 2 marks
>> - Difference: pharming is malicious code that redirects to a **fake website**; phishing uses an **email** to prompt user action
>> - Difference: pharming is **automatic**; phishing requires **user action**
>> - Similarity: both try to obtain financial or personal information
>> - Similarity: both are a false representation of an official organisation, e.g. a bank
>> - Similarity: both make use of fake websites
>>
>> *Latest: `9618_w23_qp_13_sc_8.b`*

> [!question] 9618 | Two similarities and one difference between spyware and a virus [3]
> Give **two** similarities and **one** difference between spyware and a virus.
>
>> [!success]- Answer — 7 points for 3 marks
>> - Similarity: both are pieces of malicious software
>> - Similarity: both are downloaded / installed / run without the user's knowledge
>> - Similarity: both can pretend to be, or are embedded in, other legitimate software when downloaded // both try to avoid the firewall
>> - Similarity: both run in the background
>> - Difference: a virus can **damage** computer data; spyware only records or accesses data
>> - Difference: a virus does not send data out of the computer; spyware sends recorded data to a third party
>> - Difference: a virus **replicates itself**; spyware does not replicate itself
>>
>> *Latest: `9618_w21_qp_11_sc_2.c`*

> [!question] 9618 | Identify two threats posed by networks and the internet [2]
> Identify **two** threats to the data that are posed by networks and the internet.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Malware // viruses // spyware // by example
>> - Hacking
>> - Phishing
>> - Pharming
>>
>> *Latest: `9618_s21_qp_12_sc_8.c`*

> [!question] 9608 | Explain the term computer virus [2]
> Explain the term **computer virus**.
>
>> [!success]- Answer — 5 points for 2 marks
>> - Malicious code / software / program
>> - **That replicates / copies itself**
>> - Can cause loss of data / corruption of data on the computer
>> - Can cause the computer to "crash" / run slowly
>> - **Can fill up the hard disk with data**
>>
>> *Latest: `9608_w15_qp_13_sc_10.a`. Self-replication is the defining feature and appears in **no 9618 mark scheme** for a virus description.*

> [!question] Inferred | Why the internet increases the risk to a stand-alone PC [3]
> Explain why connecting a stand-alone computer to the internet increases the risk to its data.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The computer becomes reachable by anyone on the internet, so hackers can attempt to access it
>> - Malware can arrive through downloads, email attachments and web pages
>> - Data transmitted over the internet can be **intercepted** in transit
>> - Users can be targeted by phishing emails and pharming redirects
>> - Malware on one networked machine can spread to the others
>>
>> *Every question so far names a threat and asks for a description; the bullet's actual wording is untested. Tariff set to 3.*

> [!question] SME | How hackers gain access, and the effects [4]
> Describe **two** ways a hacker exploits a system, and **two** effects of a successful attack.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Unpatched software** — missing security updates leave known vulnerabilities open
>> - **Out-of-date anti-malware** — older protection fails to detect newer threats
>> - **Weak or reused passwords** — easy to guess or crack
>> - Effect: **data breach** — personal or company information is leaked or stolen
>> - Effect: further **malware installation**, data loss through deleted or corrupted files
>> - Effect: **identity theft** or financial loss (bank access, ransom demands)
>>
>> *Tariff set to 4. This is the "why" behind the credited prevention points.*

> [!question] SME | Phishing as social engineering, and its prevention [3]
> Explain what is meant by phishing and describe **two** methods of preventing it.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Phishing is a form of **social engineering**: fraudulent, legitimate-looking emails sent to a large number of addresses, claiming to be from a reputable company
>> - … usually coaxing the user to click a login button and enter their details
>> - Prevention: **anti-spam filters**, so fraudulent emails do not arrive in the inbox
>> - Prevention: **training staff** to recognise fraudulent emails and not open attachments from unrecognised senders
>> - Prevention: **user access levels** that stop staff opening executable (.exe) or batch (.bat) files
>>
>> *Tariff set to 3. The staff-training and file-type points are not in any mark scheme here.*

> [!question] SME | How pharming works technically [2]
> Explain how a pharming attack redirects a user, and give **one** way of preventing it.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The attacker alters the **DNS settings** or the user's **browser settings**
>> - … so that typing a legitimate address redirects to a fraudulent site
>> - Prevention: keep anti-malware up to date
>> - Prevention: check the URL carefully and look for the padlock icon
>>
>> *Tariff set to 2. The DNS mechanism is absent from the 9618 mark scheme and links this topic to Chapter 2.*

---

## 6.1.5 Methods that restrict the risks posed by threats

> [!question] 9618 | Explain how the data security risks of malware can be restricted [3]
> Explain how the data security risks of malware can be restricted.
>
>> [!success]- Answer — 6 pairs for 3 marks (point + expansion)
>> - Download programs from reputable websites / sources … as these are less likely to contain malware
>> - Backup / archive computer systems … so they can be restored in case of data loss from malware installation
>> - **Install and run** an anti-malware program … so regular scans can be made for known malware, anything found is quarantined or removed, and definitions are regularly updated
>> - Use a firewall to block unused ports … so that malware cannot enter the computer system
>> - **Deny administrator privileges to everyday users** … so that malware cannot be downloaded by them
>> - **Avoid the use of / access to removable devices** … so that malware cannot be installed from these devices
>>
>> *Latest: `9618_w23_qp_13_sc_8.c`*

> [!question] 9618 | Identify and describe one method of restricting interception during transfer [3]
> Identify **and** describe **one** method of restricting the risks posed by an unauthorised person intercepting data whilst it is being transferred across the internet. *(1 mark method + max 2 description.)*
>
>> [!success]- Answer — 4 points for 3 marks
>> - Method: **Encryption**
>> - Data is encoded / scrambled using a key to create **cipher text**
>> - If intercepted it cannot be **understood**
>> - … without being decrypted using a key
>>
>> *Latest: `9618_s25_qp_11_sc_7.a`*

> [!question] Inferred | Two-factor authentication [2]
> Describe what is meant by two-factor authentication.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The user must provide two separate pieces of evidence to log in
>> - Something they **know** (a password) plus something they **have** (a device or token)
>> - For example, a one-time code sent to the user's phone or generated by an app
>> - So a stolen password alone is not enough to gain access
>>
>> *Accepted as a one-word answer in `s21_qp_12_sc_8.b` but never described. Tariff set to 2.*

> [!question] Inferred | Restricting risk through user behaviour and policy [3]
> Other than installing software, describe **three** ways a company can reduce the risk posed by threats.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Train staff to recognise phishing emails and suspicious links
>> - Set an acceptable-use policy covering downloads and removable media
>> - Deny administrator privileges to everyday users
>> - Enforce strong password rules and regular password changes
>> - Restrict access rights so each user only reaches the data they need
>>
>> *`w23_qp_13_sc_8.c` is the only behavioural 9618 question of its kind. Tariff set to 3.*

---

## 6.1.6 Security methods that protect the security of data

> [!question] 9618 | Identify a method of keeping files secure during transmission and on the computer [4]
> Complete the table by identifying **one** method of keeping files secure during electronic data transmission **and one** method of keeping them secure on the computer. State how each method protects the data. *(1 mark method + 1 matching description, ×2.)*
>
>> [!success]- Answer — 8 points for 4 marks
>> - **During transmission — Encryption** // by example such as a **VPN**
>> - … jumble / encode the data so it cannot be decrypted or understood without the key
>> - **On computer — Firewall / proxy**
>> - … filter incoming transmissions and stop any that could be attempting unauthorised access
>> - **On computer — Anti-malware**
>> - … find and delete or quarantine any malware that could delete the data / files
>> - **On computer — Encryption** … jumble / encode data so it cannot be understood without the key
>> - **On computer — Physical method** … e.g. the computer storing the data cannot be accessed without the key to the room
>>
>> *Latest: `9618_s25_qp_13_sc_3.b`*

> [!question] 9618 | Two methods a DBMS can use to protect data from unauthorised access [4]
> Identify **two** methods a DBMS can use to protect the data in a table from unauthorised access. Explain how each method protects the data. *(1 mark method + 1 matching explanation, ×2.)*
>
>> [!success]- Answer — 8 points for 4 marks
>> - **Access rights** … appropriate permissions for the table are needed to read or edit the data
>> - **A password** for the database or for the table … prevents users without the password from accessing the data
>> - **Encrypting the database** … stops users without the decryption key from decoding / understanding the data
>> - **Views** … users can be given a view of the database that does not include the data in the protected table
>>
>> *Latest: `9618_s25_qp_12_sc_5.c.i`*

> [!question] 9618 | Identify a security method to protect program code during email transfer [3]
> Identify **one** security method that can protect program code from unauthorised access during email transfer, and explain how it protects the code. *(1 mark method + 2 explanation.)*
>
>> [!success]- Answer — 4 points for 3 marks
>> - Method: **Encryption**
>> - File contents are converted to **cipher text**
>> - If intercepted, the data cannot be understood
>> - … without the decryption key
>>
>> *Latest: `9618_w24_qp_12_sc_4.c`; `9618_s24_qp_12_sc_3.a.ii` is the identical 3-marker for data in transmission.*

> [!question] 9618 | Explain how encryption protects data during transmission [2]
> Explain how encryption can protect the security of data during transmission.
>
>> [!success]- Answer — 3 points for 2 marks
>> - Encodes / scrambles the data
>> - … so if it is intercepted it cannot be **understood**
>> - An algorithm / **key** is required to decode the data
>>
>> *Latest: `9618_s24_qp_13_sc_7.f.ii`*

> [!question] 9618 | Describe how access rights protect data from unauthorised access [3]
> Describe the ways in which access rights can be used to protect the data in a database from unauthorised access.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Access rights give different users access to different elements
>> - … by having different accounts / logins
>> - … which have different access rights, e.g. **read-only // no access // read/write**
>> - Specific **views** can be assigned to different users
>> - … e.g. managers can only see the data for their own shop(s)
>>
>> *Latest: `9618_w21_qp_11_sc_5.b`*

> [!question] 9608 | Describe three security measures a bank could implement [6]
> Describe **three** security measures that a bank could implement to protect its electronic data. *(3 pairs: measure + description.)*
>
>> [!success]- Answer — 7 pairs for 6 marks
>> - Installing a **firewall** and ensuring **it is switched on** … to stop unauthorised access / hackers gaining access to the bank's network
>> - Use **authentication** methods such as passwords and usernames … passwords should be strong, or use biometrics
>> - **Encrypt** the data … so that if data is accessed it will be meaningless, only readable by those with the decryption key
>> - Set up **access rights** … to stop users reading or editing data they are not permitted to access
>> - Install and run an up-to-date **anti-malware** program … to detect, remove or quarantine viruses and key-loggers
>> - Make **regular backups** of the data … to a separate device or off site, to enable recovery if necessary
>> - Employ measures for **physical security** … with an example of such a measure
>>
>> *Latest: `9608_s16_qp_13_sc_7.b`*

> [!question] 9608 | Explain how encrypting source code stored on a laptop keeps it secure [3]
> Explain how encrypting the source code can keep it secure on a laptop.
>
>> [!success]- Answer — 4 points for 3 marks
>> - Encryption scrambles the source code so it is meaningless
>> - … using an encryption key / algorithm
>> - If the file is accessed without authorisation it will be meaningless
>> - It requires a decryption key / algorithm to unscramble
>>
>> *Latest: `9608_s20_qp_13_sc_5.a`. 9618 only ever asks about encryption **in transit**, never a stored file on a stand-alone machine.*

> [!question] 9608 | Three ways to ensure users' details are kept secure [3]
> Give **three** ways that a developer can ensure users' details stored in a database on his computer are kept secure.
>
>> [!success]- Answer — 7 points for 3 marks
>> - Firewall / proxy
>> - Encryption
>> - Username and password
>> - Physical security
>> - Biometric authentication // by example
>> - Two-step authentication // by example
>> - Anti-malware
>>
>> *Latest: `9608_w18_qp_13_sc_5.b`*

> [!question] Inferred | Backup as a data-security method [3]
> Explain how regular backups protect the security of a company's data.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A copy of the data is taken and stored in a separate location / off site
>> - If the original data is lost or corrupted, the backup can be used to restore it
>> - This protects against accidental deletion, hardware failure and malware such as ransomware
>> - Backups should be taken regularly, so little data is lost between them
>> - The backup itself should be encrypted or physically secured, so it is not a new weakness
>>
>> *Backup appears only as a mark point inside `w23_qp_13_sc_8.c`; it has never been the subject of a 9618 question. Tariff set to 3.*

> [!question] SME | Access rights described properly [3]
> Describe how access rights are assigned and state the three levels of access.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Access rights control what users can see or do on a network
>> - They are assigned based on a user's **role, responsibilities or security clearance**
>> - **Full access** — the user can open, create, edit and delete files or folders
>> - **Read-only** — the user can open and view files but cannot edit or delete them
>> - **No access** — the user cannot see or interact with the file or folder at all
>> - Users can be **grouped** (e.g. "Year 11", "Staff", "Admin") and given rights as a group
>>
>> *Tariff set to 3 to match `9618_w21_qp_11_sc_5.b`. The grouping point is the one the mark schemes do not make.*

> [!question] SME | How wireless data is encrypted — the master key [4]
> Explain how data transmitted on a wireless network is encrypted.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The network's **SSID** (Service Set Identifier) plus a password is used to create a **master key**
>> - Devices connecting with the SSID and password are given a copy of the master key
>> - The master key is used to encrypt the data into **cipher text** before it is transmitted
>> - The receiver uses the same master key to decrypt the cipher text back into **plain text**
>> - The master key is **never transmitted**, so any intercepted data is useless without it
>> - Wireless networks use dedicated protocols such as **WPA2**; on a wired network encryption is often left to individual applications, e.g. **HTTPS**
>>
>> *Tariff set to 4 — this is the fullest version of the credited "a key is required to decode" point, and links to wireless networks in Chapter 2.*

---

# 6.2 Data Integrity

## 6.2.1 How validation and verification protect the integrity of data

> [!question] 9618 | Describe one other method of protecting the integrity of data [2]
> Data verification is one method of protecting the integrity of data. Describe **one other** method.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Validation** // a validation method named or described
>> - … protects the data by ensuring that the data is reasonable / sensible
>> - … and within specified bounds
>> - e.g. a range check, format check or presence check applied on entry
>>
>> *Latest: `9618_w23_qp_13_sc_8.a`*

> [!question] 9618 | State the difference between data verification and data validation [1]
> State the difference between **data verification** and **data validation**.
>
>> [!success]- Answer — 3 points for 1 mark
>> - Data verification is checking if input data is the **same as the original**
>> - … whereas data validation is checking that the data is **reasonable / sensible**
>> - Both halves are needed for the mark
>>
>> *Latest: `9618_w22_qp_12_sc_4.a`*

> [!question] 9618 | Describe how data validation protects integrity, with an example [2]
> Describe how data validation helps to protect the integrity of the data. Give an example in your answer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Validation checks that the data is reasonable / sensible
>> - Example: checking the data is the right number of characters
>> - Example: checking the data is the right type of characters
>> - It stops unreasonable data being stored, so the data remains accurate
>>
>> *Latest: `9618_w21_qp_11_sc_2.b.i`*

> [!question] 9618 | Describe how data verification protects integrity, with an example [2]
> Describe how data verification helps to protect the integrity of the data. Give an example in your answer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Verification checks that the data is the **same as the original**
>> - Example: double entry
>> - Example: a visual check against the source document
>> - It stops mis-keyed data being stored, so the data matches the original
>>
>> *Latest: `9618_w21_qp_11_sc_2.b.ii`*

> [!question] 9618 | Why data might still be incorrect after validation and verification [1]
> State why a car registration number might be incorrect even after it has been validated and verified.
>
>> [!success]- Answer — 2 points for 1 mark
>> - The registration number on the **original document** might be in the correct format but may be the **incorrect registration number** for that car
>> - Neither check can tell whether the source data itself is right
>>
>> *Latest: `9618_s23_qp_13_sc_4.d.iii`*

> [!question] 9608 | Why "validation makes sure data is the same as the original" is wrong [2]
> An employee states: *"Data validation is used to make sure that data keyed in are the same as the original data supplied."* Explain why this answer is incorrect.
>
>> [!success]- Answer — 3 points for 2 marks
>> - This is an explanation of data **verification**, not validation
>> - Data validation ensures that data is reasonable / sensible / within a given criteria
>> - Original data may have been entered correctly but still not be reasonable (e.g. an age of 210)
>>
>> *Latest: `9608_w16_qp_13_sc_7.c.ii`*

> [!question] 9608 | Complete two sentences about validation and verification [4]
> Complete these two sentences about data validation and verification.
>
>> [!success]- Answer — 4 gaps for 4 marks
>> - **Validation** checks that the data entered is reasonable.
>> - One example is a **presence check**.
>> - **Verification** checks that the data entered is the same as the original.
>> - One example is **double entry**.
>>
>> *Latest: `9608_s20_qp_11_sc_1.a`*

> [!question] 9608 | Ways of maintaining data integrity at the input stage [3]
> State **two** ways of maintaining data integrity at the **input stage**. Use examples to help explain your answer. *(1 mark per way + 1 mark for an example.)*
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Validation** — to ensure the data is reasonable
>> - … examples include range checks, type checks, length checks
>> - **Verification** — checks if data input matches the original
>> - … can use double data entry, or a visual check
>> - Note: verification does not check whether or not the data is reasonable
>>
>> *Latest: `9608_s15_qp_13_sc_3.c.i`*

> [!question] 9608 | Ways of maintaining data integrity during transmission [3]
> State **two** ways of maintaining data integrity **during data transmission**. Use examples to help explain your answer.
>
>> [!success]- Answer — 6 points for 3 marks
>> - **Parity checking** — one of the bits is reserved as a parity bit
>> - … e.g. 1 0 1 1 0 1 1 0 uses odd parity, so the number of 1s must be odd
>> - … parity is checked at the receiver's end, and a change in parity indicates data corruption
>> - **Checksum** — adds up the bytes in the data being sent and sends the checksum with the data
>> - … the calculation is re-done at the receiver's end
>> - … if it is not the same sum, the data has been corrupted during transmission
>>
>> *Latest: `9608_s15_qp_13_sc_3.c.ii`*

> [!question] 9608 | Describe what is meant by verification [2]
> Describe what is meant by **verification**.
>
>> [!success]- Answer — 6 points for 2 marks
>> - Checking that the data entered matches / is consistent with that of the source
>> - Comparison of two versions of the data
>> - Examples include double entry, visual checking, **proof reading**
>> - In the event of a mismatch, the user is forced to re-enter the data
>> - By example, e.g. creation of a password (entered twice)
>> - It does **not** check that data is sensible / acceptable
>>
>> *Latest: `9608_w17_qp_12_sc_3.c`*

> [!question] 9608 | Give a brief description of validation and verification [2]
> Give a brief description of each of the terms **validation** and **verification**.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Validation: check whether data is reasonable / meets given criteria
>> - Verification: a method to ensure data which is copied or transferred is the same as the original
>> - Verification: entering data twice and the computer checks both sets of data
>> - Verification: check entered data against the original document / source
>>
>> *Latest: `9608_w15_qp_13_sc_9.a`*

> [!question] Inferred | Why both validation and verification are needed [3]
> Explain why a system uses both data validation and data verification.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Validation checks the data is reasonable, but cannot tell whether it matches the original
>> - … so a value that is sensible but mis-keyed would still be accepted
>> - Verification checks the data matches the original, but cannot tell whether it is reasonable
>> - … so an unreasonable value copied correctly would still be accepted
>> - Using both catches more errors, so the stored data is more likely to be accurate
>>
>> *Every question tests one, the other, or the difference. `s23_qp_13_sc_4.d.iii` is the closest Cambridge has come. Tariff set to 3.*

> [!question] SME | More than one validation check on one field [2]
> Explain why a single field may have more than one validation check, using an example.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Each check tests only one property of the data, so one alone is not enough
>> - For example, a password field could have a **length** check
>> - … a **presence** check
>> - … and a **type** check, all applied to the same field
>>
>> *Tariff set to 2. Explains why 9618 routinely asks for "two other ways" of validating one field.*

---

## 6.2.2 Methods of data validation

> [!question] 9618 | Identify the validation method performed by each algorithm [3]
> The table contains three algorithms that perform data validation. Identify the method of data validation for each. Each method must be different.
>
>> [!success]- Answer — 3 rows for 3 marks
>> - `IF x < 1 OR x > 26 THEN OUTPUT "Invalid"` → **Range check**
>> - `IF x <> 'R' AND x <> 'G' AND x <> 'B' THEN OUTPUT "Invalid"` → **Existence check**
>> - A loop using `MID` and `LENGTH` searching for `"@"` → **Format check**
>>
>> *Latest: `9618_w25_qp_13_sc_7.e`. `9618_s21_qp_11_sc_6` is the 1-mark-each version: `x < 0 OR x > 10` → **Range**; `x = ""` → **Presence**; `NOT(x = "Red" OR x = "Yellow" OR x = "Blue")` → **Existence**.*

> [!question] 9618 | Describe two ways a car registration number can be validated [2]
> The car registration must be 1 letter, then 3 numbers, then 2 letters. A presence check is already used. Describe **two other** ways it can be validated.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Length check**: the registration number must be **6 characters** long
>> - **Format check**: the registration must be in the format **letter-digit-digit-digit-letter-letter**
>> - **Type check**: the registration number must be **alphanumeric**
>> - Note: the description must be specific to the field, not generic
>>
>> *Latest: `9618_s23_qp_13_sc_4.d.i`*

> [!question] 9618 | Describe two methods of validating a field with a fixed set of values [2]
> The field `RiderLevel` can only have the values Beginner, Intermediate or Advanced. Describe **two** methods of validating it.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Presence check** to make sure that the rider level is entered
>> - **Look-up / existence check** to make sure the rider level is only Beginner, Intermediate or Advanced
>> - **Length check** to make sure the rider level entered is either 8 or 12 characters
>> - **Type check** to make sure the rider level is alphanumeric
>>
>> *Latest: `9618_s23_qp_12_sc_2.c.i`*

> [!question] 9618 | Describe two validation methods for non-numeric data [2]
> A presence check is one validation method. Describe **two other** validation methods that can be used to validate **non-numeric** data.
>
>> [!success]- Answer — 4 points for 2 marks
>> - To make sure data is in the required format // only expected characters allowed
>> - To make sure the data is already present in the system
>> - To make sure the data contains the correct number of characters
>> - To ensure that non-numeric data is entered
>>
>> *Latest: `9618_w22_qp_12_sc_4.c`*

> [!question] 9608 | **Calculate a modulus-11 check digit** [4]
> A Patient ID is a seven-digit number. The DBMS adds a modulus-11 check digit as an eighth digit, using the weightings 6, 5, 4, 3, 2 and 1, with 6 as the multiplier for the most significant digit. Show the calculation of the check digit for the ID beginning 786531.
>
>> [!success]- Answer — 4 marks: 6 products, 2 division steps, the subtraction, the final answer
>> - 7 × 6 = 42 · 8 × 5 = 40 · 6 × 4 = 24 · 5 × 3 = 15 · 3 × 2 = 6 · 1 × 1 = 1 → **1 mark for the six values**
>> - Total = **128**
>> - 128 ÷ 11 = 11 remainder **7** // accept 128 MOD 11 = 7 → **1 mark for the two steps**
>> - Check digit = 11 − 7 = **4** → **1 mark for the subtraction**
>> - Complete Patient ID = **786531 4** → **1 mark for the answer**
>>
>> *Latest: `9608_w17_qp_13_sc_3.b.i`. **Check digit is named in the 9618 syllabus notes and has never been examined in the 9618 series in any form.***

> [!question] 9608 | Name and describe two validation checks on a primary key [4]
> Name **and** describe **two** validation checks that a DBMS could carry out on each primary key value a user keys in for a PatientID. *(1 mark name + 1 mark description, max 2 checks.)*
>
>> [!success]- Answer — 4 pairs for 4 marks
>> - **Uniqueness check** — each PatientID must be unique
>> - **Length check** — each PatientID is exactly 7 characters
>> - **Format check / Type check** — all 7 characters must be **digits**
>> - **Presence check** — PatientID must be entered
>>
>> *Latest: `9608_w17_qp_13_sc_3.b.ii`. **Uniqueness check is not one of the seven named in the 9618 notes** — use it only where a key is involved.*

> [!question] 9608 | Write the validation type for each description [4]
> Write the validation type for each validation description in the table.
>
>> [!success]- Answer — 4 rows for 4 marks
>> - A name must be entered → **Presence check**
>> - Entered as dd/mm/yyyy → **Format check**
>> - A limit of 15 characters can be entered → **Length check**
>> - Only values between 1 and 5 can be entered → **Range check**
>>
>> *Latest: `9608_s21_qp_13_sc_1.a`*

> [!question] 9608 | Tick whether each measure is validation or verification [5]
> Put one tick in each row to indicate whether the measure is validation or verification.
>
>> [!success]- Answer — 5 rows for 5 marks
>> - Checksum → **Verification**
>> - Format check → **Validation**
>> - Range check → **Validation**
>> - Double entry → **Verification**
>> - **Check digit → Validation**
>> - *From `9608_s18_qp_13_sc_4.c`:* Type check → Validation; **Proof reading → Verification**
>>
>> *Latest: `9608_s18_qp_12_sc_3.c`*

> [!question] 9608 | Name and describe two validation checks for a data capture form [4]
> Name **and** describe **two other** types of validation check that could be appropriate for this data capture form. *(1 mark check + 1 mark description.)*
>
>> [!success]- Answer — 4 pairs for 4 marks
>> - **Range check** — check the number entered is between, say, 1 and 100
>> - **Format check** — checks the product code is a particular format // checks the number has digit characters only
>> - **Length check** — the number of items has exactly five characters
>> - **Existence check** — to ensure the product code has been assigned
>>
>> *Latest: `9608_s17_qp_13_sc_7.c.v`*

> [!question] Inferred | Limit check versus range check [2]
> Explain the difference between a **limit check** and a **range check**, giving an example of each.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **limit check** bounds one end only — it checks a value does not exceed a maximum (or fall below a minimum)
>> - … e.g. no more than 5 items can be bought in a special offer
>> - A **range check** bounds **both** ends — it checks a value falls within a set range
>> - … e.g. a percentage must be between 0 and 100
>>
>> *Both are named in the syllabus notes; **no 9618 question has ever distinguished them**. Tariff set to 2.*

> [!question] Inferred | Write a validation check as pseudocode [3]
> Write pseudocode to perform a length check that ensures an input `x` is exactly 8 characters long, outputting "Invalid" otherwise.
>
>> [!success]- Answer — 3 points for 3 marks
>> - `INPUT x`
>> - `IF LENGTH(x) <> 8 THEN`
>> - `   OUTPUT "Invalid"` … `ENDIF`
>> - *Also accept a presence check:* `IF x = "" THEN OUTPUT "Invalid" ENDIF`
>> - *Also accept a range check:* `IF x < lower OR x > upper THEN OUTPUT "Invalid" ENDIF`
>>
>> *The syllabus says "describe **and use** methods of data validation", but both series only ask you to **read** the algorithm. Tariff set to 3 to match `w25_qp_13_sc_7.e`.*

> [!question] SME | The seven validation checks with examples [4]
> Name and give an example of each of the validation checks in the syllabus.
>
>> [!success]- Answer — 7 points for 4 marks
>> - **Range** — a number falls within a set range, e.g. a percentage between 0 and 100
>> - **Limit** — a value does not exceed a maximum, e.g. no more than 5 items in an offer
>> - **Length** — the length of a string, e.g. a PIN is exactly 4 digits
>> - **Presence** — data has been entered and the field is not blank
>> - **Existence** — a referenced value exists in a database or list, e.g. a student ID that exists in the school records
>> - **Format** — data matches a pattern, e.g. an email address contains '@' and a domain like '.com'
>> - **Check digit** — the final digit of a code, calculated from the others, used to detect entry errors
>> - *(Type check — the input is of the correct data type — is credited by 9618 but is not one of the seven named in the notes.)*
>>
>> *Tariff set to 4.*

> [!question] SME | What a check digit catches, and where it is used [3]
> State what a check digit is, what kinds of error it detects, and give **two** contexts where it is used.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The last digit included in a code or sequence, calculated from the other digits by a standardised algorithm
>> - Detects **incorrect digits entered**
>> - Detects **omitted or extra digits**, and **phonetic errors**
>> - Used in **ISBN** book numbers — the final digit makes the weighted total divide exactly, with no remainder, so the ISBN is valid
>> - Used in **barcodes** — the final digit validates and authenticates the scanned item
>>
>> *Tariff set to 3. This is the framing behind the 9608 modulus-11 calculation above.*

---

## 6.2.3 Methods of data verification during data entry and data transfer

> [!question] 9618 | Complete the description of parity check [5]
> Complete the description of parity check when Computer A transmits data to Computer B.
>
>> [!success]- Answer — 5 gaps for 5 marks
>> - Computer A and Computer B agree on whether to use **odd or even** parity.
>> - Computer A divides the data into groups of **7 bits**.
>> - If the agreed parity is **odd** and the group has an even number of 1s, a parity bit of 1 is appended, otherwise a parity bit of 0 is appended.
>> - In a parity **block** check the bytes are grouped together, for example in a grid, and a bit is assigned to each column to make the column match the parity.
>> - These parity bits are transmitted with the data as a parity **byte**.
>>
>> *Latest: `9618_s24_qp_11_sc_5.b`*

> [!question] 9618 | Identify and describe two methods of verification during data transfer [4]
> Complete the table by identifying **and** describing **two** methods of data verification that can be used during data transfer. *(1 mark method + 1 matching description, ×2.)*
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Parity byte** — an additional bit is added to make the number of 1s in the byte odd or even to match the parity; if a byte with an odd number of 1 bits is received when even parity is used, there is an error
>> - **Parity block** — parity is calculated horizontally and vertically; a parity byte is created from the bits produced by the vertical parity check and sent with the data; the parity is re-checked on receipt and the position of an incorrect bit can be determined
>> - **Checksum** — a calculation is made from the data and the result is transmitted with the data; the receiver repeats the calculation and compares the result with the value received; if the two differ, there is an error
>> - Parity byte: each byte can be checked on receipt and a request sent to resend if it does not match parity
>> - Parity block: the location of an error can be found using vertical and horizontal parity
>> - Checksum: if both checksums match, the data is verified
>>
>> *Latest: `9618_s24_qp_13_sc_7.f.i`; `9618_w25_qp_13_sc_7.c` is the 3-mark single-method version.*

> [!question] 9618 | Explain how data verification is used when an identifier is entered [4]
> An example of a tutor ID is NK16C6. Explain how data verification can be used when the tutor ID is entered into the TUTOR table.
>
>> [!success]- Answer — 4 points for 4 marks (2 pairs)
>> - The administrator completes a **visual check** / checks by eye …
>> - … that the tutor identifier input matches the tutor identifier on the **original document**
>> - **Double entry check** // the administrator (or a second person) enters the number a second time …
>> - … and the **system** compares it with the first entry
>>
>> *Latest: `9618_w23_qp_13_sc_3.c`. Note who compares: the **person** for a visual check, the **system** for double entry.*

> [!question] 9618 | Explain how data can be verified using a checksum [3]
> Explain how data can be verified using a checksum.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The data is put through an algorithm to create a **checksum value**
>> - The data and the checksum are sent to the receiver
>> - The receiver performs the **same algorithm** on the received data
>> - If both checksums match, the data is verified
>> - If they do not match, an error has occurred
>>
>> *Latest: `9618_s25_qp_11_sc_7.c`; `9618_w22_qp_12_sc_4.b` is the identical 3-marker.*

> [!question] 9618 | Match each verification method to transfer or entry [2]
> Draw one line from each verification method to indicate whether it is used during data transfer or data entry.
>
>> [!success]- Answer — 4 lines for 2 marks (1 mark for 2–3 correct, 2 marks for all 4)
>> - Parity byte check → **Data transfer**
>> - Checksum → **Data transfer**
>> - **Visual check → Data entry**
>> - Parity block check → **Data transfer**
>>
>> *Latest: `9618_w25_qp_12_sc_1`*

> [!question] 9618 | Describe two ways data can be verified on entry [2]
> Describe **two** ways that a car registration number can be verified when it is entered into the database.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Visual check**: **manually** compare the registration number entered with the source document
>> - **Double entry**: enter the registration number twice and **the computer compares** to check they are the same
>> - Visual check: a prompt asks the user to confirm the data is correct before proceeding
>> - Double entry: an error message is shown if the two entries differ
>>
>> *Latest: `9618_s23_qp_13_sc_4.d.ii`*

> [!question] 9618 | Complete the missing parity bit [1]
> A computer system uses even parity, with the least significant (rightmost) bit as the parity bit. Complete the byte `0 1 0 1 1 1 0 _`.
>
>> [!success]- Answer — 1 mark
>> - The parity bit is **0**
>> - Method: count the 1s in the first seven positions (0,1,0,1,1,1,0 → four 1s). Four is already even, so the parity bit must be 0 to keep the byte even.
>>
>> *Latest: `9618_w25_qp_12_sc_6.c.i`*

> [!question] 9618 | Circle the altered bit in a parity block [1]
> A parity block uses even parity. One of the four data bytes has an error in one bit. Circle the bit that has been altered during transfer.
>
>> [!success]- Answer — 1 mark
>> - Check the parity of each **row** and identify the row whose parity is wrong
>> - Check the parity of each **column** against the parity byte and identify the column whose parity is wrong
>> - The **intersection** of that row and that column is the altered bit
>>
>> *Latest: `9618_w25_qp_12_sc_6.c.ii`*

> [!question] 9608 | Describe how a parity block check identifies a corrupted bit [4]
> Describe how a parity block check can identify a bit that has been corrupted during transmission.
>
>> [!success]- Answer — 5 points for 4 marks
>> - Each byte has a parity bit // horizontal parity
>> - An additional **parity byte** is sent with vertical (and horizontal) parity
>> - Each row and column must have an even / odd number of 1s
>> - Identify the incorrect **row** and the incorrect **column**
>> - The **intersection** is the error
>>
>> *Latest: `9608_s19_qp_13_sc_2.c.i`. 9618 only ever asks you to **circle** the bit.*

> [!question] 9608 | When a parity block check cannot identify corrupted bits [2]
> Give a situation where a parity block check **cannot** identify corrupted bits.
>
>> [!success]- Answer — 3 points for 2 marks
>> - Errors in an **even number of bits** (in the same row or column)
>> - … they could cancel each other out, so the parity still appears correct
>> - This prevents the error being identified, and the data could appear to be correct
>>
>> *Latest: `9608_s18_qp_11_sc_6.c` (2 marks); `9608_s19_qp_13_sc_2.c.ii` is the 1-mark version. **The single most important limitation of parity, and never asked in 9618.***

> [!question] 9608 | Explain how you identified the error in a parity block [2]
> Explain how you identified the error.
>
>> [!success]- Answer — 3 points for 2 marks
>> - The row and the column each have incorrect parity (odd instead of even)
>> - The **intersection** of that row and column identifies the error
>> - Every other row and column has the correct parity
>>
>> *Latest: `9608_s18_qp_11_sc_6.b.ii`*

> [!question] 9608 | Identify two bits that must be changed, and explain the method [3]
> A data block is received containing errors. Identify and circle **two** bits which must be changed to remove the errors, and explain how you arrived at your answer.
>
>> [!success]- Answer — 4 points for 3 marks
>> - Consider each **row** in sequence
>> - Identify any row with incorrect parity
>> - Repeat the process for each **column** in sequence
>> - Identify where a row and a column with incorrect parity **intersect** — each intersection is an error
>>
>> *Latest: `9608_s17_qp_13_sc_5.b.ii`. 9618's version has exactly one error; the two-error variant is 9608-only.*

> [!question] 9608 | How the sender calculates the parity bit for each byte [2]
> Describe how the data logger calculates the parity bit for each of the bytes in the data block, using odd parity with bit position 0 as the parity bit.
>
>> [!success]- Answer — 2 points for 2 marks
>> - Count the number of 1 bits in the **first seven** bit positions
>> - Add a 0 or 1 to bit position 0, to make the count of 1 bits an **odd** number
>>
>> *Latest: `9608_s17_qp_13_sc_5.a.i`*

> [!question] 9608 | How the computer uses the parity byte as a further check [2]
> Describe how the computer uses the parity byte to perform a further check on the received data bytes.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A parity bit is worked out for each **column**
>> - The computer checks the parity of each bit position in the parity byte // generates a copy of the parity byte and **compares**
>> - If incorrect parity, there is an error in the data received // no parity error means no error in the data received
>> - The **position** of the incorrect bit can be determined
>>
>> *Latest: `9608_s17_qp_13_sc_5.a.iii`*

> [!question] 9608 | Explain what is meant by a parity check, with an example [4]
> Explain what is meant by a parity check. Give an example to illustrate your answer.
>
>> [!success]- Answer — 7 points for 4 marks
>> - Parity can be **even or odd**
>> - A parity check uses the **number of 1s** in a binary pattern
>> - If there is an even / odd number of 1s, then the parity is even / odd
>> - Following transmission …
>> - … the parity of each byte is re-checked
>> - A **parity bit** is used to make sure the binary pattern has the correct parity
>> - Example: `1 0 0 1 0 1 1 1` has the parity bit set to 1 in the MSB, since the system uses odd parity (original data `0 0 1 0 1 1 1` has four 1 bits)
>>
>> *Latest: `9608_w15_qp_13_sc_9.b`*

> [!question] 9608 | Name and describe one other verification method during transfer [3]
> Parity is not the only method to verify the data has been sent correctly. Name **and** describe **one other** method of data verification during data transfer. *(1 mark name + max 2 description.)*
>
>> [!success]- Answer — 6 points for 3 marks
>> - **Checksum** — a calculation is done on a block of data
>> - … the result is transmitted with the data, the calculation is repeated at the receiving end, and the results are compared; if different, an error has occurred
>> - **Hash total** — a total of several fields of data
>> - … **including fields not usually used in calculations**
>> - … the result is transmitted with the data, recalculated at the receiving end and compared
>> - … if different, an error has occurred
>>
>> *Latest: `9608_s18_qp_11_sc_6.d`. **Hash total is not in the 9618 syllabus notes** — treat as background.*

> [!question] 9608 | Describe one way of ensuring integrity during transmission [4]
> Describe **one** way of ensuring that the integrity of the data is retained during the transmission stage. *(1 mark for the name + 3 for the description.)*
>
>> [!success]- Answer — 6 points for 4 marks (parity route)
>> - **Parity check**
>> - Uses even or odd parity, which is decided before the data is sent
>> - Each byte has a parity bit
>> - The parity bit is set to 0 or 1 to make the parity for the byte correct
>> - After transmission, the parity of each byte is re-checked; if it is different, an error is flagged
>> - Any reference to the use of parity blocks / a parity byte to identify the position of the incorrect bit
>>
>> *Latest: `9608_s15_qp_12_sc_4.b`. The checksum route also scores: a calculation is carried out on the data; the result is sent with it; recalculated at the receiving end; if the sums differ the data has been corrupted; a **request is sent to re-send the data**.*

> [!question] Inferred | Why a single parity bit is not enough [2]
> Explain why a single parity bit cannot locate an error, but a parity block can.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A single parity bit shows only **that** the parity of that byte is wrong, not which bit is wrong
>> - Any one of the bits in that byte could have flipped
>> - A parity block adds a parity **byte** giving vertical parity as well as horizontal
>> - Cross-referencing the faulty row with the faulty column pinpoints the exact bit
>>
>> *`w25_qp_12_sc_6.c.ii` asks you to locate an error with a block, but never asks why a single bit could not do it. Tariff set to 2.*

> [!question] Inferred | What happens after an error is detected [2]
> State what happens after a verification method detects an error during data transfer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A request is sent to the sender to **retransmit** the data
>> - … the affected byte or block is sent again
>> - Where a parity block is used, the position of the bit is known, so the error can sometimes be corrected automatically
>> - The data is not accepted / used until it passes the check
>>
>> *Appears once as a mark point inside `w25_qp_13_sc_7.c`; never the subject of a question in either series. Tariff set to 2.*

> [!question] SME | Why bits get flipped, and parity's blind spot [3]
> Explain why transmission errors occur, and state **two** limitations of a parity check.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Bits can be flipped or changed due to **interference** on a wire, or wirelessly due to weather or other signals
>> - Parity checks are quick and easy to implement …
>> - … but fail to detect **bit swaps that leave the parity unchanged**
>> - … and show only **that** an error occurred, not **where**
>> - This is why parity blocks and parity bytes exist — cross-referencing horizontal and vertical parity pinpoints the faulty cell
>>
>> *Tariff set to 3. Links this topic to transmission media in Chapter 2.*

> [!question] SME | The two entry-verification methods, precisely [2]
> Describe double entry checking and a visual check.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Double entry**: the data is entered twice in separate input boxes and the two are compared
>> - … if they do not match, an error message is shown
>> - **Visual check**: the user reads the data on screen and a prompt asks whether it is correct before proceeding
>> - … if it is not, the user enters the data again
>>
>> *Tariff set to 2. Mark schemes are strict about **who** compares: the system for double entry, the person for a visual check.*
