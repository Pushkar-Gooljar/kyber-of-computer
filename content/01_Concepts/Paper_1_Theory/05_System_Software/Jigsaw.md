---
title: Jigsaw — 5 System Software (AS Level)
syllabus: 9618 (2026)
topics: 5.1 Operating Systems · 5.2 Language Translators
---

# Jigsaw — 5 System Software

Syllabus content for **9618 Topic 5**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers.

> [!danger] The IDE bullet is new in 9618
> The 9608 Legend has **no questions at all** under *Describe features found in a typical IDE*. Yet 9618 has examined it **eleven times** since 2021 — more than any other bullet in this chapter. It is 9618-only and heavily tested; treat 5.2.4 as a guaranteed topic, not an afterthought.

---

# 5.1 Operating Systems

## 5.1.1 Why a computer system requires an Operating System

> [!success] Describe the purpose of an OS in a computer [5]
> To provide a **user interface** … so that the user is able to communicate with the hardware · to **manage memory** … so that data can be stored and accessed, and multitasking is possible · to **manage files** … allowing the user to create, edit, update and delete files and folders · to manage **inputs and outputs** from hardware/peripherals · to **handle processes** … to make sure each process has fair access. `9618_s25_qp_11_sc_6.b`

> [!success] State one purpose of the Operating System [1]
> To **hide the complexities of the hardware** from the user · to provide a **platform for software to run** · to provide a user interface. `9618_w23_qp_12_sc_8.a`

> [!warning] Explain why a personal computer needs an Operating System [2]
> The **hardware cannot be used without it** // the computer would not function · it acts as an **interface between the user and the hardware** · it provides a **platform on which application software can run**. `9608_s17_qp_12_sc_4.a.i`

> [!warning] Complete the table identifying the type of software described [4]
> Given a description, name the software type: **operating system**, **utility program**, **application software**, **compiler / translator**. Tests the boundary between system software and application software. `9608_w19_qp_12_sc_1.a`

> [!info] Types of user interface
> "Provide a user interface" is credited in both questions, but **no 9618 question asks what kind of interface** — CLI, GUI, menu, natural language — or which suits which user. This is standard content elsewhere in the subject and sits directly under "why a computer requires an OS".

> [!info] What happens **without** an OS
> Both questions ask for the OS's purpose positively. The inverse — a machine with no OS would require every program to manage the hardware itself, with no multitasking, no file system and no common interface — has not been asked, in either series.

> [!abstract] The interface types, with examples
> **CLI** — text-based commands, used by advanced users (MS-DOS, Raspbian) · **GUI** — windows, icons, menus, pointers (WIMP), optimised for mouse and touch (Windows, Android, macOS) · **Menu** — successive menus with a single option at each stage (chip-and-PIN machines, vending machines, streaming services) · **Natural language (NLI)** — responds to spoken or textual input (Alexa, Siri, search engines).
> The one-line justification SME gives for the whole bullet is the cleanest available: *a user does not need to know where on secondary storage data is kept, just that it is saved for when they want it again.*

---

## 5.1.2 Key management tasks carried out by the Operating System

> [!success] Identify the key management tasks [4]
> Memory management · file management · security management · hardware / device / peripheral / resources management · input-output management · process management · **error checking and recovery** · provision of a platform for software · provision of a user interface. `9618_s21_qp_11_sc_2.b`; `9618_w25_qp_13_sc_8.d`; `9618_s23_qp_11_sc_3.b`

> [!success] Describe the process management tasks performed by an OS [5]
> Manages the **scheduling** of processes // decides which process is to be run next · manages which **resources** the processes require, such as allocating memory · enables processes to **share data** · **prevents interference** between processes // resolution of conflicts · handles the **process queue** · allows **multi-tasking / multi-processing** … by ensuring fair access, handling priorities **and** handling interrupts. `9618_s23_qp_12_sc_5.d.i`; `9618_w24_qp_12_sc_3.c`

> [!success] Describe the file management tasks carried out by an OS [4]
> Storage space is divided into **file allocation units** · space is allocated to particular files · maintains / creates **directory structures** · specifies the **logical method of file storage**, e.g. FAT or NTFS · provides **file naming conventions** · controls access // implements access rights // password protection // makes file sharing possible · specifies the tasks that can be performed on a file (open, close, delete, copy, create, move) · allows searching for a file. `9618_w21_qp_12_sc_7.b`; `9618_w24_qp_11_sc_4.a.i`

> [!success] Describe how the OS manages peripheral hardware devices [4]
> **Installs device drivers** … to allow communication between peripherals and computer · sends data to and receives data from peripherals … such as to an output device and from an input device · **handles buffers** for transfer of data … to ensure smooth transfer between devices that transmit and receive at different speeds · manages **interrupts / signals** from the device. `9618_s23_qp_11_sc_3.a`

> [!success] State two tasks performed by hardware management [2]
> Installs **driver** software for devices connected to external ports · manages communication between devices · manages **hardware interrupts**. `9618_w25_qp_11_sc_5.a.i`

> [!success] State two tasks performed by security management [2]
> Prevents unauthorised access … by providing **authentication** // by validating users and processes · implements **access rights and permissions** · makes provision for **recovery of lost data** · carries out OS **security updates** as available · carries out **auditing** and keeps logs of activity. `9618_w25_qp_11_sc_5.a.ii`

> [!success] Describe how memory management organises and allocates RAM [2]
> RAM is assigned into **blocks** · **dynamic allocation** of RAM to programs / processes · **reclaims unused blocks** of RAM · prevents two programs occupying the same area of RAM at the same time · moves data from secondary storage when needed // manages **paging, segmentation and virtual memory**. `9618_w22_qp_11_sc_7.b`

> [!success] Explain how memory management and process management support multi-tasking [4]
> **Memory management (max 3):** stores data from all currently running programs concurrently in RAM · stops the data from overwriting each other in RAM · decides which processes should be in main memory · makes efficient use of memory. **Process management (max 3):** allows one process to be paused whilst another is actioned · decides which process is to be run next · switches between processes to let them share the processor · identification/description of **scheduling**. `9618_s24_qp_12_sc_6`

> [!success] Match each OS management task to its description [4]
> Hardware management → installs programs for devices connected to external ports · security management → validates user and process authenticity · memory management → dynamically allocates memory to processes · process management → allows processes to transfer data to and from each other. *(Distractor: marks unallocated file storage for availability = file management.)* `9618_w22_qp_13_sc_3`

> [!warning] Describe the process management and user interface tasks of an OS [6]
> *Max 4 for each task.* **Process management** — scheduling / decides which process runs next · allocates resources to processes · handles interrupts · prevents processes interfering with each other · enables multi-tasking by giving each process a share of processor time. **User interface** — allows the user to communicate with the computer · hides the complexity of the hardware · allows the user to run software, and to manage files and folders. `9608_w19_qp_11_sc_2.b`

> [!warning] State three tasks carried out by **memory management** [3]
> Allocates memory to programs and data · keeps track of which memory is in use and which is free · **deallocates** memory when a process finishes · protects one program's memory from another · allocates **virtual memory**, using **paging** or **segmentation** · moves data between main memory and backing store. `9608_s20_qp_11_sc_8.a`; `9608_w21_qp_11_sc_7.a.i`

> [!warning] State two tasks carried out by **input/output device management** [2]
> Sends data to and receives data from peripherals · manages **device drivers** · manages **buffers and queues** for devices · handles **interrupts** raised by devices · **detects devices** as they are connected · keeps track of the **status** of each device · handles **power management** for devices. `9608_w21_qp_11_sc_7.a.ii`; `9608_s21_qp_13_sc_4.a.i`

> [!warning] State three tasks carried out by **error detection and recovery** [3]
> Deals with **interrupts** · deals with **run-time errors** · deals with **hardware faults** · produces **error diagnostic messages** for the user · **deadlock detection and recovery** · allows **safe-mode** boot-up · performs a controlled **system shutdown** · maintains and uses **restore points**. `9608_s21_qp_13_sc_4.a.ii`

> [!warning] Complete the table of Operating System management tasks [4]
> Match task to description across memory, file, device, security and **interrupt processing**. `9608_s19_qp_13_sc_1.a`

> [!warning] State three tasks carried out by **file management** [3]
> Creates, opens, reads, writes, closes and deletes files · organises files into **folders/directories** · maintains the **file directory structure** and keeps track of where each file is stored · manages **access rights** to files · moves, copies and renames files. `9608_s18_qp_12_sc_1.a.i`

> [!warning] Choose two management tasks and describe each [4]
> *Max 2 marks per task.* The 9608 format asks the candidate to **select** the tasks — so any two of memory, file, device, process, security must be describable to two marks each, not just nameable. `9608_w16_qp_12_sc_7`

> [!warning] Describe the sequence of events when a file is read from the hard disk [8]
> An 8-mark sequencing question: the application requests the file · the OS **file management** looks up the file in the directory · it finds the physical address (surface/track/sector) · **device management** issues the read to the disk controller via the **device driver** · the disk head is moved to the track, the sector is read into a **buffer** · an **interrupt** signals the transfer is complete · **memory management** allocates main memory for the data · the data is copied from the buffer into that memory and control returns to the application. The longest single question in the chapter in either series. `9608_w16_qp_12_sc_3`

> [!info] **Paging, segmentation and virtual memory**
> Credited once, as an alternative mark point in `w22_qp_11_sc_7.b`. Virtual memory also appears in the Chapter 4 RAM-performance mark scheme. But **no question in either series asks what virtual memory is or how paging works** — and virtual memory is the mechanism that connects memory management to system performance.

> [!info] **Error checking and recovery**
> Listed as a creditable answer in `s21_qp_11_sc_2.b` and `s23_qp_11_sc_3.b`, but never described. It is the only named management task with no descriptive question against it.

> [!info] Scheduling described rather than named
> "Manages the scheduling of processes" is a mark point in three separate questions; "identification/description of scheduling" is explicitly creditable in `s24_qp_12_sc_6`. Yet no question asks *how* scheduling works — time slices, priorities, the ready queue. Given the tariff on process management questions (4–5 marks), this is the natural place for a harder question.

> [!abstract] The five key tasks, as SME frames them
> **Memory management** — allocating main memory (RAM) between programs open at the same time; copying programs and data from secondary to primary storage as needed.
> **File management · Security management · Hardware management · Process management** — as in the mark schemes above.
> Note the 9618 mark schemes also credit **input/output management**, **error checking and recovery**, **provision of a platform for software** and **provision of a user interface** as "key management tasks", so the list is longer than SME's five.

---

## 5.1.3 The need for typical utility software

> [!success] Match each utility to its purpose [5]
> Virus checker → to scan for malicious program code · disk formatter → to initialise a disk · backup → to create copies of files in case the original is lost · disk repair → to check for and fix inconsistencies on a disk · defragmentation → to reorganise files so they are contiguous. *(Distractor: to decrease the file size = file compression.)* `9618_w22_qp_12_sc_1.a`

> [!success] Identify one utility not intended to improve security, and explain why it is needed [3]
> **Defragmentation** — over time saving and deleting small files fragments the disk; the software makes individual files **contiguous**; so access time is improved, because **head movement is reduced**. **Disk contents analysis / disk repair** — to identify and mark bad sectors; to restore corrupted files; to recover lost data. **File compression** — to reduce the size of files; saving storage and memory space; reducing transmission time. **Disk formatter** — to prepare a disk for use // set up the file system; to partition the disc; to delete all data from the disc. `9618_w23_qp_12_sc_8.b`

> [!success] Explain how defragmentation improves performance [3]
> Rearranges blocks of individual files (on the HDD) so they are **contiguous** // moves the free space together · accessing each file is faster · because there is **no need to search for the next fragment** of the file · so **less head movement** is needed. `9618_s23_qp_11_sc_3.c`

> [!success] Describe the reasons why a disk formatter is needed [3]
> The disk needs to be **prepared for initial use** · the disk needs to be **checked for errors** · a new **file system** needs to be generated on the disk · the **file allocation table** needs to be set up. `9618_w23_qp_13_sc_5.b.ii`

> [!success] Identify two utility programs that improve performance, and state how [4]
> **Defragmentation** — less time taken to access files because each one is contiguous, so less head movement · **Virus checker** — makes more RAM available for programs to run, because it removes software that might be taking up memory or replicating · **Disk repair / disk contents analysis** — prevents bad sectors being used because it identifies and marks them; reduces access times by optimising storage · **Disk / system clean up** — releases storage by removing unwanted or temporary files. `9618_w21_qp_12_sc_7.c`

> [!success] Explain the need for back-up software [2]
> To allow data to be **retrieved / restored** when lost · to **automatically** make a duplicate copy of data … so the user does not have to remember to back up · to make regular duplicate copies of data. `9618_w24_qp_11_sc_4.a.ii`

> [!success] Describe the purpose of utility software in a computer [2]
> To help users to **set up / configure / analyse / optimise / maintain** the computer · by for example making memory allocation more efficient · by for example checking the system for faults. `9618_s23_qp_12_sc_5.d.ii`

> [!success] Identify utilities that could recover corrupted image files [2]
> **Disk repair / disk contents analysis** · **back-up software**. `9618_w25_qp_12_sc_8.b.ii`

> [!warning] Identify and describe two utility programs [4]
> *Two marks per program: one for naming it, one for what it does.* Disk defragmenter · back-up · virus checker / anti-malware · disk formatter · disk repair · file compression · **system clean-up** · **firewall** · **encryption**. `9608_w21_qp_11_sc_7.b`; `9608_s21_qp_13_sc_4.b.ii`

> [!warning] Tick to show whether each program is a utility program [2]
> The distractors matter: a **translator**, an **IDE**, **graphics software** and a **spreadsheet** are **not** utility programs. `9608_s21_qp_13_sc_4.b.i`

> [!warning] Explain why a user would use back-up / a disk defragmenter / disk repair software [2 each]
> **Back-up** — a second copy exists if data is lost, corrupted or the hardware fails, so it can be restored. **Defragmenter** — files stored in scattered blocks are rearranged into contiguous blocks, so read/access time falls. **Disk repair** — scans the disk for bad sectors and corrupted files, marks bad sectors unusable and recovers what it can. `9608_s21_qp_12_sc_7.a.i`–`iii`

> [!warning] Explain how the disk formatter, contents analysis and repair software work together [3]
> The formatter organises the disk into **tracks and sectors** and builds the file system · the contents-analysis software **scans** the disk to identify used, free, bad and corrupted areas · the repair software then **fixes or marks** those areas so the disk remains usable. `9608_s20_qp_12_sc_2.c.i`

> [!warning] Describe the purpose of disk repair software [3]
> Checks the disk for **errors and bad sectors** · attempts to **recover data** from damaged areas · **marks bad sectors** so they are not used again · repairs the **file system / directory** so files can be found. `9608_w19_qp_12_sc_1.b`

> [!warning] Describe the purpose of a virus checker and of back-up software [4]
> *Max 3 for each.* **Virus checker** — scans files and memory for known virus **signatures** and for suspicious behaviour (**heuristics**) · quarantines or deletes infected files · must be kept **up to date** · can scan on demand or in real time. **Back-up** — makes a copy of files, on a schedule or on demand, to a separate medium or the cloud, so data can be restored after loss, corruption or hardware failure. `9608_w19_qp_11_sc_2.c`

> [!warning] Explain when a virus checker should run [2]
> Continuously **in the background / in real time** as files are opened or downloaded · on a **scheduled full scan** · whenever new external media is connected · immediately after the definitions are updated. `9608_w15_qp_13_sc_10.b`

> [!warning] Describe how utility software prevents accidental loss of data [2]
> Automatic, scheduled **back-ups** so a recent copy always exists · the back-up is kept on a **separate device or off-site**, so a local failure does not destroy it · restore points allow the system to be rolled back. `9608_s15_qp_12_sc_6.b.i`

> [!info] **File compression** in its own right
> Named in the syllabus notes and credited as one option inside `w23_qp_12_sc_8.b`, but **never the subject of its own question** in 9618 — unlike defragmentation (three questions), disk formatter (two) and backup (two). Lossless vs lossy is Chapter 1 content, so a Chapter 5 question would be about *why a utility for it is provided*: saves storage, reduces transmission time, allows more files in the same space.

> [!info] **Virus checker** described as a utility
> Virus checkers are examined thoroughly in Chapter 6 as a security measure, and appear in Chapter 5 only as one line of a matching exercise and one mark point about freeing RAM. A question asking how a virus checker works *as a utility provided with the OS* would sit in both chapters.

> [!info] Why defragmentation does not help an SSD
> Every defragmentation mark scheme talks about **head movement** — which only exists on a magnetic hard disk. That defragmentation is pointless (and harmful) on solid state storage is never asked, despite Chapter 3 examining SSDs repeatedly.

> [!abstract] Disk formatter, in full
> Prepares a storage device for use by **creating a file system** and organising the space into **sectors and tracks**. Needed to wipe and re-initialise a disk before use, to change the file system format (e.g. FAT32, NTFS), and to remove all data and errors before installing a new OS or reusing a drive.

> [!abstract] Virus checker — two detection approaches
> Use a list of **known malware signatures** to block immediately, or **monitor the behaviour of programs** for suspicious activity — rapid deletion or modification of files, attempts to access sensitive data, communication with known malicious servers. Virus checkers also check for **updates to the signature database**. The behavioural-detection method is absent from every mark scheme in both chapters and is the more modern answer.

> [!abstract] Why fragmentation happens
> As programs and data are added to a new hard disk they are stored in order; over time, deleting files leaves **gaps**, and new data fills those gaps, so files end up split. **Defragmentation can only be used on magnetic storage** — the content for the `!info` gap above.

---

## 5.1.4 Program libraries

> [!success] Define the term program library [2]
> A set of **pre-written / pre-compiled / pre-tested subroutines** · which can be **called** in other programs · by **installing / importing** the library. `9618_s23_qp_12_sc_7.a.i`; `9618_s24_qp_13_sc_7.e.i`

> [!success] Explain how a programmer benefits from using program libraries [3]
> **Programming time is saved** as code does not have to be written from scratch · **testing time is saved** as code is already tested / documented · a library routine is **more likely to work**, as the code is already tested · library routines **automatically update** if they are changed or improved · the programmer can use library routines to perform **complex functions they may not be able to write themselves**. `9618_w25_qp_13_sc_8.b`; `9618_s24_qp_12_sc_8.c`; `9618_w24_qp_11_sc_4.c`

> [!success] Describe one benefit of using library routines, with expansion [2]
> Less code needs to be developed as code is pre-written … thereby reducing the time to write a program · the library routine will be pre-tested and documented … reducing testing time // giving confidence that the routine works · the code can be **written in a different programming language** … which allows the use of special features of that language · the user's source code is **more readable** … as the routine is simply called rather than written out in full · the library could contain complex routines … allowing the programmer to include modules they might not be able to code. `9618_w25_qp_11_sc_5.b.i`

> [!success] Describe one **drawback** of using library routines, with expansion [2]
> **Compatibility issues** … the library routine may not work with the current program · **not guaranteed to be thoroughly tested** … there could be unexpected problems (bugs / virus) · the routine may **not match needs exactly** // may give unexpected results … so it will need to be edited and tested · if the routine is **later edited or changed by someone else** … there could be unexpected errors or results. `9618_w25_qp_11_sc_5.b.ii`

> [!success] Describe the benefits of **creating** a program library [3]
> Subroutines can be **shared / reused** … between team members working independently … without having to rewrite or re-test them, saving the programmers' time · a program library provides **continuity** between programs and programmers · individual programmers can **contribute their specialisms** to the library, or use the specialisms of others. `9618_w24_qp_12_sc_4.b`

> [!success] Explain two benefits of creating a **Dynamic Link Library (DLL)** [4]
> **Memory requirements are reduced** … as the DLL is loaded only once / only when required · the **executable file size is smaller** … because the executable does not contain all the library routines · **maintenance is not needed by the programmer** … because the DLL is separate from the program · **no need to recompile** the main program when changes are made to the DLL … because changes, improvements and error corrections to the DLL are done independently of the main program · a single DLL can be made available to **several application programs** … saving memory. `9618_s23_qp_12_sc_7.a.ii`; `9618_s24_qp_13_sc_7.e.ii`; `9618_w22_qp_11_sc_7.a`

> [!success] Describe how a program library is used while writing a program [2]
> Program libraries store **pre-written functions and routines** · the library can be **referenced / imported** · the functions/routines can then be **called** in her own program. `9618_s21_qp_12_sc_7.a`

> [!warning] State three benefits of using library programs [3]
> The routines are **already written and tested**, so development is faster · they are **reliable / error-free** because they have been used many times · the programmer does not need **specialist knowledge** of that area · they can be **reused** in many programs · they may be **optimised** and so run efficiently. `9608_w21_qp_11_sc_7.c`; `9608_w19_qp_13_sc_6.b`; `9608_s19_qp_11_sc_3.a.i`; `9608_w16_qp_12_sc_8.a`

> [!warning] State three reasons why a program uses DLL files [3]
> The DLL is only **loaded into memory when it is needed**, so memory use is lower · the **executable is smaller** · the DLL can be **shared by several programs** at once · the DLL can be **updated or replaced without recompiling** the main program. `9608_s20_qp_13_sc_4.a.i`; `9608_w16_qp_12_sc_8.b.i`

> [!warning] State two reasons why a program might **not** use DLL files [2]
> The program **will not work if the DLL is corrupted** · an **external change** to the DLL (by another program or a user) could stop the program working · the DLL **must be present at run time** — the executable is not self-contained ("unable to find X.dll") · a **malicious change** to a DLL could introduce a virus. `9608_s20_qp_13_sc_4.a.ii`; `9608_w16_qp_12_sc_8.b.ii`

> [!warning] Describe a library routine / describe a DLL file [2]
> **Library routine** — a pre-written, pre-tested block of code that performs a common task, stored in a library and **called** by a program. **DLL** — a file of one or more routines that is **not** included in the executable at compile time but is **linked and loaded at run time**, and can be shared between programs. `9608_s19_qp_11_sc_3.a.ii`; `9608_w18_qp_12_sc_6.b.i`; `9608_w16_qp_13_sc_2.c`

> [!warning] Give one benefit and one drawback of using library routines [4]
> *Two marks each — point plus expansion.* **Benefit** — already written and tested … so development time is cut and fewer errors are introduced. **Drawback** — the programmer **cannot see or change the source code** … so the routine may do more than is needed, be inefficient, or not fit the problem exactly. `9608_w18_qp_12_sc_6.b.ii`

> [!info] **Drawbacks of a DLL**
> The benefits of DLLs have been examined **three times** (2, 4 and 4 marks). The drawbacks — version conflicts if a newer DLL is incompatible, the program failing to run if a required DLL is missing, security risk from a malicious or altered DLL, and errors being harder to trace across programs — have **never** been asked, even though `w25_qp_11_sc_5.b.ii` shows the examiners are willing to ask for library drawbacks.

> [!info] **Static** linking versus dynamic linking
> Every DLL mark scheme contrasts the DLL with "a library that does not include DLL files", but the term **static library** is never used and the contrast is never asked for directly: a static library is compiled **into** the executable, making it larger but self-contained; a DLL is linked at run time.

> [!abstract] Extra library advantages
> **Promotes code reuse** — well-tested routines used in multiple programs, reducing duplication · **improves reliability** — routines are thoroughly tested and debugged · **easier maintenance** — updates to a routine benefit all programs that use it, especially with DLLs · **efficient memory usage** — DLLs are loaded only when needed at run time · **standardisation** — promotes consistency in how common tasks such as file handling and sorting are implemented. Typical library tasks: sorting, displaying graphics, playing sounds, managing data.

> [!abstract] DLL drawbacks — the content for the untested bullet
> **Version conflicts** if a newer DLL is not compatible · the program **may fail to run** if a required DLL is missing · **security risk** — a malicious or altered DLL can be substituted · **debugging is harder** — errors inside a DLL can be difficult to trace across the multiple programs that use it.

---

# 5.2 Language Translators

## 5.2.1 The need for an assembler, a compiler and an interpreter

> [!success] Complete the descriptions of language translators [4]
> **Compilers** are used when a high-level program is complete; they translate all the code at once and produce **executable / .exe / object code** files that run without the source code. **Interpreters** translate one line at a time and then run that line, most useful while developing because errors can be corrected and the program continues from that line. **Assemblers** translate assembly code into **binary / machine code**. `9618_w21_qp_11_sc_4.d`

> [!success] Complete the description of compilers and interpreters [4]
> A compiler checks all the code before attempting to translate; if any errors are found they are all reported at the same time and the program does not translate or run. If there are no errors the compiler produces **an executable file / .exe** which can run without access to the **source / program code**. An interpreter translates one line and runs it before moving on; if the line has an error the interpreter **stops** and displays the error; the programmer can correct the error **immediately / in real time** and the interpreter continues translating from that point. `9618_s25_qp_13_sc_3.a`

> [!success] Explain how a programmer can use an interpreter and then a compiler [4]
> **Interpreter:** use it while writing/coding the program … to test/debug the partially completed program … because errors can be corrected and processing continues from where execution stopped // errors are identified one at a time. **Compiler:** use it after the program is complete … to create an executable file so the source code is not seen … use it to repeatedly test the same completed section without having to re-interpret every time. *(Max 2 each.)* `9618_w25_qp_12_sc_10.a`; `9618_s21_qp_12_sc_7.b.i` (max 3 each)

> [!warning] Complete the table by ticking the translator being described [4]
> A four-row tick table across **assembler**, **compiler** and **interpreter**. `9608_s21_qp_11_sc_8.a.i`; `9608_w17_qp_13_sc_2.a`; `9608_s16_qp_12_sc_1`

> [!warning] State the purpose of a language translator, and name another translator [1 + 1]
> **Purpose** — to convert program code written in one language (usually source code in a high-level or assembly language) into another form, usually **machine code**, so the processor can execute it. **Other translators** — assembler, compiler, interpreter. `9608_s19_qp_12_sc_2.a.i`; `9608_s19_qp_12_sc_2.a.iii`

> [!info] The **assembler** in its own right
> Assembler is named in the syllabus bullet alongside compiler and interpreter, but appears in 9618 only as **one gap in one cloze** (`w21_qp_11_sc_4.d`). Every other question in this bullet is compiler-vs-interpreter. "Explain the need for assembler software" — one mnemonic instruction maps to one machine code instruction, so a simple translator suffices, and assembly cannot be executed directly — has never been asked.

> [!info] Why a high-level language needs translating at all
> Implied throughout but never asked: the processor can only execute machine code, and a high-level statement corresponds to many machine code instructions.

> [!abstract] The three translators compared
> **Assembler** — translates mnemonics in assembly (low-level) into machine code; **each line of assembly assembles into a single machine code instruction**.
> *Advantages:* speed of execution; optimises the code; original source code will not be seen. *Disadvantages:* difficult to write due to limited, hard-to-understand commands; changes mean it must be reassembled; designed solely for one specific processor.
> **Compiler** — translates a high-level language into machine code all in one go, producing a distributable executable. *Advantages:* speed of execution; optimises the code; source code not seen. *Disadvantages:* can be memory intensive; difficult to debug; changes mean recompiling; designed for one specific processor.
> **Interpreter** — translates and executes one line at a time, stopping at the first error; does not generate machine code directly, but **calls the appropriate machine code subroutines**. *Advantages:* stops at a specific syntax error; easier to debug; **requires less RAM**. *Disadvantages:* slower execution; must be translated every time it is run; no optimisation.
> The "calls machine code subroutines rather than generating machine code" point and the RAM point appear in no mark scheme.

---

## 5.2.2 Benefits and drawbacks of a compiler or interpreter, and justifying each

> [!success] Describe the advantages of an interpreter compared with a compiler [4]
> Easier to **debug** the program · because it translates **line-by-line and stops when an error is found**, whereas the compiler translates the whole program at once · only reporting **one error at a time** · which allows the error to be corrected in **real time**, whereas with a compiler the program must be corrected and recompiled · the program can **restart at the same point** where the error occurred, whereas with a compiler it must be re-run · the effect of any changes can be seen **immediately** · a **partially completed program** can be translated and tested on its own, which a compiler cannot do. `9618_w23_qp_11_sc_6.a`

> [!success] State two disadvantages of a compiler compared with an interpreter [2]
> Large amounts of source code take time to compile · it can be slower to produce the object code than an interpreter · the code must be **recompiled when it is changed** · the program **cannot run if there are errors** · it is not possible to correct errors in real time · **one error can cause false reporting of multiple further errors** · sections of code / unfinished code cannot easily be tested. `9618_w25_qp_13_sc_8.a`; `9618_w22_qp_12_sc_1.b.i`

> [!success] Explain why an executable file makes the compiler the appropriate choice [3]
> The program can be **distributed without the source code** … so it cannot be edited, stolen or plagiarised · users **do not require the translator** to run the program … so time is not spent retranslating by the user. `9618_s24_qp_11_sc_3.b`

> [!success] Explain the reasons why a programmer uses a compiler when the program is complete [3]
> The compiler produces an **executable file** … so the user cannot access, edit or sell the code … and users do not need the translator to run the game · the game can be **compiled for different hardware specifications** … and then used to generate more income for the programmer · the program can be **tested multiple times without having to retranslate** each time. `9618_s23_qp_13_sc_5.a.ii`

> [!success] Explain why it is easier to debug using an interpreter [2]
> The interpreter **stops when an error is found** … so the error can be corrected in real time, and the result of changes is seen immediately · **only one error is displayed at a time** … so there are fewer errors to correct simultaneously **and** no dependent errors. `9618_s24_qp_11_sc_3.a`

> [!success] Describe the benefits of using the compiler during testing [2]
> Creates an **executable file** … so the code can be tested multiple times without having to recompile … so **repeated testing takes less time**. `9618_s24_qp_12_sc_8.a`

> [!success] Identify whether an interpreter or a compiler is appropriate, and justify [3]
> **No mark for the choice — all marks are in the justification.** *Interpreter:* allows real-time changes … so the program can be debugged **at each stage** … the effect of changes is seen immediately · the developer can test when incomplete … so small parts can be tested without testing the rest … if one section does not work others can still be tested · to avoid **dependent errors**. *Compiler:* the developer can debug **multiple errors simultaneously** · produces an executable file … so the program can be tested multiple times without recompiling. `9618_s23_qp_12_sc_7.b`

> [!success] Explain why an interpreter is used while writing the program code [2]
> The programmer can test sections of the code **without every part working or being written** · can debug in **real time** … so errors can be fixed and the program continued from that point · the effect of any changes can be seen immediately · to avoid **dependent errors**. `9618_s23_qp_13_sc_5.a.i`

> [!warning] Explain why a programmer would use both an interpreter and a compiler [4]
> *Max 3 for each side.* **Interpreter** — used while developing, because it stops at the first error and reports it with its line, errors are easier to find and correct, and no full recompilation is needed after every change. **Compiler** — used once the program is complete, to produce an executable that runs faster, runs without the translator present, can be distributed without the source code, and can be **cross-compiled for a different platform**. `9608_w18_qp_12_sc_6.c`

> [!warning] State three benefits of using an interpreter [3]
> Errors are reported **one at a time, as they are met**, with the line number · the program can be run and tested **without waiting for a full compilation** · partially written programs can be run · it is easier to **trace and debug** · the same source can run on any machine with that interpreter. `9608_w21_qp_11_sc_10.a`

> [!warning] State one drawback of using an interpreter [1]
> The **source code is needed every time** the program runs · **no executable file** is produced · the translator must be present on the machine · **execution is slower**, because each line is translated every time it is met (including on every loop pass). `9608_w21_qp_11_sc_10.b`

> [!warning] State three drawbacks of using a compiler [3]
> The **whole program must be compiled** before it can be run · errors are reported only at the end, as a list, so debugging is slower · the source must be **recompiled after every change** · the object code is **machine/platform specific** · compilation of a large program takes a long time and uses memory. `9608_s21_qp_13_sc_7.a`

> [!warning] Complete the table comparing an interpreter with a compiler [5]
> A five-row comparison table — the densest single translator question in either series. `9608_w15_qp_13_sc_11`

> [!warning] Explain why a web language such as JavaScript is interpreted [2]
> The code is sent as **source** to the client and must run on **any browser / platform**, so it cannot be pre-compiled to one machine code · it is interpreted by the browser as the page loads, so it runs immediately without a separate build step. `9608_w19_qp_11_sc_2.d`

> [!info] **Advantages of a compiler** asked positively
> Nine questions in this bullet, and every one is either "advantages of the interpreter", "disadvantages of the compiler", or "why use a compiler **at the end**". A plain "state two advantages of using a compiler" — faster execution of the finished program, optimised code, no translator needed at run time, source code protected — has not been set, even though all those points are credited elsewhere.

> [!info] **Disadvantages of an interpreter**
> Likewise untested as a question in its own right: slower execution because translation happens every run, the translator must be present on the user's machine, the source code is exposed, and no optimisation is performed.

> [!info] Execution speed of the **finished** program
> Every 9618 question is about the **development** stage. The runtime difference — compiled code runs faster because it is already machine code, whereas interpreted code is retranslated line by line every time it runs — is the single most important compiler advantage and appears in no 9618 mark scheme in this bullet.

---

## 5.2.3 Programs partially compiled and partially interpreted

> [!success] State a reason why some high-level languages are partially compiled and partially interpreted [2]
> Partially compiled programs can be used on **different platforms**, as they are **interpreted when run** · code is **optimised for the CPU**, as machine code is generated at **run time** · source code does not need recompiling, so it is more efficient to run. `9618_w23_qp_11_sc_6.b`; `9618_w22_qp_12_sc_1.b.ii`

> [!warning] Explain why a game bought pre-compiled does not need a translator on the user's machine [2]
> It has already been translated into **machine code / an executable** · so the processor can run it directly, and **no translator is required** on the customer's computer (which also keeps the source code hidden). `9608_s20_qp_11_sc_8.b`

> [!info] The **mechanism**, not just the reason
> Both 9618 questions ask *why*. **Neither asks how**: the source is compiled to an intermediate **bytecode**, which is then interpreted by a **virtual machine** on each platform. The syllabus names Java (console mode) explicitly, and the words *bytecode* and *virtual machine* appear in no 9618 mark scheme for this bullet — the nearest is "machine code is generated at run time".

> [!info] Java named in a question
> The syllabus notes say "such as **Java (console mode)**". Neither 9618 question names a language; both are generic. A question set in a named language context has not appeared.

> [!info] Drawbacks of the hybrid approach
> Untested: slower than fully compiled code because the intermediate code is still interpreted, and the target machine must have the virtual machine installed.

---

## 5.2.4 Features found in a typical Integrated Development Environment (IDE)

> [!danger] No 9608 questions, eleven 9618 questions
> The most heavily examined bullet in this chapter, and entirely new in 9618. The syllabus notes group the features under four headings — **coding**, **initial error detection**, **presentation**, **debugging** — and 9618 questions almost always ask by heading, so learn them grouped, not as one list.

> [!success] Identify one common IDE feature for each purpose and describe it [6]
> **For coding — Context-sensitive prompts:** gives **suggestions** for code as the user types instead of having to write or remember the code. **For coding — Auto-correct:** corrects spelling mistakes so the user has fewer errors to correct. **For presentation — Pretty-printing:** colour codes keywords so the user can identify any errors. **For presentation — Expand/collapse code blocks:** the user can hide code they are not currently working on. **For debugging — Single stepping:** run the code **one line at a time** // shows the effect of each line of code. **For debugging — Breakpoints:** stop the code running at a set point to check the flow or variable contents. *(1 mark feature + 1 mark matching description, ×3.)* `9618_s24_qp_12_sc_8.b`

> [!success] Describe how programmers use the debugging features of a typical IDE [4]
> **Single stepping** — run the program one line at a time … and check the variable contents / program flow // show the effect of each line of code · **Set breakpoints** — run the code up to a set line … and then check the status · **Variable / report watch window** — view how the data changes as the program is running. `9618_w24_qp_12_sc_4.a`

> [!success] Describe named IDE features [4]
> **Context-sensitive prompts:** as the code is being written … the options to complete the statement are shown. **Single stepping:** allows the programmer to execute the program one line at a time … so that the effects of each statement can be seen. *(Max 2 per feature.)* `9618_w23_qp_13_sc_5.a`

> [!success] Complete a table describing typical IDE features [4]
> **Breakpoints** — stop the code at a specific line to check the current progress / values · **Dynamic syntax checks** — highlight / underline / colour syntax errors **as the code is entered** · **Context-sensitive prompts** — suggest the code to add // automatically complete statements · **Single stepping** — run the code one line at a time so the values can be checked. `9618_s23_qp_12_sc_7.c`

> [!success] Identify and describe one other **presentation** feature [2]
> **Expand/collapse code blocks** … sections of source code that are part of the same block can be expanded to see the content or collapsed so the overall code is seen · **Auto-indentation / auto-formatting** … automatically indents or formats code as the user types so the structure is clear // aids readability. `9618_w24_qp_11_sc_4.d.i`

> [!success] Identify and describe one other **debugging** feature [2]
> **Breakpoints** … stops the code running on a set line to view the current status / variable contents / program flow · **Report window / variable watch window** … shows the values in variables and data structures and how they change when each line is run. `9618_w24_qp_11_sc_4.d.ii`

> [!success] Identify two presentation features [2]
> Prettyprint · expand/collapse code blocks · **auto** indentation / formatting. `9618_w25_qp_11_sc_5.c`; `9618_w23_qp_11_sc_6.c.i`

> [!success] Identify two debugging features [2]
> Single stepping · breakpoints · report window · **variable expressions**. `9618_w23_qp_11_sc_6.c.ii`; `9618_s21_qp_12_sc_7.b.ii`

> [!success] Identify three tools that support the **writing** of a program [3]
> Colour coding // pretty printing · **auto-complete** · **auto-correct** · context-sensitive prompts · expand and collapse code blocks. `9618_w21_qp_11_sc_4.b.ii`

> [!info] **Dynamic syntax checks** as their own question
> The syllabus notes give "initial error detection, including **dynamic syntax checks**" its own heading, alongside coding, presentation and debugging. It has appeared **once**, as one row of the `s23_qp_12_sc_7.c` table — whereas presentation and debugging have four questions each. It is the least-examined of the four headings and the most likely next target.

> [!info] The IDE's **built-in translators** as a feature
> `s24_qp_12_sc_8.b` explicitly says "**do not** give translator as one of your features", which tells you examiners consider it an obvious answer. Two other questions (`s21_qp_12_sc_7.b.i`, `s24_qp_12_sc_8.a`) treat the built-in compiler and interpreter as IDE features. The link — that an IDE bundles editor, translators and debugger in one environment — is never asked directly.

> [!info] Why an IDE is used at all
> Every question names features. "Explain the benefits to a programmer of using an IDE rather than a plain text editor" — errors caught as you type, no switching between tools, debugging without extra software, faster and more accurate coding — has not been set.

> [!abstract] The four headings, with every feature the notes name
> **For coding:** context-sensitive prompts (suggests completions as you type); auto-complete (e.g. closing brackets added automatically); auto-correct (fixes common typing errors).
> **For initial error detection:** dynamic syntax checks — errors highlighted **as the code is entered**, so mistakes are caught instantly.
> **For presentation:** prettyprint / syntax highlighting (distinct colours for keywords, strings, comments, variables); expand and collapse code blocks; auto-indentation; **code comments**, which are not executed but document the code's purpose.
> **For debugging:** single stepping; breakpoints; report window / variable watch window; variable expressions.
> SME's definition of an IDE is worth having for a "what is an IDE" opener: *software providing a comprehensive, integrated platform to write, edit, compile, debug and manage code efficiently* — it may be a downloaded app or web-based.
