---
title: Jigsaw — 4 Processor Fundamentals (AS Level)
syllabus: 9618 (2026)
topics: 4.1 CPU Architecture · 4.2 Assembly Language · 4.3 Bit manipulation
---

# Jigsaw — 4 Processor Fundamentals

Syllabus content for **9618 Topic 4**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers.

> [!danger] 4.3 Bit manipulation is new in 9618
> The 9608 Legend's Bit manipulation file is **two pages with no questions at all**. Bit manipulation is 9618-only, like AI and embedded systems — and it is examined **every single series**, usually as part of the big assembly question. There is no old-syllabus safety net.

---

# 4.1 Central Processing Unit (CPU) Architecture

## 4.1.1 The Von Neumann model and the stored program concept

> [!success] Correct incorrect statements about the Von Neumann model
> The PC stores the **address of** the next instruction to be fetched (not the instruction itself) · the CU sends signals to other components on the **control** bus (not the data bus) · the MDR **holds data to be stored in**, or **data read from**, the memory address in the MAR (it does not "transfer data to" it). `9618_s25_qp_12_sc_1.a`

> [!success] Identify components of the Von Neumann model
> Other than registers and buses: **Control Unit (CU)** · **Arithmetic and Logic Unit (ALU)** · **Immediate Access Store (IAS)** · system clock. `9618_w23_qp_13_sc_9.a.i`

> [!success] State what is meant by the stored program concept [1]
> Instructions **and** data are stored in the **same** memory space // in main memory. `9618_w22_qp_11_sc_5.a`

> [!info] Why the stored program concept matters
> 9618 has only ever asked for the one-line definition. What it *enables* — a computer that can run any program without being rewired, programs treated as data so they can be loaded and replaced — has never been asked, in either series.

> [!abstract] The model in one paragraph
> Proposed by John Von Neumann in the 1940s; most general-purpose computers are built on it. It consists of a **CPU able to access memory directly**, **memory that stores programs as well as data**, and **stored programs containing instructions executed in order**. The framing "the CPU can access memory directly" is the part the mark schemes never state.

---

## 4.1.2 Registers: purpose, role, and general vs special purpose

> [!success] Describe the purpose of each named register (table)
> **PC** — stores the address of the next instruction to be fetched/executed · **MAR** — stores the address of the memory location where data will be read from or written to · **MDR** — stores the data read from the address in the MAR, or the data to be written to it · **IX** — stores a number that will be added to the operand to form the address of the data. `9618_w24_qp_12_sc_3.a` (4 marks, 1 each)

> [!success] Identify two other special purpose registers and state their roles [4]
> **PC** — stores the address where the **next** instruction is to be read from · **MAR** — stores the address of the memory location (or I/O component) currently being read from or written to · **CIR** — holds the instruction currently being decoded and/or executed · **Status Register** — contains bits which can be referenced individually and set or cleared depending on the operation, e.g. overflow, underflow. `9618_w23_qp_11_sc_5.a`

> [!success] Describe the purpose of the Status Register (SR) [2]
> To store the value of **flags / bits** · that can be changed / set / cleared after **arithmetic or logical operations** · to allow flags to be checked · to change the instruction sequence. `9618_w24_qp_11_sc_8.a`

> [!success] Two differences between general purpose and special purpose registers [2]
> Special purpose registers have a **specified role** in the machine, whereas general purpose registers can be used for **any purpose** defined by the programmer · special purpose registers hold the **state of the program's execution**, general purpose registers hold the program's **data** during operations · general purpose registers can be used by most instructions, special purpose only by certain instructions. `9618_w24_qp_11_sc_8.b`; `9618_w23_qp_13_sc_9.a.ii`

> [!success] Describe the role of the ACC and the CIR [2]
> **ACC** — stores the intermediate results of arithmetic and logical operations // holds the result of a calculation · **CIR** — holds the instruction currently being decoded and/or executed. `9618_w25_qp_11_sc_6.a`

> [!success] Identify one other register used in the F-E cycle and describe its role [2]
> **CIR** — to store the instruction to be decoded/executed next · **Status register** — to contain bits that can be referenced individually to indicate a state or event · **Interrupt register** — to store details of any interrupts that have occurred. `9618_s25_qp_12_sc_1.b`

> [!info] The **interrupt register**
> Credited as an acceptable answer in `s25_qp_12_sc_1.b` and `w21_qp_12_sc_8.a.ii`, but it is **not in the syllabus's list of special purpose registers** (PC, MDR, MAR, ACC, IX, CIR, Status). Safe to offer as "one other register", but lead with a syllabus-named one.

> [!info] The Index Register described rather than named
> IX appears in the `w24_qp_12_sc_3.a` table and in every indexed-addressing question, but no question asks *why* an index register exists — to step through an array or table by changing one register rather than rewriting the instruction. That link between 4.1 and 4.2 is untested.

> [!abstract] The seven registers, with acronym and purpose
> **PC** holds the address of the next instruction and increments as the cycle runs · **MAR** holds the address data or instructions are fetched from · **MDR** stores the data/instruction fetched from memory · **CIR** stores the instruction currently being decoded or executed · **ACC** stores the results of calculations from the ALU · **IX** stores a value added to an address to get the effective address, used for indexed addressing · **SR** stores flags reflecting the outcome of CPU operations.
> SME's framing that registers are "extremely small, extremely fast memory located in the CPU" is the one-line definition the mark schemes assume but never state.

---

## 4.1.3 The ALU, Control Unit, system clock and Immediate Access Store

> [!success] Explain how the CU and the system clock work together [2]
> The control unit **synchronises** the actions of the processor · by sending a command / signal on **each timing signal** produced by the system clock · using the **control bus**. `9618_s25_qp_13_sc_2.a.i`

> [!success] Explain how the CU, system clock and control bus transfer data [4]
> The **system clock** gives out **timing** signals · which are sent on the **control bus** · to **synchronise** the other system components · the **Control Unit** initiates data transfer · by generating signals that are sent on the control bus to other components. `9618_s23_qp_13_sc_7.b`

> [!success] State the purpose of the system clock and the Control Unit [2]
> **System clock:** to synchronise operations, by creating and transmitting timing signals on the control bus; to keep track of the date and time; to process operations in the correct sequence. **Control Unit:** sends and receives control signals along the control bus; reads an instruction from the memory location whose address is in the PC; coordinates/synchronises the activity of other CPU components; manages the execution of instructions; controls communication between CPU components. `9618_w24_qp_11_sc_3.a`; `9618_w22_qp_13_sc_4.b`; `9618_w22_qp_11_sc_5.b.iii`

> [!success] Describe what is meant by the Immediate Access Store (IAS) [2]
> Holds all the data / instructions / programs **currently in use** · is **volatile** memory · has **fast access times**. `9618_w23_qp_11_sc_5.b`

> [!success] Complete a cloze on internal components [5]
> The **control unit/bus** transmits the signals to coordinate events based on the pulses of the **(system) clock**. The **data bus** carries data to components, while the **address bus** carries the address where data is being written to or read from. The **arithmetic logic unit / ALU** performs mathematical operations and logical comparisons. `9618_s21_qp_12_sc_5.a`

> [!info] The ALU on its own
> The ALU is named in the component list and in the cloze, but **no 9618 question asks you to describe its role**. Compare the CU (asked three times) and the system clock (twice). "Describe the purpose of the ALU" — performs arithmetic operations (add, subtract) and logical operations (AND, OR, comparisons), with the result placed in the ACC and flags set in the SR — is an obvious 2-marker.

> [!info] IAS versus RAM versus cache
> `w23_qp_11_sc_5.b` credits "volatile, fast access, holds what is currently in use" — which is also true of RAM. Whether the IAS *is* main memory, and how it relates to cache and registers, has never been examined.

---

## 4.1.4 Data transfer using the address, data and control buses

> [!success] Identify two types of signal a control bus can transfer [2]
> Interrupt · timing · read · write. `9618_s23_qp_12_sc_5.a`

> [!success] Tick which bus each CPU component uses [1]
> System clock → **control bus** · MAR → **address bus**. `9618_w22_qp_11_sc_5.b.ii`

> [!success] Describe the roles of the address bus, data bus and buffers when writing to a device [3]
> **Buffers** — temporarily hold data until it is ready to be transmitted to the device · **Address bus** — the address of the data to be written to the device (in RAM) is carried on the address bus · **Data bus** — all data to be written to the device/buffer is carried on the data bus. `9618_w23_qp_12_sc_8.c.ii`

> [!success] Explain how different bus widths affect performance [2]
> A **wider data bus** means more data can be transferred between components at a time · so there is less delay / latency when fetching data for a running process · a **wider address bus** means larger memory addresses can be used · allowing more memory locations to be accessed directly · so it is less likely to run out of memory. `9618_s25_qp_11_sc_6.a.iii`

> [!info] Which buses are **unidirectional**
> Every mark scheme describes what each bus *carries*, but none asks about direction. The address bus is **unidirectional** (CPU → memory); the data and control buses are **bidirectional**. This is standard credited content in other syllabuses and follows directly from what each bus does.

> [!info] Calculating addressable memory from address bus width
> `s25_qp_11_sc_6.a.iii` credits "larger memory addresses can be used, allowing more memory locations to be accessed". The numeric version — an *n*-bit address bus can address 2ⁿ locations — has never been asked in this topic, though the same arithmetic appears in Chapter 1.

> [!abstract] What a bus actually is
> A bus is a **set of parallel wires** through which data or signals are transmitted between components. **Address** — unidirectional, carries the location that is being written to or read from · **Data** — bidirectional, carries data or instructions · **Control** — bidirectional, carries commands and control signals telling components when to read or write. The "parallel wires" definition and the directionality are absent from every mark scheme in this topic.

---

## 4.1.5 Factors contributing to the performance of the computer system

> [!success] Explain why increasing clock speed and cache memory improves performance [4]
> **Clock speed:** the processor can perform more F-E cycles per second … so more instructions/data can be processed each second. **Cache memory:** can store more of the most frequently used instructions … which reduces the need to access slower RAM. *(Max 2 each.)* `9618_w25_qp_12_sc_3.c`

> [!success] Describe two hardware upgrades and explain how each improves performance [4]
> Increase the **number of cores** … each core can **independently** carry out a process at the same time, so more instructions are performed **in parallel** · increase **RAM capacity** … allowing more applications to reside in memory at once, saving disk access times · increase **cache memory** … more data can be stored in fast access, so less time is spent accessing RAM · increase **clock speed** … more F-D-E cycles can run per unit time. `9618_s23_qp_12_sc_5.b`; `9618_w22_qp_13_sc_4.c`

> [!success] Explain why a dual-core CPU is not always twice as fast [5]
> Multiple cores introduce **additional overheads** … because of the need for communication between cores · software may not be designed for multiple cores … so one of the cores will be left **idle** · memory access speed may not match the speed of the cores … causing delay · the two computers may differ in more than the cores — one may have more RAM allowing faster multitasking, or a GPU. `9618_w23_qp_11_sc_5.c.ii`

> [!success] Describe the drawbacks of increasing the number of cores [2]
> **Latency may be increased** … because the cores must communicate with one another · there is a potential for **dead-lock** situations … where one core waits for information from other cores which are waiting for the first · not all software is designed to use multi-cores … so some additional cores would be idle · **increased heat generation** … which could damage other components. `9618_w25_qp_11_sc_6.b`

> [!success] Describe how the number of cores and the clock speed affect performance [4]
> **Cores:** each core processes one instruction per clock pulse; multiple cores mean sequences of instructions can be **split between them**, so more than one instruction is executed per clock pulse; more cores decreases the time taken to complete a task. **Clock speed:** each instruction is executed on a clock pulse // one F-E cycle runs on each clock pulse, so the clock speed dictates the number of instructions run per second. *(Max 3 per factor.)* `9618_s21_qp_12_sc_5.b`

> [!success] Describe one benefit of cache memory [2]
> Cache is **fast access memory close to the CPU** · which stores frequently used instructions / data · so they can be accessed faster than from RAM · more cache means less swapping between RAM and cache · prevents the CPU idling while waiting for data. `9618_s25_qp_13_sc_2.b`; `9618_w22_qp_11_sc_7.d`

> [!success] Explain how different amounts of RAM affect performance [3]
> More RAM means more currently running data and instructions can be stored · **without needing to use virtual memory** · without having to fetch data from secondary storage first · which has a slower access time · less latency / delay waiting for instructions or data. `9618_s25_qp_11_sc_6.a.ii`

> [!success] Identify one feature of a processor that affects performance and state why [2]
> Clock speed — higher clock speed means more F-E cycles executed per second // more throughput · bus width — a larger bus width means more data transferred at the same time. `9618_w24_qp_11_sc_3.b.i`

> [!info] **Processor type** as a named factor
> The syllabus notes say "processor **type** and number of cores". Every 9618 question examines cores, clock speed, cache and bus width; the *type* of processor (e.g. a GPU for graphics work, a low-power processor in an embedded device, instruction-set differences) is never asked, despite being the first item in the notes.

> [!info] Diminishing returns on cache
> The mark schemes treat "more cache is better" as always true. Why cache is small and expensive — it is SRAM (Chapter 3) — and why a bigger cache gives diminishing returns, is the link between the two chapters and is untested.

> [!abstract] Cache levels
> **L1** inside each CPU core — fastest, smallest · **L2** inside or near each core — fast, medium · **L3** shared by all cores — slower than L1/L2, largest. Not named in any 9618 mark scheme, but explains why "cache is close to the CPU" is the credited reason it is fast.

> [!abstract] The throughput arithmetic
> A quad-core CPU at 3 GHz gives 4 × 3 billion = 12 billion instructions per second as an upper bound. SME's caveat matches the `w23_qp_11_sc_5.c.ii` mark scheme exactly: a dual-core is not twice as fast because time is spent **organising tasks between cores**, and some tasks are **sequential** and must be done step by step.

---

## 4.1.6 How different ports provide connection to peripheral devices

> [!success] Identify a port and explain how it provides an automatic connection [3]
> Port: **USB**. Explanation: a **voltage change** occurs when the drive is plugged in · the computer detects this voltage change · the **code of the device** is transferred to the computer · the OS finds the code of the device in its list of devices · and loads the appropriate **device driver**. `9618_w24_qp_11_sc_3.b.ii`

> [!success] Explain the benefits of HDMI instead of VGA [4]
> HDMI has **faster transfer rates** than VGA … needed for the high resolution / large number of pixels of the monitor · HDMI supports **video and audio** transfer on one cable … so no separate sound cable is needed, unlike VGA · HDMI is a **digital** interface, so no data is lost converting to analogue and back · HDMI is less prone to error / crosstalk / external interference. `9618_w24_qp_12_sc_3.b`

> [!success] Explain how HDMI provides connection to peripheral devices [2]
> Transfers both audio and video using a single cable · has high bandwidth · data is transmitted in a stream · of **uncompressed digital signals** · uses **Transition-Minimized Differential Signalling (TMDS)**. `9618_s25_qp_13_sc_2.c`

> [!success] Identify a port for a device and justify the choice [3]
> **USB** — fast data transfer speeds; is a universal / popular standard. **HDMI** — allows video and audio to be transferred on the same cable; convenience, as no need for two cables. `9618_w23_qp_13_sc_7.d`

> [!success] Describe how data is transmitted through a USB port [1]
> **1 bit is transferred at a time** (serial) · can be synchronous **or** asynchronous · USB-3 is full duplex and earlier versions are half-duplex. `9618_s23_qp_12_sc_5.c.i`

> [!success] Name a port for a given peripheral [2]
> 3D printer → USB port / COM port · Monitor → HDMI / VGA / USB / DisplayPort · Optical disc reader/writer → USB / HDMI. `9618_w22_qp_11_sc_7.e`; `9618_w23_qp_12_sc_8.c.i`

> [!info] **VGA** described in its own right
> VGA is named in the syllabus notes and appears only as the *loser* in the HDMI comparison. What VGA actually is — an **analogue** video-only interface, so audio needs a separate cable and the signal degrades over distance and with conversion — has never been asked directly.

> [!info] Why a port needs a device driver
> The driver appears in `w24_qp_11_sc_3.b.ii` and in the OS hardware-management mark schemes (Chapter 5), but the connection between the two — the port detects the device, the OS loads the driver so the two can communicate — is never the subject of a question.

> [!abstract] USB detail worth having
> USB is a **serial**, **asynchronous** standard. Connector types: **USB-A** (flash drives, mice, keyboards), **USB-B** (printers, scanners), **USB-C** (small, fast, carries power). Generations: USB 1.1 ≈ 12 Mbps, USB 2.0 ≈ 480 Mbps, USB 3.x ≈ 5–20 Gbps, USB4 up to 80 Gbps.
> **Advantages:** automatic detection and driver loading; connectors fit only one way, preventing incorrect connection; widely standardised so support is easy to find; several transmission rates supported; **backwards compatible** with older standards.
> **Disadvantages:** maximum cable length around 5 m, so unusable over long distances; older versions have limited transfer rates; very old standards may lose support.
> The backwards-compatibility and cable-length points are absent from every mark scheme and are exactly what a "justify the port choice" answer needs.

---

## 4.1.7 Stages of the Fetch-Execute cycle, and register transfer notation

> [!success] Write the stages of the F-E cycle in register transfer notation [4]
> `MAR ← [PC]` · `PC ← [PC] + 1` · `MDR ← [[MAR]]` · `CIR ← [MDR]` — plus **1 mark for the correct order**. The first two may be combined as `MAR ← [PC] and PC ← [PC] + 1`. `9618_s25_qp_13_sc_2.a.ii`

> [!success] Complete a table of F-E steps and their descriptions [4]
> `PC ← [PC] + 1` ↔ the address in PC is incremented · `MDR ← [[MAR]]` ↔ the **data in the location pointed to by the MAR** is copied to the MDR · `MAR ← [PC]` ↔ the **contents** of PC are copied to the MAR · `CIR ← [MDR]` ↔ the contents of MDR are copied into CIR. `9618_w23_qp_13_sc_9.b`

> [!success] Write the RTN for each described stage [3]
> Copy the address of the next instruction into the MAR → `MAR ← [PC]` · increment the Program Counter → `PC ← [PC] + 1` · copy the contents of the MDR into the CIR → `CIR ← [MDR]`. `9618_w22_qp_12_sc_7.c`; `9618_s23_qp_13_sc_7.c`

> [!success] Identify and correct errors in given register transfer notation [4]
> Line `PC ← [PC] − 1` → the Program Counter should be **incremented, not decremented** → `PC ← [PC] + 1` · line `MDR ← [MAR]` → it should be the **contents of the address in** the MAR → `MDR ← [[MAR]]`. *(1 mark for line + description, 1 for the correct statement.)* `9618_w21_qp_11_sc_6.a`

> [!success] Describe the role of the MAR and MDR in the F-E cycle [4]
> **MAR** stores the **address** of the next instruction / data to be read from or written to memory · the address is received from the **PC** · **MDR** stores the data / instruction at the address in the MAR which has been read or written · the instruction passes to the **CIR** for decoding and executing. `9618_w25_qp_13_sc_6.b`; `9618_w21_qp_12_sc_8.a.i`

> [!success] Complete a cloze describing the registers in the F-E cycle [5]
> The **Program Counter** holds the address of the next instruction to be loaded. This address is sent to the **Memory Address Register**. The **Memory Data Register** holds the data fetched from this address. This data is sent to the **Current Instruction Register** and the CU decodes the opcode. The **Program Counter** is incremented. `9618_s21_qp_11_sc_3.a`

> [!info] The **execute** stage in RTN
> Every 9618 question stops at `CIR ← [MDR]` — that is, the **fetch** only, despite the bullet being titled "the stages of the Fetch-Execute cycle". The decode and execute stages in RTN (e.g. `MAR ← operand`, `MDR ← [[MAR]]`, `ACC ← [MDR]` for an LDD) have never been asked, and the syllabus says "describe **and use** register transfer notation to describe the F-E cycle".

> [!info] The **decode** stage described
> The CIR splitting the instruction into **opcode and operand**, and the CU decoding it, appears once as a cloze mark point (`s21_qp_11_sc_3.a`). A question asking what happens during decode has not been set.

> [!abstract] The three stages, and what happens where
> **Fetch** — supply the address and receive the instruction from memory. **Decode** — interpret the instruction and retrieve any required data from their addresses. **Execute** — the CPU carries out the required action.
> SME's execute examples in RTN (LDA, STA, ADD) are the content for the `!info` gap above: for `LDA X`, `MAR ← operand` then `MDR ← RAM[MAR]` then `ACC ← MDR`; for `STA X`, `MAR ← operand` then `MDR ← ACC` then `RAM[MAR] ← MDR`.

---

## 4.1.8 The purpose of interrupts

> [!success] Explain how the computer handles an interrupt [5]
> An **interrupt flag** is raised in the (interrupt) register · at the **end of the current F-E cycle** // at the start of the next F-E cycle · the system checks the interrupt register for interrupts of **higher priority** than the current process · if true, it stores the current contents of the registers **on the stack** · the appropriate **Interrupt Service Routine (ISR)** is called · the input data is processed · the contents of the registers are **restored from the stack** · and control is passed back to the previous process. `9618_s23_qp_11_sc_6`

> [!success] Explain how an interrupt is detected and handled in the F-E cycle [4]
> At the start / end of the F-E cycle the **interrupt register is checked** · the **priority** of any interrupts waiting is checked · if the priority of the interrupt is higher than the current process · the contents of the registers are **stored on the stack** · the relevant **ISR / interrupt handler** is called to process the interrupt · when the ISR has finished, a further check is made for higher priority interrupts · if none, the register contents are restored and the next F-E cycle continues. `9618_s25_qp_12_sc_1.c`

> [!success] Order the stages the CPU performs when an interrupt is detected [3]
> 1 At the end of each F-E cycle the processor checks if an interrupt flag is set → **2 D**: the processor identifies the source of the interrupt and checks its priority → 3 If the priority is high enough the processor saves the current register contents → **4 A**: the address of the ISR is loaded into the PC → 5 When servicing is complete the processor restores the registers → **6 B**: lower priority interrupts are re-enabled. `9618_w23_qp_13_sc_9.d`

> [!success] State when interrupts are detected during the F-E cycle [1]
> **After completion of the execute stage** // before the cycle begins. `9618_w22_qp_13_sc_4.a.ii`

> [!success] Describe the purpose of an interrupt [2]
> To **send a signal** from a device or process · seeking the **attention of the processor**. `9618_w22_qp_11_sc_5.c`

> [!success] Identify causes of a software interrupt [2]
> Division by zero // runtime error in a program · attempt to access an invalid memory location // out of memory bounds · array index out of bounds · **stack overflow** · buffer overflow · program requesting an external device / input. `9618_w22_qp_11_sc_5.d`; `9618_w23_qp_13_sc_9.c`

> [!success] Tick whether each event is a hardware or a software interrupt [3]
> Buffer full → **software** · printer out of paper → **hardware** · user has pressed a key → **hardware** · division by zero → **software** · power failure → **hardware** · stack overflow → **software**. *(1 mark per pair of rows.)* `9618_w21_qp_12_sc_7.a`

> [!info] **Applications** of interrupts
> The syllabus notes list "possible causes of interrupts, **applications** of interrupts, use of an ISR, when interrupts are detected, how interrupts are handled". Causes, detection and handling are examined repeatedly; **applications** — what interrupts make possible, i.e. multitasking, responsive I/O without polling, real-time event handling — has never been asked. It is the one named sub-point with no question against it.

> [!info] Why interrupts are better than polling
> Implied by "seeking the attention of the processor" but never examined. Without interrupts the CPU would have to repeatedly check every device, wasting cycles.

> [!info] The **stack** in interrupt handling
> "Stores the register contents on the stack" and "restores from the stack" are credited mark points in two questions, but **why** a stack (so nested interrupts unwind in the right order) is never asked — even though `w23_qp_13_sc_9.d` includes re-enabling lower-priority interrupts, which only makes sense with nesting.

> [!abstract] The five-step interrupt process
> **1 Interrupt Request (IRQ)** — a device or software generates an interrupt; the interrupt controller passes it to the interrupt handler. **2 Acknowledge** — the handler decides whether to deal with it now or later; if now, the current register contents are saved. **3 ISR lookup** — the processor fetches the ISR associated with that interrupt type. **4 ISR execution** — control transfers to the ISR. **5 Interrupt exit** — registers are restored and the F-D-E cycle resumes.

> [!abstract] Priority and nesting
> **Prioritisation** lets the processor switch to a higher-priority interrupt; lower-priority ISRs may be suspended until it completes. **Nesting** is handling interrupts within interrupts; proper management avoids conflicts and keeps the system stable. This is the content behind the `w23_qp_13_sc_9.d` step "lower priority interrupts are re-enabled".

> [!abstract] Purpose and applications of interrupts — the untested bullet
> **Real-time event handling** — hardware errors and signals from input devices, e.g. hard disk failure · **Device communication** — alerts from external devices, e.g. printer jams, network errors · **Multitasking** — suspending one application so the user can switch to another.
> SME also names a third type alongside hardware and software: a **trap interrupt**, intentionally triggered by a program for debugging or handling unexpected errors. Traps are not in the 9618 syllabus, which names only hardware and software — do not offer one where the question asks for a type.

> [!abstract] What an ISR is
> A special routine that handles one particular interrupt type; each type has its own routine (printer jam, hard disk failure, network connection error). ISRs should be **concise and efficient**, because they often handle time-sensitive events. The "concise so as not to delay other work" point is not in any mark scheme.

---

# 4.2 Assembly Language

## 4.2.1 The relationship between assembly language and machine code

> [!success] Complete the description of language translators [4]
> **Compilers** are used when a high-level program is complete; they translate all the code at once and produce **executable / .exe / object code** files that run without the source code. **Interpreters** translate one line at a time and run it, useful while developing because errors can be corrected and the program continues from that line. **Assemblers** translate assembly code into **binary / machine code**. `9618_w21_qp_11_sc_4.d`

> [!info] The **one-to-one relationship**
> This bullet has **exactly one 9618 question**, and it is a cloze shared with Chapter 5. The defining fact — **one assembly language instruction translates to one machine code instruction**, unlike a high-level statement which becomes many — is not credited anywhere in the 9618 series and is the most likely content for a new question on this bullet.

> [!info] Why anyone still writes assembly
> Untested in 9618: direct control of hardware, minimal memory footprint, speed of execution, and use in embedded systems and device drivers — which links straight to embedded systems in Chapter 3.

> [!abstract] The two languages compared
> **Machine code** is a **first-generation language**, directly executable by the processor, written in binary. **Assembly** is a **second-generation language** written using **mnemonics** (abbreviated text commands), human-readable but corresponding almost exactly to machine code; it must be translated by an **assembler**, and **each CPU type has its own instruction set**.
> An instruction splits into an **opcode** (what operation to perform) and an **operand** (the data or memory address it works with).

---

## 4.2.2 The stages of the assembly process for a two-pass assembler

> [!success] Identify the purpose of the first pass [1]
> To **create a symbol table**. `9618_w23_qp_11_sc_8.a`

> [!success] Identify which pass each action takes place in [3]
> Generates object code → **second pass** · reads the source code one line at a time → **both passes** · removes white space → **first pass** · adds labels to the symbol table → **first pass**. `9618_s23_qp_12_sc_3.a`

> [!success] Tick whether each task is first pass or second pass [2]
> Remove comments → **first** · read the assembly language program one line at a time → **both** · generate the object code → **second** · check the opcode is in the instruction set → **first**. `9618_w22_qp_11_sc_6.c`

> [!info] What the **second pass** actually does
> All three 9618 questions are sorting exercises. None asks candidates to *describe* the second pass — replacing each label with the address stored against it in the symbol table, and converting each mnemonic into its binary opcode to generate the object code. The syllabus says "describe the different **stages**", so a prose question is available.

> [!info] Apply the two-pass process to a given program
> The syllabus notes say explicitly: *"Apply the two-pass assembler process to a given simple assembly language program."* **No 9618 question has ever required a symbol table to be built from a given program.** Every question is a tick-box or line-matching exercise. This is the clearest untested instruction in 4.2.

> [!info] Why **two** passes are needed
> Never asked in either series. The reason is forward references: a `JMP` to a label defined later in the program cannot be resolved until every label's address is known, which is what pass one establishes.

> [!abstract] A worked two-pass example
> Program: `LOAD A` / `ADD B` / `STORE C` / `HALT` / `A: DATA 5` / `B: DATA 3` / `C: DATA 0`.
> **Pass 1** assigns addresses and records labels, building the **symbol table**: A = 04, B = 05, C = 06. Instructions are not yet translated.
> **Pass 2** replaces each label with its address and outputs the object code: `01 04` / `02 05` / `03 06` / `00 00` / …
> The assembler produces an **object program** that can be stored, loaded and run later; **a loader is needed to execute it**. The loader is mentioned in no 9618 mark scheme and is the missing piece of "what the assembler produces".

---

## 4.2.3 Trace a given simple assembly language program

> [!success] Complete a trace table for an assembly program [6]
> Columns typically: instruction address · ACC · several memory addresses · IX · Output. **Marks are awarded per shaded *set* of values**, not per cell — so a single early error can lose a whole block. `9618_s24_qp_13_sc_3.a`-style; the 6-mark version is the largest in the topic.

> [!success] Write the contents of the ACC after each instruction [4]
> e.g. ACC `0000 1111`, `AND 101` → `0000 1110` · ACC `0000 0000`, `LDM #100` → `0110 0100` · ACC `0000 0001`, `XOR &F1` → `1111 0000` · ACC `0001 0001`, `CMP 101` → `0001 0001` (**CMP does not change the ACC** — the classic trap). `9618_w25_qp_13_sc_6.a`

> [!success] State the purpose of a fragment of assembly code [1]
> `LDD 100 / STO 165 / LDD 101 / STO 100 / LDD 165 / STO 101` → **swaps the contents of memory addresses 100 and 101**. `9618_w22_qp_11_sc_6.a.ii`

> [!success] State the effect of changing one instruction [1]
> Changing `LDD 10` to `LDM #10` → the **number 10** is loaded into the ACC instead of the **contents of address 10** · so the addition gives 20 not 22, the comparison fails and the result is an **infinite loop**. `9618_s25_qp_12_sc_7.a.ii`

> [!info] Writing, rather than tracing, an assembly program
> Every 9618 question gives you the program. The syllabus bullet is only "**trace** a given simple assembly language program", so this is correctly untested — but `s25_qp_13_sc_5.b` and `w24_qp_13_sc_7.b` do ask candidates to **write bit-manipulation instructions**, so writing short fragments is clearly within reach.

> [!abstract] Tracing technique
> A trace table tracks the values of variables (here, registers and memory locations) line by line. Because 9618 marks in **blocks**, work down the instruction-address column first and fill every register change on each row before moving on — and remember that `CMP` sets a flag but leaves the ACC unchanged, and that `JPE`/`JPN` depend on the **most recent** compare.

---

## 4.2.4 Instruction groups

> [!success] Complete statements naming the instruction group [3]
> Loading data into the accumulator → **data movement** · incrementing the index register → **arithmetic operations** · branching to another address → **conditional and unconditional (jump) instructions**. `9618_w25_qp_13_sc_6.c`

> [!success] Identify the instruction group for each opcode [4]
> `IN` → **input and output of data** · `ADD` → **arithmetic operations** · `JPE` → **unconditional and conditional instructions** · `CMI` → **compare instructions**. `9618_w23_qp_12_sc_9.a`

> [!success] Give an example instruction for each named group [3]
> Data movement: e.g. `LDR #50` // `STO 201` · Arithmetic operation: e.g. `ADD 100` // `INC IX` · Conditional instruction: e.g. `JPE 96`. **Each instruction must have a suitable operand.** `9618_w23_qp_11_sc_8.b.i`

> [!success] Write an appropriate instruction for each of the five groups [4]
> Data movement → `LDM #2` · Input and output → `IN` / `OUT` · Arithmetic → `INC ACC` / `INC IX` · Unconditional and conditional → `JPN 100` / `JMP 100` · Compare → `CMP 100`. `9618_w21_qp_12_sc_8.b.ii`

> [!success] Name one other instruction group [1]
> Input and output of data · arithmetic operations · unconditional and conditional instructions · compare instructions. `9618_w22_qp_13_sc_6.c`

> [!info] Why instructions are grouped at all
> Every question is naming or matching. The purpose of grouping — that the instruction set is organised by **function**, which makes the processor's capabilities systematic and the assembler's job of checking opcodes possible — is untested.

> [!info] `MOV` and `END`
> `MOV <register>` and `END` are in the syllabus instruction set but fit awkwardly into the five groups (`MOV` is data movement; `END` belongs to none cleanly). No question has asked about either, and no mark scheme classifies `END`.

---

## 4.2.5 Modes of addressing

> [!success] Identify and describe modes of addressing (table) [4]
> **Direct** — the operand **is the address of the data** · **Indirect** — the operand **points to the memory location which contains the address** of the data · **Indexed** — the address of the data is formed by **adding the contents of the Index Register (IX) to the operand** · **Immediate** — the operand is the data itself · **Relative** — the address is calculated using its **distance from a base address**. *(1 mark mode + 1 mark matching description.)* `9618_s25_qp_13_sc_5.a.ii`

> [!success] State what is meant by relative addressing [1]
> The value of the operand is an **offset value** which is added to another **base value** to give the address from which the contents are loaded to the accumulator. `9618_w25_qp_12_sc_3.a.i`

> [!success] Write the contents of the ACC after each instruction (addressing trace) [3]
> With memory 98→8, 99→16, 100→3, 101→98, 102→32 and IX = 2: `LDM #98` → **98** (immediate: the number itself) · `LDI 101` → **8** (indirect: address 101 holds 98, so load the contents of 98) · `LDX 100` → **32** (indexed: 100 + IX(2) = 102, so load the contents of 102). `9618_w25_qp_12_sc_3.b`

> [!success] Identify and describe one mode of addressing not in the given table [2]
> `9618_s25_qp_12_sc_7.a.iii`

> [!info] **Relative addressing used, not just defined**
> Relative is named in the syllabus notes and has been *defined* twice (`w25_qp_12_sc_3.a.i`, `s25_qp_12_sc_7.a.iii`). **No question has ever required a relative-addressed instruction to be traced**, unlike immediate, direct, indirect and indexed — partly because the standard instruction set has no relative opcode. Know the definition cold; the trace is unlikely.

> [!info] Why each mode exists
> The modes are described and traced, but never justified. Indexed addressing exists so one instruction can step through an array by changing IX; indirect exists so the address can be changed at run time. `w21_qp_12_sc_8` gets closest by combining IX with a loop, but the reasoning is never asked for.

> [!abstract] The five modes, with the mechanism stated plainly
> **Immediate** — the operand is a constant value included directly in the instruction · **Direct** — the exact memory address of the operand is given in the instruction · **Indirect** — a register or location contains the memory address of the operand · **Indexed** — uses a base address plus an index to calculate the memory address · **Relative** — the operand is an offset relative to the current instruction address, used in branching.

---

# 4.3 Bit manipulation

> [!danger] No 9608 questions exist for this entire sub-topic
> Everything below is 9618 or inference. Bit manipulation appears in **every 9618 series**, almost always attached to the assembly-language question.

## 4.3.1 Binary shifts: logical, arithmetic and cyclic; left and right

> [!success] Perform a logical shift [1]
> `01001111` left logical 2 → **0011 1100** · `11001100` right logical 3 → **0001 1001** · `11001010` left logical 2 → **0010 1000**. Zeros fill the vacated end. `9618_s25_qp_13_sc_7.a.i`

> [!success] Perform an arithmetic right shift on a two's complement negative integer [1]
> `10010011` arithmetic right 3 → **1111 0010** · `10011110` arithmetic right 3 → **1111 0011**. The **sign bit is copied** into the vacated leftmost bits. `9618_w25_qp_13_sc_2.c`; `9618_s25_qp_13_sc_7.a.ii`

> [!success] Show the result of an LSL / LSR instruction [1]
> `0110 1011` after `LSR #5` → **0000 0011** · `0101 0011` after `LSL #3` → **1001 1000** · `1001 0011` after `LSR #2` → **0010 0100**. `9618_s25_qp_11_sc_8.b.iii`

> [!success] Describe the difference between a right logical and a right arithmetic shift [2]
> A **logical** shift moves all bits to the right and **inserts zeros** in the appropriate leftmost bits · an **arithmetic** shift moves all bits to the right but **copies the sign bit into the Most Significant Bit**. `9618_w24_qp_13_sc_8.c`

> [!success] Write a bit manipulation instruction that produces a given result [1]
> ACC `0001 1110` → `0111 1000` requires **`LSL #2`**. `9618_w25_qp_11_sc_4.a`

> [!info] **Cyclic shifts**
> The syllabus notes name **"logical, arithmetic and cyclic"**. Logical shifts are examined every series and arithmetic shifts twice in w25/s25 — **cyclic shifts have never been examined in 9618**, and there is no 9608 fallback. There is also no cyclic opcode in the standard instruction set, so it would have to be asked as a written shift, e.g. "show the result of a 3-place cyclic left shift on 10110001". This is the single clearest gap in Chapter 4.

> [!info] Shifts as multiplication and division
> Never asked in 9618. Each left shift **doubles** the value; each right shift **halves** it. An arithmetic right shift divides a signed number by 2 while preserving the sign. A question asking *why* a shift is used instead of a multiply instruction (it is far faster) is available and would test understanding rather than mechanics.

> [!info] What is **lost** in a shift
> Bits shifted off the end are discarded, so a left shift can overflow and a right shift can lose precision. `w25_qp_11_sc_4.a` requires a shift that happens not to lose a 1 bit; a question where it does has not been set.

> [!abstract] The three shift types, side by side
> **Logical** — moves bits and fills the gap with 0s; used for unsigned numbers or raw bit manipulation.
> **Arithmetic** — left is the same as logical left; **right copies the sign bit (MSB)** into the new leftmost bit, preserving the sign for two's complement numbers.
> **Cyclic** — rotates the bits around; **nothing is lost and no 0s are added** — the bit that falls off one end reappears at the other.
> Worked: `0000 1110` (14) left 2 → `0011 1000` (56), doubling each time. `1100 1000` (200) right 3 → `0001 1001` (25), halving each time. `1110 1000` (−24) arithmetic right 3 → `1111 1101` (−3), rounding towards negative infinity.

---

## 4.3.2 Bit manipulation to monitor and control a device (masking)

> [!success] Write an instruction to **set** a specific bit to 1 [1–2]
> Set the **least significant** bit: `OR B00000001` // `OR #1` // `OR &1`. Set **only the most significant** bit in a register containing any 8-bit number, requires two instructions: `AND B00000000` then `OR B10000000` (accepted as `AND #0 / OR #128`, or `AND &0 / OR &80`). `9618_s25_qp_11_sc_8.b.i`; `9618_s25_qp_13_sc_5.b`

> [!success] Explain how bit manipulation can **clear** a register, and write the instruction [3]
> A bit manipulation operation is required to **set all the bits to zero** · compare the result of the masking with 0 · the result of the comparison will be true if the register is cleared · Instruction: **`AND B00000000`** / `AND #00` / `AND &00`. `9618_w24_qp_13_sc_7.b`

> [!success] Explain how bit manipulation can **test** a bit, and write the instruction [3]
> To test whether the number in the ACC is **odd**: an odd binary number will have a **1 in the Least Significant Bit** · a bit manipulation operation is required to **access/mask only the LSB and clear all the others** · compare the result of the masking with denary 1 · the result of the comparison will be true if the number is odd · Instruction: **`AND B00000001`** // `AND #1` // `AND &01`. `9618_w24_qp_12_sc_8.b.ii`

> [!success] Write the ACC contents after a bitwise instruction [1]
> `1111 0000` then `OR B00001111` → **1111 1111** · `0001 1101` then `XOR #30` → **0000 0011** · `0101 0101` then `XOR &FE` → **1010 1011**. `9618_s25_qp_12_sc_7.b.i`

> [!success] Complete a table of ACC contents after each set of instructions [3]
> With ACC reloaded to `1001 1010` each time: `LSL #2` → **0110 1000** · `ADD #5` then `AND #30` → **0001 1110** · `OR B11110010` then `INC ACC` → **1111 1011**. `9618_w24_qp_12_sc_8.b.i`

> [!success] Trace programs mixing masks and addresses [3]
> With ACC `1111 1111`: `LSL #2` → **1111 1100** · `XOR 100` (100 = `00001101`) → **1111 0010** · `AND 103` (103 = `00110111`) → **0011 0111**. `9618_s24_qp_13_sc_3.b`

> [!info] The **monitor/control device** context itself
> The bullet reads "show understanding of how bit manipulation can be used to **monitor/control a device**". Every 9618 question asks about an abstract 8-bit register — set a bit, clear a register, test for odd. **No question has placed the register in a device**, e.g. "each bit of this register corresponds to a sensor; write the instruction that tests whether sensor 3 has triggered", despite that being the literal wording and the obvious link to monitoring and control in Chapter 3.

> [!info] Using a mask to **clear one specific bit**
> Setting a bit (`OR`), clearing the whole register (`AND #0`) and testing a bit (`AND` + compare) have all been examined. Clearing **one** bit while leaving the others unchanged — `AND` with a mask of all 1s except a 0 in that position, e.g. `AND B11110111` — has not been asked, and is the natural fourth member of the set.

> [!info] **Flipping** a bit with XOR
> XOR appears constantly as a traced instruction, but no question asks candidates to *use* it purposefully — `XOR` with a 1 in one position toggles that bit and leaves the rest alone. Given that set, clear and test all have "explain and write the instruction" questions, toggle is the missing one.

> [!abstract] The three mask operations, as rules
> **OR** with a 1 **sets** that bit to 1; OR with a 0 leaves it unchanged. **AND** with a 0 **clears** that bit to 0; AND with a 1 leaves it unchanged. **XOR** with a 1 **flips** that bit; XOR with a 0 leaves it unchanged.
> The standard answer structure that the 9618 mark schemes reward is three-part: say which bit(s) matter · say that a mask is applied to isolate or change them · say that the result is **compared** with an expected value to give a true/false outcome. Then give the instruction.
