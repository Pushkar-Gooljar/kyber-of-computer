---
title: Pack — 5 System Software (AS Level)
syllabus: 9618 (2026)
topics: 5.1 Operating Systems · 5.2 Language Translators
pairs with: Jigsaw
---

# Pack — 5 System Software

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **9608 |** — same rule, using 9608 tariffs. Still inside the 9618 syllabus wording, but untested in the current series.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

> [!danger] 5.2.4 (IDE) is 9618-only and the most examined bullet in the chapter
> The 9608 Legend has **no** IDE questions. 9618 has asked it **eleven times** since 2021. Every IDE entry below is `9618 |` — there is no old-syllabus safety net, and no excuse for leaving it last.

---

# 5.1 Operating Systems

## 5.1.1 Why a computer system requires an Operating System

> [!question] 9618 | Describe the purpose of an Operating System in a computer [5]
> Describe the purpose of an Operating System in a computer system.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Provides a **user interface**
>> - … so that the user is able to communicate with the hardware
>> - **Manages memory**
>> - … so that data can be stored and accessed, and multi-tasking is possible
>> - **Manages files**
>> - … allowing the user to create, edit, update and delete files and folders
>> - Manages **inputs and outputs** from hardware / peripherals
>> - **Handles processes**, making sure each process has fair access to the processor
>>
>> *Latest: `9618_s25_qp_11_sc_6.b`*

> [!question] 9618 | State one purpose of the Operating System [1]
> State one purpose of the Operating System.
>
>> [!success]- Answer — 3 points for 1 mark
>> - To **hide the complexities of the hardware** from the user
>> - To provide a **platform on which application software can run**
>> - To provide a **user interface**
>>
>> *Latest: `9618_w23_qp_12_sc_8.a`*

> [!question] 9608 | Explain why a personal computer needs an Operating System [2]
> Explain why a personal computer requires an Operating System.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Without it the **hardware cannot be used** // the computer would not function
>> - It acts as an **interface between the user and the hardware**
>> - It provides a **platform on which application software can run**
>> - It **hides the complexity** of the hardware from the user
>>
>> *Latest: `9608_s17_qp_12_sc_4.a.i`*

> [!question] 9608 | Identify the type of software being described [4]
> Complete the table by identifying the type of software described in each row.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Manages the hardware and provides a platform for other software → **operating system**
>> - Performs a specific housekeeping task on the system → **utility program**
>> - Allows the user to carry out a task such as writing a letter → **application software**
>> - Converts source code into machine code → **translator / compiler**
>> - System software = operating system + utilities + translators
>> - Application software is **not** system software, even when supplied with the OS
>>
>> *Latest: `9608_w19_qp_12_sc_1.a`*

> [!question] Inferred | Describe the four types of user interface an OS can provide [4]
> An Operating System provides a user interface. Describe four different types of user interface.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Command line interface (CLI)** — the user types text commands
>> - … fast for an expert, but the commands must be known exactly
>> - **Graphical user interface (GUI)** — windows, icons, menus and pointers (WIMP)
>> - … intuitive for a novice, but uses more memory and processing power
>> - **Menu interface** — the user chooses one option at each stage from successive menus
>> - **Natural language interface (NLI)** — the user speaks or types in ordinary language
>>
>> *Inference: "provide a user interface" is credited in both 9618 OS-purpose mark schemes, but no 9618 question has yet asked what the interfaces are. 9618 marks description questions at 1 mark per named item plus expansion, so 4 is the natural tariff.*

> [!question] Inferred | Explain what would happen if a computer had no Operating System [3]
> Explain the problems that would arise if a computer system had no Operating System.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Every program would have to **manage the hardware itself**
>> - … so each program would need its own drivers for every device
>> - There would be **no multi-tasking** — only one program could run at a time
>> - There would be **no file system**, so data could not be organised or found easily
>> - There would be **no common user interface**, so the user must address the hardware directly
>>
>> *Inference: both 9618 questions ask the purpose positively. The inverse framing is a standard 9618 "explain" move, and it marks at 3.*

> [!question] SME | Give one example of each type of user interface [4]
> For each of four types of user interface, give one example of a device or system that uses it.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **CLI** — MS-DOS, the Linux/Raspbian terminal
>> - … used by advanced users and system administrators
>> - **GUI** — Windows, macOS, Android
>> - … optimised for mouse and touch input
>> - **Menu** — a chip-and-PIN machine, a vending machine, a streaming service
>> - **Natural language** — Alexa, Siri, a search engine
>>
>> *SME's one-line justification for the whole bullet: a user does not need to know where on secondary storage data is kept, only that it is saved for when they want it again.*

---

## 5.1.2 Key management tasks carried out by the Operating System

> [!question] 9618 | Identify the key management tasks carried out by an Operating System [4]
> Identify four key management tasks carried out by an Operating System.
>
>> [!success]- Answer — 9 points for 4 marks
>> - **Memory** management
>> - **File** management
>> - **Security** management
>> - **Hardware / device / peripheral / resource** management
>> - **Input–output** management
>> - **Process** management
>> - **Error checking and recovery**
>> - Provision of a **platform for software** to run on
>> - Provision of a **user interface**
>>
>> *Latest: `9618_w25_qp_13_sc_8.d` (also `9618_s23_qp_11_sc_3.b`, `9618_s21_qp_11_sc_2.b`)*

> [!question] 9618 | Describe the process management tasks performed by an Operating System [5]
> Describe the tasks performed by the process management of an Operating System.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Manages the **scheduling** of processes // decides which process runs next
>> - Manages the **resources** each process requires, such as allocating memory
>> - Enables processes to **share data**
>> - **Prevents interference** between processes // resolves conflicts between them
>> - Handles the **process queue**
>> - Allows **multi-tasking / multi-processing**
>> - … by ensuring fair access, handling priorities and handling interrupts
>>
>> *Latest: `9618_w24_qp_12_sc_3.c` (also `9618_s23_qp_12_sc_5.d.i`)*

> [!question] 9618 | Describe the file management tasks carried out by an Operating System [4]
> Describe the tasks carried out by the file management of an Operating System.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Allows files to be **created, opened, read, written, renamed and deleted**
>> - Organises files into a **directory / folder structure**
>> - Keeps track of **where each file is physically stored** on secondary storage
>> - … maintaining the file allocation table / directory
>> - Manages **access rights and permissions** to files
>> - Allows files to be **moved and copied** between locations
>>
>> *Latest: `9618_w24_qp_11_sc_2.b`*

> [!question] 9618 | Describe how an Operating System manages peripheral hardware devices [4]
> Describe how the Operating System manages the peripheral devices attached to a computer.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Installs and uses the appropriate **device driver** for each peripheral
>> - **Detects** devices as they are connected and keeps track of their **status**
>> - Sends data to and receives data from each device
>> - Uses **buffers and queues** so that slow devices do not hold up the processor
>> - Handles **interrupts** raised by devices when they need attention
>> - Resolves **conflicts** when two programs request the same device
>>
>> *Latest: `9618_s24_qp_12_sc_4.c`*

> [!question] 9618 | State two tasks performed by hardware management [2]
> State two tasks performed by the hardware management of an Operating System.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Communicates with hardware using **device drivers**
>> - Allocates hardware **resources** to the processes that need them
>> - Keeps track of which devices are **connected and available**
>> - Manages the **transfer of data** between the processor and peripherals
>>
>> *Latest: `9618_w23_qp_11_sc_5.b`*

> [!question] 9618 | State two tasks performed by security management [2]
> State two tasks performed by the security management of an Operating System.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Manages **user accounts, usernames and passwords**
>> - Controls **access rights / privileges** to files and resources
>> - Applies **updates and patches** to the Operating System
>> - Keeps **logs** of system access and provides / manages the firewall and anti-malware
>>
>> *Latest: `9618_w23_qp_11_sc_5.c`*

> [!question] 9618 | Describe how memory management organises and allocates RAM [2]
> Describe how the memory management of an Operating System organises and allocates RAM.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Allocates** memory to each program and its data as it is loaded
>> - Keeps track of which areas of memory are **in use and which are free**
>> - **Deallocates** memory when a process ends, so it can be reused
>> - **Protects** each process's memory so one program cannot overwrite another's
>>
>> *Latest: `9618_s24_qp_11_sc_3.b`*

> [!question] 9618 | Explain how memory and process management support multi-tasking [4]
> Explain how memory management and process management work together to allow a computer to multi-task.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Process management **schedules** the processes, giving each a share of processor time
>> - … so each appears to run at the same time
>> - Memory management **allocates a separate area of memory** to each process
>> - … so more than one program can be resident in RAM at once
>> - Memory protection stops one process **overwriting** another's data
>> - When memory is short, **virtual memory / paging** moves data to backing store so more processes fit
>>
>> *Latest: `9618_w25_qp_12_sc_5.c`*

> [!question] 9618 | Match each Operating System management task to its description [4]
> Complete the table by writing the name of the management task that matches each description.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Allocates and deallocates RAM to processes → **memory management**
>> - Decides which process the processor runs next → **process management**
>> - Keeps track of where files are stored and who may open them → **file management**
>> - Communicates with printers and scanners using drivers → **device / peripheral management**
>> - Manages usernames, passwords and access rights → **security management**
>> - Produces diagnostic messages when something goes wrong → **error checking and recovery**
>>
>> *Latest: `9618_s22_qp_12_sc_4.a`*

> [!question] 9608 | Describe the process management and user interface tasks of an Operating System [6]
> Describe the tasks carried out by (a) process management and (b) the user interface of an Operating System.
>
>> [!success]- Answer — 8 points, max 4 for each task, 6 marks
>> - **Process management:** schedules processes // decides which runs next
>> - … allocates resources to each process
>> - … handles interrupts
>> - … prevents processes interfering with each other
>> - … enables multi-tasking by sharing processor time
>> - **User interface:** allows the user to communicate with the computer
>> - … hides the complexity of the hardware
>> - … allows the user to run software and manage files and folders
>>
>> *Latest: `9608_w19_qp_11_sc_2.b`*

> [!question] 9608 | State three tasks carried out by memory management [3]
> State three tasks carried out by the memory management of an Operating System.
>
>> [!success]- Answer — 6 points for 3 marks
>> - Allocates memory to programs and data
>> - Keeps track of which memory is **in use** and which is **free**
>> - **Deallocates** memory when a process finishes
>> - **Protects** one program's memory from another
>> - Allocates **virtual memory**, using **paging** or **segmentation**
>> - Moves data between main memory and **backing store**
>>
>> *Latest: `9608_w21_qp_11_sc_7.a.i` (also `9608_s20_qp_11_sc_8.a` at 4 marks)*

> [!question] 9608 | State two tasks carried out by input/output device management [2]
> State two tasks carried out by the input/output device management of an Operating System.
>
>> [!success]- Answer — 7 points for 2 marks
>> - Sends data to and receives data from peripherals
>> - Manages **device drivers**
>> - Manages **buffers and queues** for devices
>> - Handles **interrupts** raised by devices
>> - **Detects devices** as they are connected
>> - Keeps track of the **status** of each device
>> - Handles **power management** for devices
>>
>> *Latest: `9608_w21_qp_11_sc_7.a.ii` (also `9608_s21_qp_13_sc_4.a.i` at 3 marks)*

> [!question] 9608 | State three tasks carried out by error detection and recovery [3]
> State three tasks carried out by the error detection and recovery function of an Operating System.
>
>> [!success]- Answer — 8 points for 3 marks
>> - Deals with **interrupts**
>> - Deals with **run-time errors**
>> - Deals with **hardware faults**
>> - Produces **error diagnostic messages** for the user
>> - **Deadlock detection and recovery**
>> - Allows **safe-mode** boot-up
>> - Performs a controlled **system shutdown**
>> - Maintains and uses **restore points**
>>
>> *Latest: `9608_s21_qp_13_sc_4.a.ii`*

> [!question] 9608 | State three tasks carried out by file management [3]
> State three tasks carried out by the file management of an Operating System.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Creates, opens, reads, writes, closes and deletes files
>> - Organises files into **folders / directories**
>> - Maintains the **directory structure** and keeps track of where each file is stored
>> - Manages **access rights** to files
>> - Moves, copies and renames files
>>
>> *Latest: `9608_s18_qp_12_sc_1.a.i`*

> [!question] 9608 | Choose two management tasks and describe each [4]
> Choose two management tasks carried out by an Operating System. Describe each one.
>
>> [!success]- Answer — max 2 marks per task, 4 marks
>> - **Memory management** — allocates memory to each process … and deallocates it when the process ends
>> - **File management** — organises files into a directory structure … and controls access rights to them
>> - **Device management** — uses drivers to communicate with peripherals … and buffers data so slow devices do not hold up the processor
>> - **Process management** — schedules which process runs next … and prevents processes interfering with each other
>> - **Security management** — manages accounts and passwords … and applies updates and patches
>>
>> *Latest: `9608_w16_qp_12_sc_7`. The candidate picks the tasks — so any two must be worth two marks each, not just nameable.*

> [!question] 9608 | Describe the sequence of events when a file is read from the hard disk [8]
> Describe the sequence of events that takes place when an application program requests a file from the hard disk.
>
>> [!success]- Answer — 10 points for 8 marks
>> - The application sends a **request for the file** to the Operating System
>> - **File management** looks the file up in the **directory / file allocation table**
>> - … and finds its **physical address** (surface, track, sector)
>> - It checks the user's **access rights** to the file
>> - **Device management** issues the read instruction to the **disk controller** via the **device driver**
>> - The read/write **head is moved to the correct track** and waits for the sector to rotate under it
>> - The sector is read into a **buffer**
>> - An **interrupt** signals that the transfer is complete
>> - **Memory management** allocates an area of main memory for the data
>> - The data is copied from the buffer into that memory and **control returns to the application**
>>
>> *Latest: `9608_w16_qp_12_sc_3`. The longest single question in this chapter in either series.*

> [!question] Inferred | Explain paging, segmentation and virtual memory [4]
> Explain how an Operating System uses virtual memory, and describe how paging and segmentation are used.
>
>> [!success]- Answer — 6 points for 4 marks
>> - When RAM is full, part of the **secondary storage** is used as though it were RAM
>> - Pages / segments not currently needed are **swapped out** to that backing store
>> - … and swapped back in when they are needed again
>> - **Paging** divides memory into **fixed-size** blocks called pages
>> - **Segmentation** divides it into **variable-size** blocks that follow the program's logical structure
>> - Excessive swapping causes **disk thrashing**, which slows the system down
>>
>> *Inference: 9618 credits "manages virtual memory" inside memory-management answers but has never made it the question. A 4-mark describe is how 9618 handles comparable mechanism questions.*

> [!question] Inferred | Describe the error checking and recovery task of an Operating System [3]
> Describe the error checking and recovery tasks carried out by an Operating System.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Detects **run-time errors** and **hardware faults** as they occur
>> - Produces **diagnostic error messages** for the user
>> - Closes the offending process **without crashing the whole system**
>> - Detects and recovers from **deadlock**
>> - Offers **safe mode** or a **restore point** so the system can be recovered
>>
>> *Inference: it appears on the 9618 "identify the key tasks" mark scheme but has never been the subject of its own 9618 question; 9608 asks it at 3 marks, so 3 is the right tariff.*

> [!question] Inferred | Describe scheduling without naming it [3]
> An Operating System must decide which process uses the processor next. Describe how it does this.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Each process is placed in a **queue** when it is ready to run
>> - The scheduler gives each process a **slice of processor time** in turn
>> - Processes are given **priorities**, so more urgent work runs first
>> - A process is **interrupted / pre-empted** when its time slice ends or a higher-priority process arrives
>> - Its state is **saved** so it can resume from where it stopped
>>
>> *Inference: 9618 credits the word "scheduling" in process-management answers but has not asked the candidate to explain the mechanism.*

> [!question] SME | Describe the five key management tasks as a set [5]
> Describe five key management tasks carried out by an Operating System.
>
>> [!success]- Answer — 7 points for 5 marks
>> - **Memory management** — allocates, tracks and deallocates RAM, and manages virtual memory
>> - **File management** — organises files and folders and controls who may access them
>> - **Device / peripheral management** — uses drivers, buffers and queues to talk to hardware
>> - **Process management** — schedules processes and enables multi-tasking
>> - **Security management** — accounts, passwords, access rights, updates and logs
>> - **Input/output management** — controls the flow of data to and from peripherals
>> - **Error checking and recovery** — detects faults and reports or recovers from them
>>
>> *SME frames the chapter around these; the 9618 4-mark "identify" question plus a 1-mark description each gives the tariff.*

---

## 5.1.3 The need for typical utility software

> [!question] 9618 | Match each utility program to its purpose [5]
> Complete the table by writing the name of the utility program that matches each purpose.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Rearranges files into contiguous blocks to cut access time → **disk defragmenter**
>> - Makes a second copy of files so they can be restored → **back-up software**
>> - Scans for and removes malicious software → **virus checker / anti-malware**
>> - Prepares a disk with tracks, sectors and a file system → **disk formatter**
>> - Finds bad sectors and recovers what it can → **disk repair / contents analysis**
>> - Reduces file size for storage or transmission → **file compression**
>> - Scrambles data so it cannot be read without the key → **encryption software**
>>
>> *Latest: `9618_w24_qp_13_sc_2.a`*

> [!question] 9618 | Identify one utility not intended to improve security, and explain why it is needed [3]
> Identify one utility program that is **not** intended to improve the security of a computer, and explain why it is needed.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Disk defragmenter**
>> - … files become fragmented across the disk as they are edited and deleted
>> - … it rearranges them into contiguous blocks, so read/access time falls and performance improves
>> - **File compression** — reduces file size so less storage is used and transmission is faster
>> - **Disk formatter** — prepares a new disk, or wipes an old one, so it can store files
>>
>> *Latest: `9618_s24_qp_13_sc_5.b`*

> [!question] 9618 | Explain how defragmentation software improves performance [3]
> Explain how defragmentation software improves the performance of a computer.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Over time files are stored in **non-contiguous blocks** scattered across the disk
>> - … because files are edited, deleted and new files fill the gaps
>> - The read/write head must **move to several places** to read one file, which is slow
>> - Defragmentation **rearranges the blocks** so each file is stored contiguously
>> - … so head movement is reduced and **access / read time falls**
>>
>> *Latest: `9618_w25_qp_11_sc_4.c`*

> [!question] 9618 | Describe the reasons why a disk formatter is needed [3]
> Describe the reasons why a computer system needs disk formatting software.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Organises the disk into **tracks and sectors** so data can be addressed
>> - Sets up the **file system / directory structure** the Operating System will use
>> - Prepares a **new disk** so it can be used for the first time
>> - **Erases all existing data** from a disk that is being reused or disposed of
>> - Can identify and **mark bad sectors** so they are not used
>>
>> *Latest: `9618_s23_qp_13_sc_3.b`*

> [!question] 9618 | Identify two utility programs that improve performance, and state how [4]
> Identify two utility programs that can improve the performance of a computer, and state how each does so.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Disk defragmenter**
>> - … rearranges fragmented files into contiguous blocks, reducing access time
>> - **File compression**
>> - … reduces file sizes, so less storage is used and files transfer faster
>> - **System clean-up / disk clean-up** — deletes temporary and unused files, freeing storage
>> - **Virus checker** — removes malware that would otherwise consume processor time
>>
>> *Latest: `9618_w24_qp_12_sc_5.b`*

> [!question] 9618 | Explain the need for back-up software [2]
> Explain why a computer system needs back-up software.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Makes a **second copy** of the data on a separate medium or in the cloud
>> - … so the data can be **restored** if the original is lost, corrupted or deleted
>> - Protects against **hardware failure, theft, fire and ransomware**
>> - Can run **automatically on a schedule**, so a recent copy always exists
>>
>> *Latest: `9618_s25_qp_12_sc_3.c`*

> [!question] 9618 | Describe the purpose of utility software in a computer [2]
> Describe the purpose of utility software.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Performs a **specific housekeeping / maintenance task** on the computer system
>> - … keeping the system running efficiently and securely
>> - It is **system software**, usually supplied with the Operating System
>> - Examples: defragmenter, back-up, virus checker, formatter, compression
>>
>> *Latest: `9618_w22_qp_12_sc_1.c`*

> [!question] 9618 | Identify utilities that could recover corrupted image files [2]
> A user's image files have become corrupted. Identify two utility programs that could help, and state how.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Back-up software** — restores an uncorrupted earlier copy of the files
>> - **Disk repair / contents analysis software** — scans for bad sectors and attempts to recover the data
>> - **Virus checker** — removes the malware that caused the corruption, preventing further damage
>> - **Disk defragmenter** would *not* help — recognising this is part of the question
>>
>> *Latest: `9618_s22_qp_11_sc_6.c`*

> [!question] 9608 | Identify and describe two utility programs [4]
> Identify two utility programs and describe the purpose of each.
>
>> [!success]- Answer — 2 marks per program (name + purpose), 4 marks
>> - **Disk defragmenter** — rearranges fragmented files into contiguous blocks to cut access time
>> - **Back-up software** — copies files to a separate medium so they can be restored after loss
>> - **Virus checker** — scans for, quarantines and removes malicious software
>> - **Disk formatter** — organises a disk into tracks and sectors and creates the file system
>> - **File compression** — reduces file size for storage or transmission
>> - **System clean-up, firewall, encryption software** are also credited
>>
>> *Latest: `9608_w21_qp_11_sc_7.b` (also `9608_s21_qp_13_sc_4.b.ii`)*

> [!question] 9608 | Tick to show which programs are utility programs [2]
> Tick to show whether each of the programs listed is a utility program.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Are** utilities: defragmenter, back-up, virus checker, formatter, disk repair, compression
>> - A **translator / compiler** is **not** a utility — it is system software of its own kind
>> - An **IDE** is **not** a utility
>> - **Graphics software** and a **spreadsheet** are **application** software, not utilities
>>
>> *Latest: `9608_s21_qp_13_sc_4.b.i`. The distractors are the whole question.*

> [!question] 9608 | Explain why a user would use back-up, a defragmenter and disk repair software [2 each]
> Explain why a user would use (i) back-up software, (ii) a disk defragmenter, (iii) disk repair software.
>
>> [!success]- Answer — 2 marks per part
>> - **Back-up** — a second copy exists … so data can be restored after loss, corruption or hardware failure
>> - **Defragmenter** — files are stored in scattered blocks … rearranging them into contiguous blocks cuts read/access time
>> - **Disk repair** — scans the disk for bad sectors and corrupted files … marks bad sectors unusable and recovers what it can
>>
>> *Latest: `9608_s21_qp_12_sc_7.a.i`–`iii`*

> [!question] 9608 | Explain how the formatter, contents analysis and repair software work together [3]
> Explain how disk formatting software, disk contents analysis software and disk repair software work together to maintain a hard disk.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The **formatter** organises the disk into tracks and sectors and builds the file system
>> - The **contents analysis software scans** the disk
>> - … identifying used, free, bad and corrupted areas
>> - The **repair software** then fixes the corrupted files or file system
>> - … and **marks bad sectors** so they are not used again, keeping the disk usable
>>
>> *Latest: `9608_s20_qp_12_sc_2.c.i`*

> [!question] 9608 | Describe the purpose of disk repair software [3]
> Describe the purpose of disk repair software.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Checks the disk for **errors and bad sectors**
>> - Attempts to **recover data** from damaged areas
>> - **Marks bad sectors** so that they are not written to again
>> - Repairs the **file system / directory** so files can be located
>> - Reports to the user on the **health of the disk**
>>
>> *Latest: `9608_w19_qp_12_sc_1.b`*

> [!question] 9608 | Describe the purpose of a virus checker and of back-up software [4]
> Describe the purpose of (a) a virus checker and (b) back-up software.
>
>> [!success]- Answer — max 3 for each, 4 marks
>> - **Virus checker:** scans files and memory for known virus **signatures**
>> - … and for suspicious behaviour (**heuristic** checking)
>> - … quarantines or deletes infected files and alerts the user
>> - … must be kept **up to date** with new definitions
>> - **Back-up:** makes a copy of files on a schedule or on demand
>> - … to a separate medium or the cloud
>> - … so data can be restored after loss, corruption or hardware failure
>>
>> *Latest: `9608_w19_qp_11_sc_2.c`*

> [!question] 9608 | Explain when a virus checker should run [2]
> Explain when a virus checker should be run on a computer system.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Continuously **in the background / in real time**, as files are opened or downloaded
>> - On a **scheduled full scan** of the whole system
>> - Whenever **new external media** is connected
>> - Immediately after the **virus definitions are updated**
>>
>> *Latest: `9608_w15_qp_13_sc_10.b`*

> [!question] 9608 | Describe how utility software prevents accidental loss of data [2]
> Describe how utility software can prevent the accidental loss of data.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Automatic, **scheduled back-ups**, so a recent copy always exists
>> - The copy is kept on a **separate device or off-site**, so a local failure does not destroy it
>> - **Restore points** allow the system to be rolled back to a working state
>> - Disk repair software recovers files from damaged areas before they are lost
>>
>> *Latest: `9608_s15_qp_12_sc_6.b.i`*

> [!question] Inferred | Describe the purpose of file compression software [3]
> Describe the purpose of file compression software and explain the difference between its two types.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Reduces the **size** of a file so it uses less storage and transmits faster
>> - **Lossless** compression removes redundancy and the original can be **restored exactly**
>> - … used for text, program files and spreadsheets, where nothing may be lost
>> - **Lossy** compression **discards data** permanently to achieve a smaller file
>> - … used for images, audio and video, where small losses are acceptable
>>
>> *Inference: compression is named in the 9618 utility mark schemes but has never been the question in this topic; 9618 marks lossless-vs-lossy at 3 elsewhere in the syllabus.*

> [!question] Inferred | Describe how a virus checker works [3]
> Describe how a virus checker protects a computer system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Scans files, memory and incoming data against a database of known virus **signatures**
>> - Uses **heuristic** checking to spot suspicious behaviour from unknown malware
>> - **Quarantines** the infected file so it cannot run
>> - … then deletes or attempts to **disinfect** it, after alerting the user
>> - Must be **kept up to date**, because new malware appears constantly
>>
>> *Inference: 9618 names the virus checker in matching questions but never asks how it works, though 9618 does mark comparable "describe how X protects" questions at 3.*

> [!question] Inferred | Explain why defragmentation does not benefit a solid-state drive [2]
> Explain why defragmentation software is not used on a solid-state drive.
>
>> [!success]- Answer — 4 points for 2 marks
>> - An SSD has **no moving parts / no read-write head**
>> - … so access time does not depend on where the data is physically stored
>> - Defragmentation therefore gives **no performance gain**
>> - It also causes unnecessary **write cycles**, shortening the SSD's lifespan
>>
>> *Inference: 9618 has examined SSD-vs-HDD structure in Topic 3 and defragmentation here, but has never joined them. It is the obvious synoptic question.*

> [!question] SME | Describe disk formatting in full [3]
> Describe what happens when a hard disk is formatted.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The disk surface is organised into **tracks and sectors**
>> - A **file system** (e.g. NTFS, FAT32) is written to the disk
>> - An empty **root directory / file allocation table** is created
>> - Any **existing data becomes inaccessible** // the disk is effectively wiped
>> - Bad sectors found during formatting are **marked so they are not used**
>>
>> *SME devotes a section to this; 9618's own 3-mark formatter question sets the tariff.*

> [!question] SME | Explain why file fragmentation happens [2]
> Explain why the files on a hard disk become fragmented over time.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Files are **deleted**, leaving gaps of free blocks scattered across the disk
>> - New or edited files are **larger than a single gap**
>> - … so the Operating System splits them across several **non-contiguous** blocks
>> - The more the disk is used, the more scattered the blocks become
>>
>> *SME explains the cause; 9618's defragmentation mark scheme credits it as the first point of a 3-mark answer.*

---

## 5.1.4 Program libraries

> [!question] 9618 | Define the term program library [2]
> Define the term *program library*.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **collection of pre-written, pre-compiled routines / subroutines**
>> - … that perform common tasks
>> - They are **tested and ready to use**
>> - … and can be **called by** (incorporated into) any program that needs them
>>
>> *Latest: `9618_w25_qp_12_sc_2.a`*

> [!question] 9618 | Explain how a programmer benefits from using program libraries [3]
> Explain the benefits to a programmer of using program libraries.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The routines are **already written**, so development time is reduced
>> - They have been **thoroughly tested**, so they are reliable and contain fewer errors
>> - The programmer does not need **specialist knowledge** of that area
>> - The routines can be **reused** in many different programs
>> - They are often **optimised**, so they run efficiently
>>
>> *Latest: `9618_s25_qp_13_sc_4.b`*

> [!question] 9618 | Describe one benefit of using library routines, with expansion [2]
> Describe one benefit of using library routines in a program.
>
>> [!success]- Answer — 1 point + expansion, 2 marks
>> - The routine is **already written and tested**
>> - … so the program is completed faster and contains fewer errors
>> - *or* the programmer needs no specialist knowledge … so tasks beyond their expertise can still be included
>>
>> *Latest: `9618_w24_qp_11_sc_5.a.i`*

> [!question] 9618 | Describe one drawback of using library routines, with expansion [2]
> Describe one drawback of using library routines in a program.
>
>> [!success]- Answer — 1 point + expansion, 2 marks
>> - The programmer **cannot see or modify the source code**
>> - … so the routine cannot be adapted to fit the problem exactly
>> - *or* the routine may contain **more code than is needed** … so the program is larger and may run more slowly
>> - *or* the library **must be present** when the program runs … so the program will fail if it is missing
>>
>> *Latest: `9618_w24_qp_11_sc_5.a.ii`*

> [!question] 9618 | Describe the benefits of creating a program library [3]
> Describe the benefits to a software company of creating its own program library.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The routines can be **reused across many projects**, saving development time
>> - Code is written and tested **once**, so quality is consistent
>> - Maintenance is easier — a fix in the library **benefits every program** that uses it
>> - Routines can be **shared between programmers** in the company
>> - The library can be **sold or licensed** to others
>>
>> *Latest: `9618_s24_qp_11_sc_6.c`*

> [!question] 9618 | Explain two benefits of creating a Dynamic Link Library (DLL) [4]
> Explain two benefits of using a Dynamic Link Library (DLL).
>
>> [!success]- Answer — 2 marks per benefit (point + expansion), 4 marks
>> - The DLL is only **loaded into memory when it is needed**
>> - … so the program uses less memory, and the executable file is smaller
>> - The DLL can be **shared by several programs** at the same time
>> - … so the same code is not duplicated on the system
>> - The DLL can be **updated or replaced without recompiling** the main program
>> - … so bug fixes and improvements are distributed easily
>>
>> *Latest: `9618_w25_qp_13_sc_5.b`*

> [!question] 9618 | Describe how a program library is used while writing a program [2]
> Describe how a programmer uses a program library when writing a program.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The library is **imported / included** at the start of the program
>> - The programmer **calls** a routine by its name, passing any required parameters
>> - … and uses the value the routine returns
>> - The routine is **linked** into the program by the linker (at compile time, or at run time for a DLL)
>>
>> *Latest: `9618_s23_qp_11_sc_7.b`*

> [!question] 9608 | State three benefits of using library programs [3]
> State three benefits of using library programs.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The routines are **already written and tested**, so development is faster
>> - They are **reliable**, because they have been used many times
>> - The programmer needs no **specialist knowledge** of that area
>> - They can be **reused** in many programs
>> - They may be **optimised**, so they run efficiently
>>
>> *Latest: `9608_w21_qp_11_sc_7.c` (also `9608_w19_qp_13_sc_6.b` at 4, `9608_w16_qp_12_sc_8.a` at 4)*

> [!question] 9608 | State three reasons why a program uses DLL files [3]
> State three reasons why a programmer would use DLL files in a program.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The DLL is only **loaded into memory when it is needed**, so less memory is used
>> - The **executable file is smaller**
>> - The DLL can be **shared by several programs** at once
>> - The DLL can be **updated without recompiling** the main program
>> - The source code of the routine stays **hidden** from the programmer using it
>>
>> *Latest: `9608_s20_qp_13_sc_4.a.i` (also `9608_w16_qp_12_sc_8.b.i` at 4)*

> [!question] 9608 | State two reasons why a program might not use DLL files [2]
> State two reasons why a programmer might choose **not** to use DLL files.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The program **will not work if the DLL is corrupted**
>> - An **external change** to the DLL, by another program or a user, could stop the program working
>> - The DLL **must be present at run time** — the executable is not self-contained ("unable to find X.dll")
>> - A **malicious change** to a DLL could introduce a virus into the program
>>
>> *Latest: `9608_s20_qp_13_sc_4.a.ii` (also `9608_w16_qp_12_sc_8.b.ii` at 2)*

> [!question] 9608 | Describe a library routine and describe a DLL file [2 each]
> (i) Describe what is meant by a library routine. (ii) Describe what is meant by a DLL file.
>
>> [!success]- Answer — 2 marks each
>> - **Library routine** — a pre-written, pre-tested block of code that performs a common task
>> - … stored in a library and **called** by a program when it is needed
>> - **DLL** — a file of one or more routines that is **not included in the executable** at compile time
>> - … but is **linked and loaded at run time**, and can be shared between programs
>>
>> *Latest: `9608_s19_qp_11_sc_3.a.ii`; `9608_w18_qp_12_sc_6.b.i`; `9608_w16_qp_13_sc_2.c`*

> [!question] 9608 | Give one benefit and one drawback of using library routines [4]
> Give one benefit and one drawback of using library routines. Expand each answer.
>
>> [!success]- Answer — 2 marks each (point + expansion), 4 marks
>> - **Benefit:** the routine is already written and tested
>> - … so development time is cut and fewer errors are introduced
>> - **Drawback:** the programmer **cannot see or change the source code**
>> - … so the routine may do more than is needed, be inefficient, or not fit the problem exactly
>>
>> *Latest: `9608_w18_qp_12_sc_6.b.ii`*

> [!question] Inferred | Explain the drawbacks of using a DLL [4]
> Explain two drawbacks of using Dynamic Link Libraries in a program.
>
>> [!success]- Answer — 2 marks per drawback, 4 marks
>> - The executable is **not self-contained**
>> - … so the program fails at run time if the DLL is missing, moved or corrupted
>> - The DLL can be **changed by something outside the program**
>> - … so an update by another program, or a malicious replacement, can break it or inject a virus
>> - **Version conflicts** arise when two programs need different versions of the same DLL
>>
>> *Inference: 9618 has asked DLL **benefits** at 4 marks but never the drawbacks. The mirror question at the same tariff is the obvious next step — and 9608 marks the drawback side at 2.*

> [!question] Inferred | Compare static linking with dynamic linking [3]
> Explain the difference between static linking and dynamic linking of library routines.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Static** linking copies the library code **into the executable at compile time**
>> - … so the executable is larger but **self-contained** and runs without the library present
>> - **Dynamic** linking leaves the code in a separate file, **linked at run time**
>> - … so the executable is smaller and the library can be shared or updated independently
>> - … but the DLL must be present and correct whenever the program runs
>>
>> *Inference: 9618's DLL questions assume the distinction without ever asking for it; a 3-mark compare is how 9618 handles such pairs.*

> [!question] SME | State further advantages of using program libraries [3]
> Other than saving development time, state three advantages of using program libraries.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The routines have been **used and debugged by many programmers**, so they are dependable
>> - Complex tasks (graphics, encryption, mathematics) can be used **without understanding the theory**
>> - The routine is often **optimised** for speed or memory by specialists
>> - Programs written by different people become **consistent**, because they use the same routines
>> - The library may be **maintained by someone else**, so fixes arrive without extra work
>>
>> *SME lists these; 9618's own 3-mark library-benefit question sets the tariff.*

> [!question] SME | Describe the drawbacks of DLL files [2]
> Describe one drawback of storing library routines in DLL files.
>
>> [!success]- Answer — 1 point + expansion, 2 marks
>> - The program depends on a file it **does not contain**
>> - … so if the DLL is deleted, moved, corrupted or replaced with an incompatible version, the program will not run
>> - The user may see an error such as **"unable to find X.dll"** and be unable to fix it
>>
>> *SME supplies the content for the untested drawback bullet; 9618's point-plus-expansion format gives 2.*

---

# 5.2 Language Translators

## 5.2.1 The need for an assembler, a compiler and an interpreter

> [!question] 9618 | Complete the descriptions of language translators [4]
> Complete the statements describing language translators, using the terms provided.
>
>> [!success]- Answer — 6 points for 4 marks
>> - An **assembler** translates **assembly language** into machine code, one instruction to one machine-code instruction
>> - A **compiler** translates the **whole** high-level program into machine code **before** it is run
>> - … producing an **executable** file that can be run repeatedly without the compiler
>> - An **interpreter** translates and executes the program **one line at a time**
>> - … and stops at the **first error** it meets, reporting it to the programmer
>> - All three convert **source code** into a form the processor can execute
>>
>> *Latest: `9618_w25_qp_12_sc_6.a`*

> [!question] 9618 | Complete the description of compilers and interpreters [4]
> Complete the description of how a compiler and an interpreter translate a program.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The compiler translates the **entire** program in one go
>> - … producing an **object / executable** file
>> - … and reports **all errors together** at the end as an error report
>> - The interpreter translates **one line**, executes it, then moves to the next
>> - … so **no executable file** is produced
>> - … and a line inside a loop is **re-translated every time** it is executed
>>
>> *Latest: `9618_s25_qp_12_sc_5.a`*

> [!question] 9618 | Explain how a programmer uses an interpreter and then a compiler [4]
> Explain why a programmer would use an interpreter while developing a program and a compiler once it is finished.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The **interpreter** stops at the first error and reports it with its line number
>> - … so errors are found and corrected quickly, without recompiling the whole program
>> - … and partially written code can be run and tested
>> - The **compiler** is used when the program is complete
>> - … producing an executable that runs faster and needs no translator present
>> - … and can be distributed without releasing the source code
>>
>> *Latest: `9618_w24_qp_13_sc_6.b`*

> [!question] 9608 | Complete the table by ticking the translator being described [4]
> Complete the table by ticking the translator — assembler, compiler or interpreter — that each statement describes.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Translates assembly language into machine code → **assembler**
>> - Translates the whole program before execution → **compiler**
>> - Translates and executes one line at a time → **interpreter**
>> - Produces an executable file → **compiler**
>> - Must be present every time the program runs → **interpreter**
>> - Halts at the first error found → **interpreter**
>>
>> *Latest: `9608_s21_qp_11_sc_8.a.i` (also `9608_w17_qp_13_sc_2.a`, `9608_s16_qp_12_sc_1`)*

> [!question] 9608 | State the purpose of a language translator and name another translator [2]
> (i) State the purpose of a language translator. (ii) Name another type of language translator.
>
>> [!success]- Answer — 1 mark each
>> - **Purpose:** to convert program code written in one language into another form
>> - … usually source code into **machine code**, so the processor can execute it
>> - **Other translators:** assembler, compiler, interpreter
>>
>> *Latest: `9608_s19_qp_12_sc_2.a.i` and `9608_s19_qp_12_sc_2.a.iii`*

> [!question] Inferred | Describe the purpose of an assembler [3]
> Describe the purpose of an assembler and explain why it is needed.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Translates a program written in **assembly language** into **machine code**
>> - Each assembly instruction usually translates to **one machine-code instruction** (one-to-one)
>> - It replaces **mnemonics** with op-codes and **labels / symbolic addresses** with actual addresses
>> - The processor can only execute machine code, so the translation is essential
>> - Assembly language is used where **direct hardware control** or speed is needed
>>
>> *Inference: 9618 credits "assembler" inside cloze questions but has never asked about it on its own, even though 4.2 examines assembly language heavily. A synoptic 3-mark describe is the natural form.*

> [!question] Inferred | Explain why a high-level language must be translated [2]
> Explain why a program written in a high-level language must be translated before it can be run.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The processor can only execute **machine code / binary instructions**
>> - High-level source code is written for **humans to read**, not for the processor
>> - … so it must be converted into machine code by a compiler or interpreter
>> - The translation also allows the same source to run on **different processors**, each with its own translator
>>
>> *Inference: assumed by every question in this sub-topic but never asked directly; 9618 marks such "explain why" questions at 2.*

> [!question] SME | Compare the three translators [6]
> Compare an assembler, a compiler and an interpreter.
>
>> [!success]- Answer — 8 points for 6 marks
>> - **Assembler:** translates assembly language, one-to-one, into machine code
>> - **Compiler:** translates the whole high-level program at once, producing an executable
>> - … errors are reported together at the end, as an error report
>> - … the executable runs faster and without the translator present
>> - **Interpreter:** translates and executes a high-level program one line at a time
>> - … no executable is produced, so the source and the interpreter are needed every run
>> - … execution is slower, because lines are re-translated each time they are met
>> - … but errors are reported immediately, one at a time, making debugging easier
>>
>> *SME frames the sub-topic as a three-way comparison; 9618's 4-mark cloze plus its 2-mark advantage questions justify 6.*

---

## 5.2.2 Benefits and drawbacks of a compiler or interpreter

> [!question] 9618 | Describe the advantages of an interpreter compared with a compiler [4]
> Describe the advantages of using an interpreter rather than a compiler.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Errors are reported **one at a time, as they are found**, with the line number
>> - … so the error is easy to locate and correct
>> - The program can be **run immediately**, with no wait for a full compilation
>> - **Partially written** programs can be run and tested
>> - There is **no need to recompile** the whole program after every change
>> - The same source code can run on **any machine** that has the interpreter
>>
>> *Latest: `9618_s25_qp_12_sc_5.b`*

> [!question] 9618 | State two disadvantages of a compiler compared with an interpreter [2]
> State two disadvantages of using a compiler rather than an interpreter.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **whole program must be compiled** before any of it can be run
>> - Errors are reported **only at the end**, as a list, so they are harder to locate
>> - The program must be **recompiled after every change**, which takes time
>> - The object code is **machine / platform specific**
>>
>> *Latest: `9618_w24_qp_12_sc_6.b`*

> [!question] 9618 | Explain why an executable file makes the compiler the appropriate choice [3]
> A company wants to sell its software to customers. Explain why a compiler is the appropriate translator.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The compiler produces an **executable file**
>> - … which the customer can run **without needing a translator** installed
>> - The **source code is not distributed**, so the company's work is protected
>> - The executable **runs faster** than interpreted code, because it is already in machine code
>> - The customer cannot **alter** the program
>>
>> *Latest: `9618_s24_qp_12_sc_6.c`*

> [!question] 9618 | Explain why a programmer uses a compiler once the program is complete [3]
> Explain the reasons why a programmer uses a compiler when a program is complete.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The program is **finished and error-free**, so line-by-line error reporting is no longer needed
>> - Compilation produces an **executable** that can be distributed
>> - … which runs **faster**, because it is translated only once
>> - … and runs **without the translator** being present
>> - The source code stays **hidden** from the user
>>
>> *Latest: `9618_w23_qp_13_sc_5.c`*

> [!question] 9618 | Explain why it is easier to debug using an interpreter [2]
> Explain why debugging a program is easier when an interpreter is used.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The interpreter **stops at the first error** it meets
>> - … and reports it together with the **line number**, so it is easy to find
>> - Only one error is shown at a time, so the programmer is not overwhelmed
>> - The corrected program can be **re-run immediately**, with no recompilation
>>
>> *Latest: `9618_s23_qp_13_sc_6.b`*

> [!question] 9618 | Describe the benefits of using the compiler during testing [2]
> Describe the benefits of using a compiler during the testing of a program.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **error report** lists every error found in one pass
>> - … so all errors can be corrected together before the next compilation
>> - The compiled program runs at **full speed**, so performance can be tested realistically
>> - It tests the program in the **form the customer will receive**
>>
>> *Latest: `9618_w22_qp_11_sc_6.c`*

> [!question] 9618 | Identify whether an interpreter or a compiler is appropriate, and justify [3]
> For the given scenario, identify whether an interpreter or a compiler is more appropriate and justify your choice.
>
>> [!success]- Answer — no mark for the choice; all 3 marks are in the justification
>> - **Still being written / debugged → interpreter**: errors reported one at a time with line numbers
>> - … the program can be run before it is complete, and no recompilation is needed after each change
>> - **Finished / being sold or distributed → compiler**: an executable is produced
>> - … it runs faster, needs no translator on the user's machine, and hides the source code
>> - The justification **must match the scenario given** — generic advantages score nothing
>>
>> *Latest: `9618_w25_qp_11_sc_5.b`. Examiners repeatedly note that candidates score the choice and lose the marks.*

> [!question] 9618 | Explain why an interpreter is used while writing the program code [2]
> Explain why a programmer uses an interpreter while writing a program.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Errors are reported **as each line is met**, so they are found straight away
>> - … and the line number is given, so the error is easy to locate
>> - Sections of an **incomplete** program can be run and tested
>> - There is no wait for the **whole program to compile** after each change
>>
>> *Latest: `9618_s22_qp_13_sc_5.b`*

> [!question] 9608 | Explain why a programmer would use both an interpreter and a compiler [4]
> Explain why a programmer would use both an interpreter and a compiler when developing software.
>
>> [!success]- Answer — max 3 for each side, 4 marks
>> - **Interpreter** — stops at the first error and reports it with its line number
>> - … errors are easier to find and correct
>> - … no full recompilation is needed after every change, and partial programs can be run
>> - **Compiler** — used once the program is complete, producing an executable
>> - … which runs faster and without the translator present
>> - … can be distributed without the source code
>> - … and can be **cross-compiled for a different platform**
>>
>> *Latest: `9608_w18_qp_12_sc_6.c`. The cross-compilation point is unique to this mark scheme.*

> [!question] 9608 | State three benefits of using an interpreter [3]
> State three benefits of using an interpreter.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Errors are reported **one at a time, as they are met**, with the line number
>> - The program can be run and tested **without waiting for a full compilation**
>> - **Partially written** programs can be run
>> - It is easier to **trace and debug** the program
>> - The same source can run on any machine that has that interpreter
>>
>> *Latest: `9608_w21_qp_11_sc_10.a`*

> [!question] 9608 | State one drawback of using an interpreter [1]
> State one drawback of using an interpreter.
>
>> [!success]- Answer — 4 points for 1 mark
>> - The **source code is needed every time** the program runs
>> - **No executable file** is produced
>> - The **translator must be present** on any machine that runs the program
>> - **Execution is slower**, because each line is translated every time it is met, including on every pass of a loop
>>
>> *Latest: `9608_w21_qp_11_sc_10.b`*

> [!question] 9608 | State three drawbacks of using a compiler [3]
> State three drawbacks of using a compiler.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The **whole program must be compiled** before it can be run
>> - Errors are reported only at the **end**, as a list, so debugging is slower
>> - The program must be **recompiled after every change**
>> - The object code is **machine / platform specific**
>> - Compiling a large program **takes time and memory**
>>
>> *Latest: `9608_s21_qp_13_sc_7.a`*

> [!question] 9608 | Complete the table comparing an interpreter with a compiler [5]
> Complete the table comparing an interpreter with a compiler.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Unit translated: **one line at a time** vs **the whole program**
>> - Output: **no executable produced** vs **an executable / object file**
>> - Error reporting: **first error, immediately** vs **all errors at the end**
>> - Translator needed at run time: **yes** vs **no**
>> - Execution speed: **slower** vs **faster**
>> - Re-translation of loops: **every pass** vs **once only**
>> - Source code distributed: **yes** vs **no**
>>
>> *Latest: `9608_w15_qp_13_sc_11`. The densest single translator question in either series.*

> [!question] 9608 | Explain why JavaScript in a web page is interpreted [2]
> Explain why a scripting language such as JavaScript is interpreted rather than compiled.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The code is sent to the client as **source**, and must run on **any browser or platform**
>> - … so it cannot be pre-compiled into one machine's machine code
>> - The **browser interprets** it as the page loads
>> - … so it runs immediately, with no separate build step
>>
>> *Latest: `9608_w19_qp_11_sc_2.d`*

> [!question] 9608 | Explain why a pre-compiled game needs no translator on the user's computer [2]
> A game is bought as a pre-compiled program. Explain why the user's computer does not need a translator to run it.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The program has already been translated into **machine code / an executable**
>> - … so the processor can execute it **directly**
>> - No translation takes place at run time, so **no translator is required**
>> - It also means the **source code** is not supplied to the user
>>
>> *Latest: `9608_s20_qp_11_sc_8.b`*

> [!question] Inferred | State the advantages of a compiler compared with an interpreter [4]
> Describe the advantages of using a compiler rather than an interpreter.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Produces an **executable file** that can be distributed
>> - … which runs **without the translator** being present
>> - The compiled program **runs faster**, because it is translated only once
>> - … a line inside a loop is translated once, not on every pass
>> - The **source code is not distributed**, so it is protected from copying or alteration
>> - Errors are reported **all together**, so they can be corrected in one pass
>>
>> *Inference: 9618 has repeatedly asked interpreter advantages at 4 marks and compiler disadvantages at 2, but never this direct mirror. Same tariff as its twin.*

> [!question] Inferred | State the disadvantages of an interpreter [3]
> State three disadvantages of using an interpreter.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The **source code must be supplied** every time the program is run
>> - The **interpreter must be installed** on every machine that runs it
>> - Execution is **slower** than compiled code
>> - … because each line is re-translated every time it is executed
>> - **No executable** is produced, so the program cannot be sold as a stand-alone product
>>
>> *Inference: 9618 asks compiler disadvantages but not interpreter disadvantages; 9608 marks it at 1–3, and 9618's comparable "state three" questions carry 3.*

> [!question] Inferred | Compare the execution speed of compiled and interpreted programs [2]
> Explain why a compiled program usually runs faster than the same program run through an interpreter.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The compiled program is **already in machine code**, so no translation happens while it runs
>> - The interpreter must **translate each line as it is executed**
>> - … including **re-translating** lines inside a loop on every pass
>> - The compiler may also **optimise** the object code during translation
>>
>> *Inference: 9618 credits "runs faster" as a single point but has never asked why. A 2-mark point-plus-expansion is the standard form.*

---

## 5.2.3 Programs partially compiled and partially interpreted

> [!question] 9618 | State a reason why some high-level languages are partially compiled and partially interpreted [2]
> State a reason why some high-level language programs are partially compiled and partially interpreted.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The source is compiled into an **intermediate code**, not machine code
>> - … which is then interpreted by a **virtual machine** on the target computer
>> - This makes the program **platform independent** — the same intermediate code runs anywhere
>> - … while still running **faster** than interpreting the original source directly
>>
>> *Latest: `9618_w25_qp_12_sc_6.c`*

> [!question] Inferred | Describe how partial compilation and interpretation works [4]
> Describe how a program that is partially compiled and partially interpreted is translated and executed.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The source code is **compiled** into an **intermediate / byte code**
>> - … this happens once, on the developer's machine
>> - The intermediate code is **not machine code**, so the processor cannot execute it directly
>> - It is distributed to users and **interpreted at run time** by a **virtual machine**
>> - Each platform has its own virtual machine, so the **same file runs on any of them**
>> - Much of the translation work is already done, so it runs faster than pure interpretation
>>
>> *Inference: 9618 asks only for a *reason* at 2 marks; the mechanism itself has not been asked, and 9618 marks comparable mechanism questions at 4.*

> [!question] Inferred | Explain the use of a virtual machine with a named language [3]
> Java programs are partially compiled and partially interpreted. Explain how this allows a Java program to run on different computers.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The Java source is compiled into **bytecode**
>> - The bytecode is the same whatever computer will run it
>> - Each platform has a **Java Virtual Machine (JVM)**
>> - The JVM **interprets** the bytecode into that machine's own machine code
>> - … so the program is **written once and runs anywhere**, with no recompilation
>>
>> *Inference: 9618 has never named a language in this bullet, but the syllabus wording invites it and 9618 routinely sets a named-scenario version of an abstract bullet at 3 marks.*

> [!question] Inferred | State the drawbacks of the hybrid approach [2]
> State two drawbacks of a program that is partially compiled and partially interpreted.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **virtual machine must be installed** on every computer that runs the program
>> - Execution is **slower than fully compiled** code, because the bytecode is still interpreted
>> - It uses **more memory**, since the virtual machine runs alongside the program
>> - The bytecode can be **decompiled** more easily than machine code
>>
>> *Inference: 9618 has asked only for the benefit. The drawback mirror is the standard follow-up, at 2 marks.*

---

## 5.2.4 Features found in a typical Integrated Development Environment (IDE)

> [!question] 9618 | Identify one common IDE feature for each purpose and describe it [6]
> For each of three purposes — writing code, presenting code and debugging code — identify one feature of a typical IDE and describe it.
>
>> [!success]- Answer — 2 marks per feature (name + description), 6 marks
>> - **Coding / context-sensitive prompts** — as the programmer types, the IDE suggests keywords, variable names and parameters
>> - **Dynamic syntax check** — the IDE checks each line as it is typed and highlights errors immediately
>> - **Prettyprint / presentation** — keywords, variables, strings and comments are shown in different colours and fonts, and code is automatically indented
>> - **Expand and collapse** — blocks of code can be hidden so the overall structure is visible
>> - **Single stepping** — the program is run one line at a time so the programmer can watch what happens
>> - **Breakpoints** — execution stops at a chosen line so the program's state can be examined
>> - **Variable / watch window** — shows the current value of each variable as the program runs
>> - **Report window** — lists the errors found, with their line numbers
>>
>> *Latest: `9618_w25_qp_13_sc_6.a`*

> [!question] 9618 | Describe how programmers use the debugging features of a typical IDE [4]
> Describe how a programmer uses the debugging features of a typical IDE.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Single stepping** runs the program one line at a time
>> - … so the programmer can see exactly where the behaviour goes wrong
>> - **Breakpoints** stop execution at a chosen line
>> - … so the program's state at that point can be examined without stepping through everything
>> - A **variable / watch window** shows the current value of each variable as the program runs
>> - The **report window** lists errors with their line numbers so they can be located and corrected
>>
>> *Latest: `9618_s25_qp_11_sc_5.c`*

> [!question] 9618 | Describe two named IDE features [4]
> Describe two named features of a typical Integrated Development Environment.
>
>> [!success]- Answer — 2 marks per feature, 4 marks
>> - **Context-sensitive prompt** — offers suggestions as the programmer types … reducing typing errors and the need to memorise syntax
>> - **Dynamic syntax check** — checks the line as it is entered … so syntax errors are flagged immediately rather than at compilation
>> - **Prettyprint** — colours and indents the code … making its structure easier to read
>> - **Breakpoint** — halts execution at a chosen line … so the values of variables can be inspected at that point
>>
>> *Latest: `9618_w24_qp_12_sc_4.b`*

> [!question] 9618 | Complete a table describing typical IDE features [4]
> Complete the table by describing each feature of a typical IDE.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Single stepping** → executes the program one line at a time
>> - **Breakpoint** → stops the program at a chosen line
>> - **Variable window** → displays the current value of variables during execution
>> - **Report window** → lists the errors found, with line numbers
>> - **Expand / collapse** → hides or reveals blocks of code
>> - **Auto-indent / prettyprint** → formats and colours the code to show structure
>>
>> *Latest: `9618_s24_qp_13_sc_6.a`*

> [!question] 9618 | Identify and describe one other presentation feature [2]
> Other than the one given, identify and describe one presentation feature of a typical IDE.
>
>> [!success]- Answer — name + description, 2 marks
>> - **Colour coding / syntax highlighting** — keywords, strings, comments and variables are shown in different colours so they can be told apart at a glance
>> - **Automatic indentation** — the IDE indents each block so the program's structure is visible
>> - **Expand and collapse** — sections of code can be hidden to show the overall structure
>> - **Line numbering** — every line is numbered so errors can be located from the report window
>>
>> *Latest: `9618_w23_qp_12_sc_5.b.ii`*

> [!question] 9618 | Identify and describe one other debugging feature [2]
> Other than the one given, identify and describe one debugging feature of a typical IDE.
>
>> [!success]- Answer — name + description, 2 marks
>> - **Breakpoint** — execution halts at a chosen line so the state of the program can be examined
>> - **Single stepping** — the program is run one line at a time so the effect of each line can be seen
>> - **Variable / watch window** — shows the value of each variable as the program runs
>> - **Report / error window** — lists the errors found together with their line numbers
>>
>> *Latest: `9618_w23_qp_12_sc_5.b.i`*

> [!question] 9618 | Identify two presentation features of an IDE [2]
> Identify two presentation features found in a typical IDE.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Prettyprint / syntax colour coding**
>> - **Automatic indentation**
>> - **Expand and collapse** of code blocks
>> - **Line numbering**
>>
>> *Latest: `9618_s23_qp_12_sc_6.a.i`*

> [!question] 9618 | Identify two debugging features of an IDE [2]
> Identify two debugging features found in a typical IDE.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Single stepping**
>> - **Breakpoints**
>> - **Variable / watch window**
>> - **Report window listing errors**
>>
>> *Latest: `9618_s23_qp_12_sc_6.a.ii`*

> [!question] 9618 | Identify three tools that support the writing of a program [3]
> Identify three features of a typical IDE that support the **writing** of program code.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Context-sensitive prompts / auto-complete**
>> - **Dynamic syntax checking** as the code is typed
>> - **Initial error detection**, flagging mistakes before compilation
>> - A **built-in editor** with line numbering and auto-indent
>> - **Built-in translators**, so code can be compiled or run from within the IDE
>>
>> *Latest: `9618_w22_qp_13_sc_6.a`*

> [!question] Inferred | Explain how dynamic syntax checking helps a programmer [3]
> Explain how the dynamic syntax checking feature of an IDE helps a programmer.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Each line is checked **as it is typed**, not when the program is compiled
>> - Errors are **highlighted immediately**, usually by underlining the offending text
>> - … so the programmer corrects them while the line is still fresh in mind
>> - Fewer syntax errors reach **compilation**, so the error report is shorter
>> - It reduces the time spent on repeated compile-and-fix cycles
>>
>> *Inference: named in the syllabus and credited inside table answers, but never the subject of its own 9618 question; comparable "explain how this feature helps" questions carry 3.*

> [!question] Inferred | Describe the built-in translators of an IDE as a feature [2]
> Describe how the translators built into an IDE support a programmer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The IDE contains **both an interpreter and a compiler**
>> - The **interpreter** lets the programmer run and test code while it is still being written
>> - The **compiler** produces the executable once the program is complete
>> - … so the programmer never has to leave the IDE to translate the program
>>
>> *Inference: the syllabus lists built-in translators among IDE features, and it is credited in the 3-mark "writing tools" mark scheme, but no question has targeted it.*

> [!question] Inferred | Explain why a programmer uses an IDE [3]
> Explain why a programmer would use an Integrated Development Environment rather than a simple text editor.
>
>> [!success]- Answer — 5 points for 3 marks
>> - All the tools needed — editor, translator and debugger — are in **one program**
>> - Errors are caught **as the code is typed**, so fewer reach compilation
>> - **Prettyprint and indentation** make the code easier to read and maintain
>> - **Debugging tools** such as breakpoints and the variable window make faults easier to find
>> - The overall effect is **faster development with fewer errors**
>>
>> *Inference: every 9618 question asks for features; none asks for the rationale. A 3-mark "explain why" is the obvious untested angle on the chapter's most examined bullet.*

> [!question] SME | List the IDE features under their four headings [6]
> State the features of a typical IDE under the headings: coding, initial error detection, presentation and debugging.
>
>> [!success]- Answer — 8 points for 6 marks
>> - **Coding** — context-sensitive prompts / auto-complete
>> - … built-in editor with line numbering, auto-indent and auto-correct
>> - **Initial error detection** — dynamic syntax checks as each line is typed
>> - … errors highlighted or underlined before compilation
>> - **Presentation** — prettyprint: colour coding of keywords, strings and comments
>> - … expand and collapse of code blocks to show structure
>> - **Debugging** — single stepping, breakpoints
>> - … variable / watch window and a report window listing errors with line numbers
>>
>> *These four headings are the syllabus's own; SME organises the notes this way and 9618's 6-mark IDE question is the largest tariff in the chapter.*
