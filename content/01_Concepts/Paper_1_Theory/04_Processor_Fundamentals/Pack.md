---
title: Pack — 4 Processor Fundamentals (AS Level)
syllabus: 9618 (2026)
topics: 4.1 CPU Architecture · 4.2 Assembly Language · 4.3 Bit manipulation
pairs with: Jigsaw
---

# Pack — 4 Processor Fundamentals

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

> [!danger] This chapter has almost no 9608 safety net
> 9618 has rebuilt Topic 4 so thoroughly that the 9608 Legend contributes almost nothing usable here — and **4.3 Bit manipulation** has no 9608 questions at all (its Legend file is two pages with none). Bit manipulation is nonetheless examined in **every single series**, usually attached to the big assembly question. That is why there are no `9608 |` entries below: unlike chapters 2, 3, 5, 6 and 7, there is no old-syllabus fallback to draw on.

---

# 4.1 Central Processing Unit (CPU) Architecture

## 4.1.1 The Von Neumann model and the stored program concept

> [!question] 9618 | Correct the incorrect statements about the Von Neumann model [3]
> Each statement about the Von Neumann model contains an error. Write the correct statement.
>
>> [!success]- Answer — 1 mark per correction, 3 marks
>> - The PC stores the **address of** the next instruction to be fetched — **not the instruction itself**
>> - The CU sends signals to other components on the **control bus** — not the data bus
>> - The MDR **holds data to be stored in, or data read from**, the memory address in the MAR
>> - … it does **not** "transfer data to" the MAR
>> - Each answer must be the **corrected statement**, not just a note of what is wrong
>>
>> *Latest: `9618_s25_qp_12_sc_1.a`*

> [!question] 9618 | Identify the components of the Von Neumann model [3]
> Other than registers and buses, identify three components of the Von Neumann model of a computer.
>
>> [!success]- Answer — 4 points for 3 marks
>> - **Control Unit (CU)**
>> - **Arithmetic and Logic Unit (ALU)**
>> - **Immediate Access Store (IAS)**
>> - **System clock**
>>
>> *Latest: `9618_w23_qp_13_sc_9.a.i`. Registers and buses are excluded by the question — offering them scores nothing.*

> [!question] 9618 | State what is meant by the stored program concept [1]
> State what is meant by the stored program concept.
>
>> [!success]- Answer — 2 phrasings for 1 mark
>> - **Instructions and data** are stored in the **same memory space**
>> - … that is, both are held in main memory, and instructions are fetched from there in sequence
>>
>> *Latest: `9618_w22_qp_11_sc_5.a`*

> [!question] Inferred | Explain why the stored program concept is significant [3]
> Explain why the stored program concept was significant in the development of computers.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The program is held in **memory alongside the data**, not fixed in the hardware
>> - … so the computer can run **any program** without being physically rewired
>> - A program can be **loaded and replaced** like any other data
>> - … so the same machine becomes **general purpose**
>> - Instructions can be fetched in sequence at **electronic speed** rather than read from external media
>>
>> *Inference: 9618 has only ever asked for the one-line definition. What the concept **enables** has never been asked in either series, and 9618 marks "explain the significance" questions at 3.*

> [!question] SME | Describe the Von Neumann model [3]
> Describe the Von Neumann model of a computer system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Proposed by **John Von Neumann** in the 1940s; most general-purpose computers are built on it
>> - A **CPU that can access memory directly**
>> - **Memory that stores programs as well as data**, in the same address space
>> - **Stored programs whose instructions are executed in order**, one at a time
>> - The CPU contains a **CU, an ALU and registers**, connected to memory by buses
>>
>> *The framing "the CPU can access memory directly" is the part no mark scheme states.*

---

## 4.1.2 Registers: purpose, role, and general vs special purpose

> [!question] 9618 | Describe the purpose of each named register [4]
> Complete the table by describing the purpose of the PC, MAR, MDR and IX.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - **PC** — stores the **address of the next instruction** to be fetched / executed
>> - **MAR** — stores the **address** of the memory location where data will be read from or written to
>> - **MDR** — stores the **data read from** the address in the MAR, or the data to be written to it
>> - **IX** — stores a number that is **added to the operand** to form the address of the data
>>
>> *Latest: `9618_w24_qp_12_sc_3.a`*

> [!question] 9618 | Identify two other special purpose registers and state their roles [4]
> Identify two special purpose registers, other than the accumulator, and state the role of each.
>
>> [!success]- Answer — 2 marks per register (name + role), 4 marks
>> - **PC** — stores the address from which the **next instruction** is to be read
>> - **MAR** — stores the address of the memory location (or I/O component) **currently** being read from or written to
>> - **CIR** — holds the instruction **currently being decoded and/or executed**
>> - **Status Register** — contains bits that can be referenced individually and set or cleared depending on the operation, e.g. **overflow, underflow**
>>
>> *Latest: `9618_w23_qp_11_sc_5.a`*

> [!question] 9618 | Describe the purpose of the Status Register [2]
> Describe the purpose of the Status Register.
>
>> [!success]- Answer — 4 points for 2 marks
>> - To store the values of **flags / individual bits**
>> - … which are set or cleared after **arithmetic or logical operations**
>> - … such as overflow, underflow, carry, negative and zero
>> - The flags can then be **checked**, to change the **instruction sequence** (e.g. by a conditional jump)
>>
>> *Latest: `9618_w24_qp_11_sc_8.a`*

> [!question] 9618 | State two differences between general purpose and special purpose registers [2]
> State two differences between general purpose registers and special purpose registers.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Special purpose registers have a **specified role** in the machine; general purpose registers can be used for **any purpose the programmer defines**
>> - Special purpose registers hold the **state of the program's execution**; general purpose registers hold the program's **data** during operations
>> - General purpose registers can be used by **most instructions**; special purpose registers only by **certain instructions**
>> - There are usually **many** general purpose registers but a fixed small set of special purpose ones
>>
>> *Latest: `9618_w24_qp_11_sc_8.b` (also `9618_w23_qp_13_sc_9.a.ii`)*

> [!question] 9618 | Describe the role of the ACC and the CIR [2]
> Describe the role of the Accumulator and of the Current Instruction Register.
>
>> [!success]- Answer — 1 mark each, 4 points
>> - **ACC** — stores the **intermediate results** of arithmetic and logical operations
>> - … // holds the result of the current calculation performed by the ALU
>> - **CIR** — holds the instruction **currently being decoded and/or executed**
>> - … it is loaded from the MDR at the end of the fetch stage
>>
>> *Latest: `9618_w25_qp_11_sc_6.a`*

> [!question] 9618 | Identify one other register used in the Fetch–Execute cycle and describe its role [2]
> Identify one register, other than those given, used in the Fetch–Execute cycle and describe its role.
>
>> [!success]- Answer — name + role, 2 marks
>> - **CIR** — stores the instruction to be decoded / executed next
>> - **Status register** — contains bits that can be referenced individually to indicate a state or event
>> - **Interrupt register** — stores details of any interrupts that have occurred
>> - Lead with a **syllabus-named** register (PC, MDR, MAR, ACC, IX, CIR, Status) where possible
>>
>> *Latest: `9618_s25_qp_12_sc_1.b`*

> [!question] Inferred | Explain why a processor has an Index Register [3]
> Explain why a processor has an Index Register.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Its contents are **added to the operand** to form the address actually used — the effective address
>> - So a **single instruction** can access **many different memory locations**
>> - … by changing only the value in IX, rather than rewriting the instruction
>> - This allows a program to **step through an array or table** inside a loop
>> - IX can be incremented (`INC IX`) each pass, which is how indexed addressing is used in practice
>>
>> *Inference: IX appears in the `w24_qp_12_sc_3.a` table and in every indexed-addressing question, but no question asks **why** an index register exists. That link between 4.1 and 4.2 is untested.*

> [!question] SME | State the purpose of each of the seven registers [4]
> Name the special purpose registers of a CPU and state the purpose of each.
>
>> [!success]- Answer — 7 registers, marked in pairs, 4 marks
>> - **PC** — holds the address of the next instruction, and increments as the cycle runs
>> - **MAR** — holds the address that data or instructions are fetched from or written to
>> - **MDR** — stores the data or instruction fetched from that memory location
>> - **CIR** — stores the instruction currently being decoded or executed
>> - **ACC** — stores the results of calculations from the ALU
>> - **IX** — stores a value added to an address to give the effective address, for indexed addressing
>> - **SR** — stores flags reflecting the outcome of CPU operations
>>
>> *SME's framing — registers are "extremely small, extremely fast memory located in the CPU" — is the one-line definition the mark schemes assume but never state.*

---

## 4.1.3 The ALU, Control Unit, system clock and Immediate Access Store

> [!question] 9618 | Explain how the Control Unit and the system clock work together [2]
> Explain how the Control Unit and the system clock work together.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The control unit **synchronises** the actions of the processor
>> - … by sending a command / signal on **each timing signal** produced by the system clock
>> - … using the **control bus**
>> - So all components act **in step**, in the correct sequence
>>
>> *Latest: `9618_s25_qp_13_sc_2.a.i`*

> [!question] 9618 | Explain how the CU, system clock and control bus transfer data [4]
> Explain how the Control Unit, the system clock and the control bus work together when data is transferred.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The **system clock** produces regular **timing signals**
>> - … which are sent out on the **control bus**
>> - … to **synchronise** the other system components
>> - The **Control Unit initiates** the data transfer
>> - … by generating control signals (such as read and write)
>> - … which are also sent on the **control bus** to the other components
>>
>> *Latest: `9618_s23_qp_13_sc_7.b`*

> [!question] 9618 | State the purpose of the system clock and of the Control Unit [2]
> State the purpose of the system clock and the purpose of the Control Unit.
>
>> [!success]- Answer — 1 mark each, 6 points available
>> - **System clock** — to **synchronise operations**, by creating and transmitting timing signals on the control bus
>> - … to keep track of the date and time, and to ensure operations run in the correct sequence
>> - **Control Unit** — sends and receives **control signals** along the control bus
>> - … reads the instruction from the memory location whose address is in the **PC**
>> - … **coordinates / synchronises** the activity of the other CPU components
>> - … manages the execution of instructions and communication between CPU components
>>
>> *Latest: `9618_w24_qp_11_sc_3.a` (also `w22_qp_13_sc_4.b`, `w22_qp_11_sc_5.b.iii`)*

> [!question] 9618 | Describe what is meant by the Immediate Access Store [2]
> Describe what is meant by the Immediate Access Store (IAS).
>
>> [!success]- Answer — 3 points for 2 marks
>> - Holds all the **data, instructions and programs currently in use**
>> - Is **volatile** memory — its contents are lost when power is removed
>> - Has **fast access times**, so the CPU can reach it directly without delay
>>
>> *Latest: `9618_w23_qp_11_sc_5.b`*

> [!question] 9618 | Complete the cloze on the internal components of a CPU [5]
> Complete the description of the internal components of a computer.
>
>> [!success]- Answer — 1 mark per gap, 5 marks
>> - The **control unit** transmits signals to coordinate events
>> - … based on the pulses of the **(system) clock**
>> - The **data bus** carries data to the components
>> - The **address bus** carries the address where data is being written to or read from
>> - The **arithmetic logic unit (ALU)** performs mathematical operations and logical comparisons
>>
>> *Latest: `9618_s21_qp_12_sc_5.a`*

> [!question] Inferred | Describe the purpose of the ALU [2]
> Describe the purpose of the Arithmetic and Logic Unit.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Performs all **arithmetic operations** — addition, subtraction, and the shifts used for multiplication and division
>> - Performs all **logical operations** — AND, OR, NOT, XOR and comparisons
>> - The **result is placed in the accumulator**
>> - … and the appropriate **flags are set in the Status Register**
>>
>> *Inference: the ALU is named in the component list and in the cloze, but **no 9618 question asks you to describe its role** — compare the CU (asked three times) and the system clock (twice). An obvious 2-marker.*

> [!question] Inferred | Compare the IAS, RAM, cache and registers [3]
> Explain how the Immediate Access Store relates to RAM, cache memory and the registers.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The **IAS is main memory** — the RAM the CPU can access directly, holding what is currently in use
>> - **Registers** are inside the CPU: smallest, fastest, holding one value each
>> - **Cache** sits between the registers and main memory, holding frequently used instructions and data
>> - Access speed **decreases** and capacity **increases** at each step out from the CPU
>> - All three are **volatile**, unlike secondary storage
>>
>> *Inference: `w23_qp_11_sc_5.b` credits "volatile, fast access, holds what is currently in use" — which is equally true of RAM. Whether the IAS **is** main memory, and how it relates to cache and registers, has never been examined.*

---

## 4.1.4 Data transfer using the address, data and control buses

> [!question] 9618 | Identify two types of signal a control bus can transfer [2]
> Identify two types of signal that can be transferred on the control bus.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Interrupt** signals
>> - **Timing** signals (from the system clock)
>> - **Read** signals
>> - **Write** signals
>>
>> *Latest: `9618_s23_qp_12_sc_5.a`*

> [!question] 9618 | Tick which bus each CPU component uses [1]
> Tick to show which bus each component uses.
>
>> [!success]- Answer — both rows for 1 mark
>> - System clock → **control bus**
>> - MAR → **address bus**
>> - MDR → **data bus**
>>
>> *Latest: `9618_w22_qp_11_sc_5.b.ii`*

> [!question] 9618 | Describe the roles of the address bus, data bus and buffers when writing to a device [3]
> Describe the role of the address bus, the data bus and buffers when data is written to a device.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - **Buffers** — temporarily hold the data until it is ready to be transmitted **to the device**
>> - **Address bus** — carries the address (in RAM) of the **data to be written to the device**
>> - **Data bus** — carries all the **data to be written to the device / buffer**
>> - Each answer must be tied to **writing to the device**, not described generically
>>
>> *Latest: `9618_w23_qp_12_sc_8.c.ii`. The same question appears in the Chapter 3 Pack under buffers.*

> [!question] 9618 | Explain how different bus widths affect performance [2]
> Explain how the widths of the data bus and the address bus affect the performance of a computer.
>
>> [!success]- Answer — 5 points for 2 marks
>> - A **wider data bus** means more data can be transferred between components at a time
>> - … so there is **less delay / latency** when fetching data for a running process
>> - A **wider address bus** means **larger memory addresses** can be used
>> - … so more memory locations can be **addressed directly**
>> - … so the computer is less likely to run out of addressable memory
>>
>> *Latest: `9618_s25_qp_11_sc_6.a.iii`*

> [!question] Inferred | State which buses are unidirectional and which are bidirectional [2]
> State whether each of the address, data and control buses is unidirectional or bidirectional, and justify your answer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **address bus is unidirectional** — addresses only ever travel **from the CPU to memory**
>> - … the CPU specifies the location; memory never sends an address back
>> - The **data bus is bidirectional** — data must travel **both to and from** memory and devices
>> - The **control bus is bidirectional** — the CPU sends read/write signals out, and receives interrupt signals back
>>
>> *Inference: every mark scheme describes what each bus **carries**, but none asks about direction. It is standard credited content elsewhere and follows directly from what each bus does.*

> [!question] Inferred | Calculate the addressable memory from the address bus width [2]
> An address bus is 32 bits wide. Calculate the number of memory locations that can be addressed directly, and state what happens if the bus is widened by one bit.
>
>> [!success]- Answer — 4 points for 2 marks
>> - An **n-bit address bus** can address **2ⁿ** locations
>> - So a 32-bit bus addresses **2³² = 4 294 967 296** locations (4 GiB if each holds one byte)
>> - Adding **one bit doubles** the number of addressable locations
>> - The **data bus width** determines how much is moved at once, not how much can be addressed
>>
>> *Inference: `s25_qp_11_sc_6.a.iii` credits "larger memory addresses can be used, allowing more memory locations to be accessed", but the numeric version has never been asked in this topic — though the same arithmetic appears in Chapter 1.*

> [!question] SME | Describe what a bus is and what each of the three carries [3]
> Describe what is meant by a bus and state what each of the three buses carries.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A bus is a **set of parallel wires** through which data or signals are transmitted between components
>> - **Address bus** — unidirectional; carries the location being written to or read from
>> - **Data bus** — bidirectional; carries data or instructions
>> - **Control bus** — bidirectional; carries commands and control signals telling components when to read or write
>> - The **width** of a bus is the number of wires, i.e. the number of bits carried at once
>>
>> *The "parallel wires" definition and the directionality are absent from every mark scheme in this topic.*

---

## 4.1.5 Factors contributing to the performance of the computer system

> [!question] 9618 | Explain why increasing clock speed and cache memory improves performance [4]
> Explain how increasing the clock speed and increasing the cache memory each improve the performance of a computer.
>
>> [!success]- Answer — max 2 for each factor, 4 marks
>> - **Clock speed:** the processor can perform **more Fetch–Execute cycles per second**
>> - … so more instructions and data can be processed each second
>> - **Cache memory:** more of the **most frequently used instructions and data** can be stored
>> - … which reduces the need to access the **slower RAM**
>> - … so the CPU spends less time idle, waiting for data
>>
>> *Latest: `9618_w25_qp_12_sc_3.c`*

> [!question] 9618 | Describe two hardware upgrades and explain how each improves performance [4]
> Describe two hardware upgrades that would improve the performance of a computer, and explain how each works.
>
>> [!success]- Answer — 2 marks per upgrade, 4 marks
>> - Increase the **number of cores** … each core independently carries out a process at the same time, so more instructions are performed **in parallel**
>> - Increase **RAM capacity** … so more applications reside in memory at once, saving slow disk access
>> - Increase **cache memory** … more data is stored in fast-access memory, so less time is spent accessing RAM
>> - Increase the **clock speed** … so more Fetch–Decode–Execute cycles run per unit of time
>>
>> *Latest: `9618_s23_qp_12_sc_5.b` (also `9618_w22_qp_13_sc_4.c`). The same question appears in the Chapter 3 Pack — it is marked identically in both topics.*

> [!question] 9618 | Explain why a dual-core CPU is not twice as fast as a single-core CPU [5]
> A computer with a dual-core processor is not twice as fast as an otherwise identical computer with a single-core processor. Explain why.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Multiple cores introduce **additional overheads**
>> - … because of the need for **communication between the cores**
>> - … and time spent **organising which task goes to which core**
>> - Software may **not be designed for multiple cores**
>> - … so one of the cores will be left **idle**
>> - **Memory access speed** may not match the speed of the cores, causing a delay
>> - The two computers may differ in **more than the cores** — one may have more RAM, or a GPU
>>
>> *Latest: `9618_w23_qp_11_sc_5.c.ii`. The largest single tariff in 4.1.*

> [!question] 9618 | Describe the drawbacks of increasing the number of cores [2]
> Describe the drawbacks of increasing the number of cores in a processor.
>
>> [!success]- Answer — 4 points + expansions for 2 marks
>> - **Latency may increase** … because the cores must communicate with one another
>> - There is a potential for **deadlock** … where one core waits for information from another core that is itself waiting
>> - Not all software is designed for **multiple cores** … so some cores would be idle
>> - **Increased heat generation** … which could damage other components
>>
>> *Latest: `9618_w25_qp_11_sc_6.b`*

> [!question] 9618 | Describe how the number of cores and the clock speed affect performance [4]
> Describe how the number of cores and the clock speed of a processor affect the performance of a computer.
>
>> [!success]- Answer — max 3 per factor, 4 marks
>> - **Cores:** each core processes one instruction per clock pulse
>> - … multiple cores mean sequences of instructions can be **split between them**
>> - … so more than one instruction is executed per clock pulse, decreasing the time to complete a task
>> - **Clock speed:** each instruction is executed on a **clock pulse**
>> - … one Fetch–Execute cycle runs on each pulse
>> - … so the clock speed dictates the **number of instructions run per second**
>>
>> *Latest: `9618_s21_qp_12_sc_5.b`*

> [!question] 9618 | Describe one benefit of cache memory [2]
> Describe one benefit of increasing the amount of cache memory in a computer.
>
>> [!success]- Answer — 5 points for 2 marks
>> - Cache is **fast-access memory close to the CPU**
>> - … which stores **frequently used instructions and data**
>> - … so they can be accessed **faster than from RAM**
>> - More cache means **less swapping** between RAM and cache
>> - … which prevents the CPU **idling** while it waits for data
>>
>> *Latest: `9618_s25_qp_13_sc_2.b` (also `9618_w22_qp_11_sc_7.d`)*

> [!question] 9618 | Explain how different amounts of RAM affect performance [3]
> Explain how the amount of RAM in a computer affects its performance.
>
>> [!success]- Answer — 5 points for 3 marks
>> - More RAM means **more of the currently running data and instructions** can be stored
>> - … so there is **no need to use virtual memory**
>> - … and data does not have to be fetched from **secondary storage** first
>> - Secondary storage has a much **slower access time**
>> - So there is **less latency** waiting for instructions or data
>>
>> *Latest: `9618_s25_qp_11_sc_6.a.ii`. Identical to the Chapter 3 entry — one answer serves both.*

> [!question] 9618 | Identify one feature of a processor that affects performance and state why [2]
> Identify one feature of a processor that affects the performance of a computer, and state why it does so.
>
>> [!success]- Answer — feature + reason, 2 marks
>> - **Clock speed** — a higher clock speed means more Fetch–Execute cycles are executed per second // greater throughput
>> - **Bus width** — a larger bus width means more data is transferred at the same time
>> - **Number of cores** — more instructions can be processed in parallel
>> - **Cache size** — more frequently used data is held close to the CPU
>>
>> *Latest: `9618_w24_qp_11_sc_3.b.i`*

> [!question] Inferred | Explain how the type of processor affects performance [3]
> Explain how the **type** of processor chosen affects the performance of a computer system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A **GPU** has many simple cores designed for **parallel** work, so it far outperforms a CPU on graphics and similar repetitive calculations
>> - A **CPU** has fewer, more capable cores, so it is better for **general-purpose, sequential** tasks
>> - A **low-power processor** in an embedded or mobile device trades speed for **battery life and heat**
>> - Different processors have different **instruction sets**, so some operations take fewer cycles on one than another
>> - The processor must **match the workload** — raw speed is not the only measure
>>
>> *Inference: the syllabus notes say "processor **type** and number of cores". Every 9618 question examines cores, clock speed, cache and bus width; the **type** is never asked, despite being the first item in the notes.*

> [!question] Inferred | Explain why a computer does not have very large cache memory [3]
> Explain why computers are not built with very large amounts of cache memory.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Cache is made from **SRAM**, which uses several transistors per cell
>> - … so it is **expensive** and has a **low storage density**
>> - It must be physically **close to the CPU**, and there is limited space on the chip
>> - Beyond a certain size there are **diminishing returns** — most frequently used data already fits
>> - … and a larger cache takes **longer to search**, eroding the speed advantage
>>
>> *Inference: the mark schemes treat "more cache is better" as always true. The link back to SRAM in Chapter 3, and the reason cache is small, is untested.*

> [!question] SME | Describe the three levels of cache [3]
> Describe the levels of cache memory in a modern processor.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **L1** — inside each CPU core; the fastest and the smallest
>> - **L2** — inside or immediately beside each core; fast, medium size
>> - **L3** — **shared by all the cores**; slower than L1 and L2, but the largest
>> - The CPU checks L1 first, then L2, then L3, then RAM
>> - This is why "cache is close to the CPU" is the credited reason it is fast
>>
>> *Not named in any 9618 mark scheme, but it explains the credited answer.*

> [!question] SME | Calculate a theoretical instruction throughput and explain its limits [3]
> A quad-core processor runs at 3 GHz. Calculate the theoretical maximum number of instructions per second and explain why this figure is not achieved in practice.
>
>> [!success]- Answer — 5 points for 3 marks
>> - 4 cores × 3 × 10⁹ pulses per second = **12 × 10⁹ (12 billion) instructions per second**
>> - … assuming one instruction completes per core per clock pulse
>> - In practice, time is spent **organising tasks between the cores**
>> - Some tasks are **sequential** and must be carried out step by step, so cannot be split
>> - Memory access and software that is not multi-core aware leave cores **idle**
>>
>> *SME's caveat matches the `w23_qp_11_sc_5.c.ii` mark scheme exactly.*

---

## 4.1.6 How different ports provide connection to peripheral devices

> [!question] 9618 | Identify a port and explain how it provides an automatic connection [3]
> Identify a port that allows a device to be connected automatically, and explain how the connection is made.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Port: **USB**
>> - A **voltage change** occurs when the device is plugged in
>> - The computer **detects this voltage change**
>> - The **code of the device** is transferred to the computer
>> - The OS finds that code in its list of devices and loads the appropriate **device driver**
>>
>> *Latest: `9618_w24_qp_11_sc_3.b.ii`*

> [!question] 9618 | Explain the benefits of using HDMI instead of VGA [4]
> Explain the benefits of connecting a high-resolution monitor using HDMI rather than VGA.
>
>> [!success]- Answer — 6 points for 4 marks
>> - HDMI has **faster transfer rates** than VGA
>> - … which is needed for the **high resolution / large number of pixels** of the monitor
>> - HDMI supports **video and audio on one cable**
>> - … so no separate sound cable is needed, unlike VGA
>> - HDMI is a **digital** interface, so no data is lost converting to analogue and back
>> - HDMI is **less prone to error, crosstalk and external interference**
>>
>> *Latest: `9618_w24_qp_12_sc_3.b`*

> [!question] 9618 | Explain how HDMI provides connection to peripheral devices [2]
> Explain how an HDMI port provides a connection to a peripheral device.
>
>> [!success]- Answer — 5 points for 2 marks
>> - Transfers both **audio and video** using a single cable
>> - Has **high bandwidth**
>> - Data is transmitted **in a stream**
>> - … of **uncompressed digital signals**
>> - Uses **Transition-Minimised Differential Signalling (TMDS)**
>>
>> *Latest: `9618_s25_qp_13_sc_2.c`*

> [!question] 9618 | Identify a suitable port for a device and justify the choice [3]
> Identify a suitable port for the device described and justify your choice.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **USB** — fast data transfer speeds
>> - … and it is a **universal / widely adopted standard**, so cables and support are easy to find
>> - **HDMI** — allows **video and audio** to be transferred on the same cable
>> - … which is convenient, as there is no need for two separate cables
>> - The justification must be **tied to the device in the question**
>>
>> *Latest: `9618_w23_qp_13_sc_7.d`*

> [!question] 9618 | Describe how data is transmitted through a USB port [1]
> Describe how data is transmitted through a USB port.
>
>> [!success]- Answer — 3 points for 1 mark
>> - **One bit is transferred at a time** — it is a **serial** connection
>> - It can be **synchronous or asynchronous**
>> - **USB 3** is full duplex; earlier versions are half duplex
>>
>> *Latest: `9618_s23_qp_12_sc_5.c.i`*

> [!question] 9618 | Name a suitable port for a given peripheral [2]
> Name a suitable port for each of the peripherals listed.
>
>> [!success]- Answer — 1 mark per device, 2 marks
>> - **3D printer** → USB port / COM port
>> - **Monitor** → HDMI / VGA / DisplayPort / USB-C
>> - **Optical disc reader/writer** → USB
>> - A named port is required — "a video port" scores nothing
>>
>> *Latest: `9618_w23_qp_12_sc_8.c.i` (also `9618_w22_qp_11_sc_7.e`)*

> [!question] Inferred | Describe what a VGA port is and state its limitations [3]
> Describe the VGA port and state two of its limitations.
>
>> [!success]- Answer — 5 points for 3 marks
>> - VGA is an **analogue** video interface, using a 15-pin connector
>> - It carries **video only**, so a **separate cable is needed for audio**
>> - The signal must be **converted from digital to analogue** and back, so quality is lost
>> - It is more prone to **interference and degradation over distance**
>> - It supports **lower resolutions and refresh rates** than HDMI or DisplayPort
>>
>> *Inference: VGA is named in the syllabus notes but appears only as the **loser** in the HDMI comparison. What VGA actually is has never been asked directly.*

> [!question] Inferred | Explain why a port needs a device driver [3]
> Explain why a device connected to a port needs a device driver.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The port detects the device and passes its **identifying code** to the operating system
>> - Each device understands its own **commands and data formats**, which differ between manufacturers
>> - The **driver translates** the OS's generic instructions into those the device understands
>> - … so the operating system does not need to know the details of every device
>> - Without the correct driver the device is **detected but unusable**
>>
>> *Inference: the driver appears in `w24_qp_11_sc_3.b.ii` and in the OS hardware-management mark schemes (Chapter 5), but the connection between the two is never the subject of a question.*

> [!question] SME | State the advantages and disadvantages of USB [4]
> State two advantages and two disadvantages of using USB to connect a peripheral.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Advantage:** automatic detection and driver loading when plugged in
>> - **Advantage:** connectors fit **only one way**, preventing incorrect connection
>> - **Advantage:** widely standardised, and **backwards compatible** with older USB versions
>> - **Disadvantage:** maximum cable length around **5 m**, so unusable over long distances
>> - **Disadvantage:** older versions have **limited transfer rates** (USB 1.1 ≈ 12 Mbps vs USB 3.x ≈ 5–20 Gbps)
>> - **Disadvantage:** very old standards may **lose support** in new operating systems
>>
>> *The backwards-compatibility and cable-length points are absent from every mark scheme, and are exactly what a "justify the port choice" answer needs.*

---

## 4.1.7 Stages of the Fetch–Execute cycle, and register transfer notation

> [!question] 9618 | Write the stages of the Fetch–Execute cycle in register transfer notation [4]
> Write the stages of the fetch stage of the Fetch–Execute cycle using register transfer notation.
>
>> [!success]- Answer — 3 marks for the statements + 1 for the order
>> - `MAR ← [PC]`
>> - `PC ← [PC] + 1`
>> - `MDR ← [[MAR]]`
>> - `CIR ← [MDR]`
>> - **1 mark for the correct order** — the increment may be combined as `MAR ← [PC] and PC ← [PC] + 1`
>> - Note the **double brackets** in `MDR ← [[MAR]]`: the contents of the address held in the MAR
>>
>> *Latest: `9618_s25_qp_13_sc_2.a.ii`*

> [!question] 9618 | Complete a table of Fetch–Execute steps and their descriptions [4]
> Complete the table by matching each register transfer statement to its description.
>
>> [!success]- Answer — 1 mark per row, 4 marks
>> - `MAR ← [PC]` ↔ the **contents of the PC** are copied to the MAR
>> - `PC ← [PC] + 1` ↔ the address in the PC is **incremented**
>> - `MDR ← [[MAR]]` ↔ the **data in the location pointed to by the MAR** is copied to the MDR
>> - `CIR ← [MDR]` ↔ the contents of the MDR are copied into the CIR
>>
>> *Latest: `9618_w23_qp_13_sc_9.b`*

> [!question] 9618 | Write the register transfer notation for each described stage [3]
> Write the register transfer notation for each of the stages described.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - Copy the address of the next instruction into the MAR → `MAR ← [PC]`
>> - Increment the Program Counter → `PC ← [PC] + 1`
>> - Copy the contents of the MDR into the CIR → `CIR ← [MDR]`
>> - Copy the contents of the address in the MAR into the MDR → `MDR ← [[MAR]]`
>>
>> *Latest: `9618_s23_qp_13_sc_7.c` (also `9618_w22_qp_12_sc_7.c`)*

> [!question] 9618 | Identify and correct the errors in given register transfer notation [4]
> The register transfer notation shown contains errors. Identify each error and write the correct statement.
>
>> [!success]- Answer — 1 mark for line + description, 1 for the correction, 4 marks
>> - `PC ← [PC] − 1` — the Program Counter should be **incremented, not decremented**
>> - … correct statement: `PC ← [PC] + 1`
>> - `MDR ← [MAR]` — it should be the **contents of the address held in** the MAR, not the MAR's own contents
>> - … correct statement: `MDR ← [[MAR]]`
>>
>> *Latest: `9618_w21_qp_11_sc_6.a`. Both halves are needed — describing the error without writing the correction scores half.*

> [!question] 9618 | Describe the role of the MAR and MDR in the Fetch–Execute cycle [4]
> Describe the role of the Memory Address Register and the Memory Data Register in the Fetch–Execute cycle.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The **MAR** stores the **address** of the next instruction or data to be read from or written to memory
>> - … the address is received from the **PC**
>> - The **MDR** stores the **data or instruction** held at the address in the MAR, once it has been read
>> - … or the data that is about to be written to that address
>> - The instruction then passes to the **CIR** for decoding and executing
>> - Every transfer between the CPU and memory passes through this pair
>>
>> *Latest: `9618_w25_qp_13_sc_6.b` (also `9618_w21_qp_12_sc_8.a.i`)*

> [!question] 9618 | Complete the cloze describing the registers in the Fetch–Execute cycle [5]
> Complete the description of the fetch stage of the Fetch–Execute cycle.
>
>> [!success]- Answer — 1 mark per gap, 5 marks
>> - The **Program Counter** holds the address of the next instruction to be loaded
>> - This address is sent to the **Memory Address Register**
>> - The **Memory Data Register** holds the data fetched from this address
>> - This data is sent to the **Current Instruction Register**, and the CU decodes the opcode
>> - The **Program Counter** is incremented
>>
>> *Latest: `9618_s21_qp_11_sc_3.a`*

> [!question] Inferred | Write the execute stage in register transfer notation [4]
> Write, in register transfer notation, the stages that take place when the instruction `LDD 100` is executed.
>
>> [!success]- Answer — 6 points for 4 marks
>> - `MAR ← [CIR(operand)]` — the operand (100) is copied into the MAR
>> - `MDR ← [[MAR]]` — the contents of address 100 are copied into the MDR
>> - `ACC ← [MDR]` — the data is copied into the accumulator
>> - For `STO 100` the sequence reverses: `MAR ← operand`, then `MDR ← [ACC]`, then `[[MAR]] ← [MDR]`
>> - For `ADD 100`: `MAR ← operand`, `MDR ← [[MAR]]`, `ACC ← [ACC] + [MDR]`
>> - 1 mark for the **correct order**, as in the fetch question
>>
>> *Inference: every 9618 question stops at `CIR ← [MDR]` — the **fetch** only — despite the bullet being titled "the stages of the **Fetch–Execute** cycle" and the syllabus saying "describe **and use** register transfer notation to describe the F-E cycle".*

> [!question] Inferred | Describe what happens during the decode stage [3]
> Describe what happens during the decode stage of the Fetch–Execute cycle.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The instruction is held in the **CIR**
>> - It is split into the **opcode** and the **operand**
>> - The **Control Unit interprets the opcode**, identifying which operation is required
>> - … by looking it up in the processor's **instruction set**
>> - Any data the instruction needs is then **retrieved from the address** given by the operand, ready for execution
>>
>> *Inference: the CIR splitting the instruction into opcode and operand appears once, as a cloze mark point (`s21_qp_11_sc_3.a`). A question asking what happens during decode has not been set.*

> [!question] SME | Describe the three stages of the cycle and what happens in each [3]
> Describe the three stages of the Fetch–Decode–Execute cycle.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Fetch** — the address of the next instruction is supplied to memory, and the instruction is returned to the CPU
>> - … the PC is incremented so it points at the following instruction
>> - **Decode** — the instruction is interpreted, and any data required is retrieved from its address
>> - **Execute** — the CPU carries out the required action
>> - … the result is placed in the **ACC** and any flags set in the **SR**, and the cycle repeats
>>
>> *SME's framing; 9618's 4-mark RTN questions cover the same ground in notation.*

---

## 4.1.8 The purpose of interrupts

> [!question] 9618 | Explain how the computer handles an interrupt [5]
> Explain how a computer handles an interrupt.
>
>> [!success]- Answer — 8 points for 5 marks
>> - An **interrupt flag is raised** in the interrupt register
>> - At the **end of the current Fetch–Execute cycle** // at the start of the next
>> - The system **checks the interrupt register** for interrupts of **higher priority** than the current process
>> - If there is one, the current contents of the registers are **stored on the stack**
>> - The appropriate **Interrupt Service Routine (ISR)** is called
>> - The input or event is **processed**
>> - The register contents are **restored from the stack**
>> - **Control is passed back** to the previous process, which resumes where it left off
>>
>> *Latest: `9618_s23_qp_11_sc_6`*

> [!question] 9618 | Explain how an interrupt is detected and handled within the Fetch–Execute cycle [4]
> Explain how an interrupt is detected and handled during the Fetch–Execute cycle.
>
>> [!success]- Answer — 7 points for 4 marks
>> - At the start / end of each Fetch–Execute cycle the **interrupt register is checked**
>> - The **priority** of any waiting interrupt is checked
>> - If its priority is **higher than the current process**, the interrupt is serviced
>> - The contents of the registers are **stored on the stack**
>> - The relevant **ISR / interrupt handler** is called
>> - When the ISR finishes, a **further check** is made for higher-priority interrupts
>> - If there are none, the register contents are **restored** and the next Fetch–Execute cycle continues
>>
>> *Latest: `9618_s25_qp_12_sc_1.c`*

> [!question] 9618 | Put the stages of interrupt handling into order [3]
> Put the stages the CPU performs when an interrupt is detected into the correct order.
>
>> [!success]- Answer — 1 mark per correct placement, 3 marks
>> - 1 — at the end of each Fetch–Execute cycle the processor checks whether an **interrupt flag is set**
>> - 2 — the processor **identifies the source** of the interrupt and checks its **priority**
>> - 3 — if the priority is high enough, the processor **saves the current register contents**
>> - 4 — the **address of the ISR is loaded into the PC**
>> - 5 — when servicing is complete, the processor **restores the registers**
>> - 6 — **lower-priority interrupts are re-enabled**
>>
>> *Latest: `9618_w23_qp_13_sc_9.d`*

> [!question] 9618 | State when interrupts are detected during the Fetch–Execute cycle [1]
> State when during the Fetch–Execute cycle interrupts are detected.
>
>> [!success]- Answer — 2 phrasings for 1 mark
>> - **After completion of the execute stage** // at the end of the current cycle
>> - … that is, **before the next cycle begins**
>>
>> *Latest: `9618_w22_qp_13_sc_4.a.ii`*

> [!question] 9618 | Describe the purpose of an interrupt [2]
> Describe the purpose of an interrupt.
>
>> [!success]- Answer — 4 points for 2 marks
>> - To **send a signal** from a device or a process
>> - … **seeking the attention of the processor**
>> - So that an event can be dealt with **as soon as it occurs**
>> - … without the processor having to keep checking every device
>>
>> *Latest: `9618_w22_qp_11_sc_5.c`*

> [!question] 9618 | Identify causes of a software interrupt [2]
> Identify two causes of a software interrupt.
>
>> [!success]- Answer — 6 points for 2 marks
>> - **Division by zero** // a runtime error in a program
>> - Attempt to access an **invalid memory location** // out of memory bounds
>> - **Array index out of bounds**
>> - **Stack overflow**
>> - **Buffer overflow** // buffer full
>> - A program **requesting an external device or input**
>>
>> *Latest: `9618_w23_qp_13_sc_9.c` (also `9618_w22_qp_11_sc_5.d`)*

> [!question] 9618 | Tick whether each event is a hardware or a software interrupt [3]
> Tick to show whether each event causes a hardware interrupt or a software interrupt.
>
>> [!success]- Answer — 1 mark per pair of rows, 3 marks
>> - Buffer full → **software**
>> - Printer out of paper → **hardware**
>> - User has pressed a key → **hardware**
>> - Division by zero → **software**
>> - Power failure → **hardware**
>> - Stack overflow → **software**
>>
>> *Latest: `9618_w21_qp_12_sc_7.a`. The rule: caused by a **device** → hardware; caused by **running code** → software.*

> [!question] Inferred | Describe the applications of interrupts [3]
> Describe three applications of interrupts in a computer system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Real-time event handling** — hardware errors and signals from input devices, e.g. a hard disk failure, are dealt with immediately
>> - **Device communication** — a peripheral alerts the processor, e.g. a printer jam, an empty buffer or a network error
>> - **Multitasking** — one application is suspended so the processor can switch to another, giving each a share of processor time
>> - **User input** — a key press or mouse click is handled at once, so the system feels responsive
>> - **Timed events** — a clock interrupt drives scheduling and the system clock
>>
>> *Inference: the syllabus notes list "possible causes of interrupts, **applications** of interrupts, use of an ISR, when interrupts are detected, how interrupts are handled". Causes, detection and handling are examined repeatedly; **applications** is the one named sub-point with no question against it.*

> [!question] Inferred | Explain why interrupts are used rather than polling [3]
> Explain why a computer uses interrupts rather than repeatedly checking each device.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Without interrupts, the CPU would have to **repeatedly check (poll) every device**
>> - … which wastes processor cycles on devices that need nothing
>> - With interrupts, the device **signals the processor** only when it needs attention
>> - … so the processor can do useful work in the meantime
>> - Response is also **faster**, because the event is handled at the end of the current cycle rather than at the next poll
>>
>> *Inference: implied by "seeking the attention of the processor" but never examined.*

> [!question] Inferred | Explain why register contents are stored on a stack [3]
> Explain why the contents of the registers are saved on a stack when an interrupt is serviced.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The ISR will **overwrite the registers**, so the interrupted program's state must be saved
>> - A stack is **last-in-first-out**
>> - … so when an interrupt interrupts another interrupt (**nesting**), the states unwind in the **reverse order** they were saved
>> - Each interrupted process therefore resumes with **its own** register values
>> - Without a stack, a second interrupt would **destroy** the first one's saved state
>>
>> *Inference: "stores the register contents on the stack" is a credited mark point in two questions, but **why a stack** is never asked — even though `w23_qp_13_sc_9.d` includes re-enabling lower-priority interrupts, which only makes sense with nesting.*

> [!question] SME | Describe the five steps of the interrupt process [5]
> Describe the process that takes place from the moment an interrupt is generated to the moment normal processing resumes.
>
>> [!success]- Answer — 7 points for 5 marks
>> - **1 Interrupt Request (IRQ)** — a device or program generates an interrupt, passed by the interrupt controller to the handler
>> - **2 Acknowledge** — the handler decides whether to deal with it now or later, based on priority
>> - … if now, the **current register contents are saved** on the stack
>> - **3 ISR lookup** — the processor fetches the address of the ISR associated with that interrupt type
>> - **4 ISR execution** — control transfers to the ISR, which handles the event
>> - **5 Interrupt exit** — the registers are **restored** and the Fetch–Decode–Execute cycle resumes
>> - Lower-priority interrupts are then **re-enabled**
>>
>> *SME's five-step framing; 9618's own 5-mark handling question sets the tariff.*

> [!question] SME | Describe what an Interrupt Service Routine is [2]
> Describe what is meant by an Interrupt Service Routine.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **special routine** that handles one particular type of interrupt
>> - Each interrupt type has **its own routine** — printer jam, hard disk failure, network error
>> - Its address is found from a table and **loaded into the PC** when the interrupt is serviced
>> - ISRs should be **concise and efficient**, because they often handle time-sensitive events and delay other work
>>
>> *The "concise so as not to delay other work" point is in no mark scheme. Note also that SME names a third type — a **trap interrupt** — which is **not** in the 9618 syllabus: do not offer one where the question asks for a type.*

---

# 4.2 Assembly Language

## 4.2.1 The relationship between assembly language and machine code

> [!question] 9618 | Complete the description of language translators [4]
> Complete the description of compilers, interpreters and assemblers.
>
>> [!success]- Answer — 1 mark per gap, 4 marks
>> - **Compilers** are used when a high-level program is complete; they translate all the code at once
>> - … and produce **executable / .exe / object code** files that run without the source code
>> - **Interpreters** translate one line at a time and run it
>> - … useful while developing, because errors can be corrected and the program continues from that line
>> - **Assemblers** translate assembly code into **binary / machine code**
>>
>> *Latest: `9618_w21_qp_11_sc_4.d`. Shared with Chapter 5 — see the System Software Pack for the fuller translator questions.*

> [!question] Inferred | Explain the relationship between assembly language and machine code [3]
> Explain the relationship between assembly language and machine code.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **One assembly language instruction translates to one machine code instruction** — a one-to-one relationship
>> - … unlike a high-level statement, which becomes **many** machine code instructions
>> - Assembly uses **mnemonics** in place of binary opcodes, and labels in place of addresses
>> - It is translated by an **assembler**
>> - Each processor type has **its own instruction set**, so assembly is machine specific
>>
>> *Inference: this bullet has **exactly one** 9618 question, and it is a cloze shared with Chapter 5. The defining one-to-one fact is not credited anywhere in the 9618 series, which makes it the most likely content for a new question on this bullet.*

> [!question] Inferred | Explain why assembly language is still used [3]
> Explain why a programmer might still write part of a program in assembly language.
>
>> [!success]- Answer — 5 points for 3 marks
>> - It gives **direct control of the hardware** — specific registers, ports and memory locations
>> - It produces a **minimal memory footprint**, which matters where memory is tiny
>> - It can be **faster to execute**, because the programmer controls exactly which instructions run
>> - It is used in **embedded systems and device drivers**, where both of these matter
>> - … which links directly to embedded systems in Chapter 3
>>
>> *Inference: untested in 9618, but every point follows from content the syllabus already covers.*

> [!question] SME | Compare machine code and assembly language [4]
> Compare machine code and assembly language.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Machine code** is a **first-generation** language, written in binary
>> - … directly executable by the processor, with no translation needed
>> - **Assembly** is a **second-generation** language written using **mnemonics**
>> - … human-readable, but corresponding almost exactly to machine code
>> - It must be translated by an **assembler**, and each CPU type has its **own instruction set**
>> - Each instruction splits into an **opcode** (the operation) and an **operand** (the data or address)
>>
>> *The opcode/operand split is credited in 9618 cloze answers; the generation labels are SME's.*

---

## 4.2.2 The stages of the assembly process for a two-pass assembler

> [!question] 9618 | Identify the purpose of the first pass [1]
> State the purpose of the first pass of a two-pass assembler.
>
>> [!success]- Answer — 1 mark
>> - To **create the symbol table**
>> - … recording each label and the address it corresponds to
>>
>> *Latest: `9618_w23_qp_11_sc_8.a`*

> [!question] 9618 | Identify which pass each action takes place in [3]
> For each action, identify whether it takes place in the first pass, the second pass, or both.
>
>> [!success]- Answer — 1 mark per row, 3 marks
>> - Generates the object code → **second pass**
>> - Reads the source code one line at a time → **both passes**
>> - Removes white space → **first pass**
>> - Adds labels to the symbol table → **first pass**
>> - Removes comments → **first pass**
>> - Checks the opcode is in the instruction set → **first pass**
>>
>> *Latest: `9618_s23_qp_12_sc_3.a` (also `9618_w22_qp_11_sc_6.c`). The rule: **preparation and the symbol table** are pass one; **generating object code** is pass two; **reading the source** is both.*

> [!question] Inferred | Describe what happens during the second pass [3]
> Describe the stages that take place during the second pass of a two-pass assembler.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The source code is read **one line at a time** again
>> - Each **label is replaced with the address** stored against it in the symbol table
>> - Each **mnemonic is converted into its binary opcode**, using the instruction set
>> - Each operand is converted into its **binary form**
>> - The **object code** is generated and output, ready to be loaded and run
>>
>> *Inference: all three 9618 questions are sorting exercises. None asks candidates to **describe** the second pass, even though the syllabus says "describe the different **stages**".*

> [!question] Inferred | Apply the two-pass process to a given program [4]
> Apply the two-pass assembler process to the assembly language program given. Show the symbol table produced.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Pass 1** assigns an address to each line, in order, starting from the load address
>> - … and records every **label** with the address it refers to, building the **symbol table**
>> - … e.g. for `LOAD A / ADD B / STORE C / HALT / A: DATA 5 / B: DATA 3 / C: DATA 0` → A = 04, B = 05, C = 06
>> - … instructions are **not yet translated** in pass 1
>> - **Pass 2** replaces each label with its address and each mnemonic with its opcode
>> - … outputting the object code — `01 04` / `02 05` / `03 06` / `00 00` — as an **object program** that a **loader** executes later
>>
>> *Inference: the syllabus notes say explicitly "apply the two-pass assembler process to a given simple assembly language program", yet **no 9618 question has ever required a symbol table to be built**. This is the clearest untested instruction in 4.2.*

> [!question] Inferred | Explain why two passes are needed [2]
> Explain why an assembler needs two passes.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A program can contain **forward references** — a `JMP` to a label defined **later** in the program
>> - … whose address is not yet known when that line is first read
>> - The **first pass** records every label and its address, so all addresses are known
>> - … so the **second pass** can resolve every reference and generate complete object code
>>
>> *Inference: never asked in either series, but it is the reason the two-pass design exists.*

---

## 4.2.3 Trace a given simple assembly language program

> [!question] 9618 | Complete a trace table for an assembly language program [6]
> Complete the trace table for the assembly language program shown.
>
>> [!success]- Answer — marked per shaded **set** of values, up to 6 marks
>> - Columns are typically: **instruction address · ACC · selected memory addresses · IX · OUTPUT**
>> - Marks are awarded per shaded **block**, not per cell — a single early error can lose a whole block
>> - Work **down the instruction-address column** first, filling every change on each row before moving on
>> - `CMP` **sets a flag but leaves the ACC unchanged**
>> - `JPE` / `JPN` depend on the **most recent** compare, not on the ACC
>> - `INC IX` changes only IX — remember that indexed loads then read a **different** address
>>
>> *Latest: `9618_s24_qp_13_sc_3.a`-style; the 6-mark version is the largest in the topic.*

> [!question] 9618 | Write the contents of the ACC after each instruction [4]
> Write the contents of the accumulator after each of the instructions shown.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - ACC `0000 1111`, then `AND 101` → **`0000 1110`**
>> - ACC `0000 0000`, then `LDM #100` → **`0110 0100`** (100 in binary)
>> - ACC `0000 0001`, then `XOR &F1` → **`1111 0000`**
>> - ACC `0001 0001`, then `CMP 101` → **`0001 0001`** — **CMP does not change the ACC**
>> - Watch the prefixes: `#` denary, `B` binary, `&` hexadecimal
>>
>> *Latest: `9618_w25_qp_13_sc_6.a`. The CMP row is the classic trap.*

> [!question] 9618 | State the purpose of a fragment of assembly code [1]
> State the purpose of the assembly language instructions shown.
>
>> [!success]- Answer — 1 mark
>> - `LDD 100 / STO 165 / LDD 101 / STO 100 / LDD 165 / STO 101`
>> - → it **swaps the contents of memory addresses 100 and 101**
>> - … using 165 as the temporary store, exactly as a swap in pseudocode would
>>
>> *Latest: `9618_w22_qp_11_sc_6.a.ii`*

> [!question] 9618 | State the effect of changing one instruction [1]
> State the effect on the program of changing the instruction shown.
>
>> [!success]- Answer — 3 points for 1 mark
>> - Changing `LDD 10` to `LDM #10` loads **the number 10** instead of **the contents of address 10**
>> - So the addition gives **20 instead of 22**
>> - … the comparison then fails, and the result is an **infinite loop**
>>
>> *Latest: `9618_s25_qp_12_sc_7.a.ii`. The answer must state the **consequence**, not just the difference.*

> [!question] Inferred | Write a short assembly fragment to perform a given task [3]
> Write assembly language instructions that add the contents of address 200 to the contents of address 201 and store the result in address 202.
>
>> [!success]- Answer — 5 points for 3 marks
>> - `LDD 200` — load the contents of address 200 into the ACC
>> - `ADD 201` — add the contents of address 201 to the ACC
>> - `STO 202` — store the result in address 202
>> - `END` — terminate the program
>> - Every instruction must have a **valid opcode from the given instruction set** and a **suitable operand**
>>
>> *Inference: the syllabus bullet is only "**trace** a given simple program", so full program writing is correctly untested — but `s25_qp_13_sc_5.b` and `w24_qp_13_sc_7.b` do ask candidates to **write bit-manipulation instructions**, so short fragments are clearly within reach.*

---

## 4.2.4 Instruction groups

> [!question] 9618 | Complete statements naming the instruction group [3]
> Complete each statement by naming the group of instructions being described.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - Loading data into the accumulator → **data movement**
>> - Incrementing the index register → **arithmetic operations**
>> - Branching to another address → **unconditional and conditional (jump) instructions**
>> - Checking a value against the accumulator → **compare instructions**
>> - Reading a character from the keyboard → **input and output of data**
>>
>> *Latest: `9618_w25_qp_13_sc_6.c`*

> [!question] 9618 | Identify the instruction group for each opcode [4]
> Identify the group of instructions that each opcode belongs to.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - `IN` → **input and output of data**
>> - `ADD` → **arithmetic operations**
>> - `JPE` → **unconditional and conditional instructions**
>> - `CMI` → **compare instructions**
>> - `LDD` / `STO` / `MOV` → **data movement**
>>
>> *Latest: `9618_w23_qp_12_sc_9.a`*

> [!question] 9618 | Give an example instruction for each named group [3]
> Give one example instruction for each of the groups named.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - **Data movement** — `LDR #50` // `STO 201` // `LDD 100`
>> - **Arithmetic operation** — `ADD 100` // `INC IX` // `INC ACC`
>> - **Conditional instruction** — `JPE 96` // `JPN 96`
>> - Each instruction **must have a suitable operand** — a bare `LDD` scores nothing
>>
>> *Latest: `9618_w23_qp_11_sc_8.b.i`*

> [!question] 9618 | Write an appropriate instruction for each of the five groups [4]
> Write one appropriate instruction for each of the five groups of instructions.
>
>> [!success]- Answer — 1 mark per group, 4 marks
>> - **Data movement** → `LDM #2`
>> - **Input and output of data** → `IN` or `OUT`
>> - **Arithmetic operations** → `INC ACC` or `INC IX`
>> - **Unconditional and conditional** → `JMP 100` or `JPN 100`
>> - **Compare** → `CMP 100`
>>
>> *Latest: `9618_w21_qp_12_sc_8.b.ii`*

> [!question] 9618 | Name one other group of instructions [1]
> Name one other group of instructions in the processor's instruction set.
>
>> [!success]- Answer — 4 groups available for 1 mark
>> - **Input and output of data**
>> - **Arithmetic operations**
>> - **Unconditional and conditional instructions**
>> - **Compare instructions**
>> - (**Data movement** is the fifth, and is usually the one already given)
>>
>> *Latest: `9618_w22_qp_13_sc_6.c`*

> [!question] Inferred | Explain why instructions are grouped [2]
> Explain why the instructions in a processor's instruction set are arranged in groups.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The set is organised by **function**, so the processor's capabilities are systematic and easy to learn
>> - Instructions in a group share a **similar format**, e.g. the same addressing modes
>> - … so the **Control Unit can decode** them with shared logic
>> - It lets the **assembler check** that an opcode exists in the instruction set during the first pass
>>
>> *Inference: every question is naming or matching; the purpose of grouping is untested.*

---

## 4.2.5 Modes of addressing

> [!question] 9618 | Identify and describe the modes of addressing [4]
> Complete the table by naming and describing each mode of addressing.
>
>> [!success]- Answer — 1 mark for the mode + 1 for the matching description, 4 marks
>> - **Immediate** — the operand **is the data itself**
>> - **Direct** — the operand **is the address of the data**
>> - **Indirect** — the operand points to a memory location that **contains the address** of the data
>> - **Indexed** — the address of the data is formed by **adding the contents of the Index Register to the operand**
>> - **Relative** — the address is calculated from its **distance (offset) from a base address**
>>
>> *Latest: `9618_s25_qp_13_sc_5.a.ii`. The description must **match the mode named** — a mismatched pair scores one, not two.*

> [!question] 9618 | State what is meant by relative addressing [1]
> State what is meant by relative addressing.
>
>> [!success]- Answer — 1 mark
>> - The operand is an **offset value**
>> - … added to a **base value** to give the address from which the contents are loaded into the accumulator
>>
>> *Latest: `9618_w25_qp_12_sc_3.a.i`*

> [!question] 9618 | Write the contents of the ACC after each addressing-mode instruction [3]
> Memory: 98→8, 99→16, 100→3, 101→98, 102→32, and IX = 2. Write the contents of the accumulator after each instruction.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - `LDM #98` → **98** — immediate: the operand **is** the number
>> - `LDI 101` → **8** — indirect: address 101 holds 98, so load the **contents of 98**
>> - `LDX 100` → **32** — indexed: 100 + IX(2) = 102, so load the **contents of 102**
>> - `LDD 100` would give **3** — direct: the contents of address 100
>> - Work the chain **one step at a time** and write down the intermediate address
>>
>> *Latest: `9618_w25_qp_12_sc_3.b`. The most reliable 3 marks in 4.2 — and the easiest to lose by skipping a step.*

> [!question] 9618 | Identify and describe one mode of addressing not in the table [2]
> Identify one mode of addressing not shown in the table and describe it.
>
>> [!success]- Answer — name + description, 2 marks
>> - **Relative** — the operand is an offset added to a base address to give the effective address
>> - **Indirect** — the operand gives a location whose contents are the address of the data
>> - **Indexed** — the contents of IX are added to the operand to give the address of the data
>> - Choose a mode genuinely **absent from the table given**, then describe **that** mode
>>
>> *Latest: `9618_s25_qp_12_sc_7.a.iii`*

> [!question] Inferred | Explain why indexed and indirect addressing exist [3]
> Explain why a processor provides indexed and indirect addressing modes.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Indexed** — one instruction can access **many different locations** by changing IX
>> - … so a loop can **step through an array or table** without rewriting the instruction
>> - … incrementing IX each pass moves to the next element
>> - **Indirect** — the address is held in memory, so it can be **changed while the program runs**
>> - … which allows a program to work on data whose location is not known when it is written
>>
>> *Inference: the modes are described and traced, but never justified. `w21_qp_12_sc_8` gets closest by combining IX with a loop, but the reasoning is never asked for.*

> [!question] SME | State the mechanism of each of the five addressing modes [3]
> State, for each of the five modes of addressing, how the effective address is determined.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Immediate** — the operand is a **constant value** included directly in the instruction; there is no address
>> - **Direct** — the **exact memory address** of the operand is given in the instruction
>> - **Indirect** — a register or memory location **contains the address** of the operand
>> - **Indexed** — a **base address plus an index** (IX) is used to calculate the address
>> - **Relative** — the operand is an **offset relative to the current instruction address**, used in branching
>>
>> *SME's phrasing of the same content 9618 credits; relative is the one worth knowing cold, since it is defined but never traced.*

---

# 4.3 Bit manipulation

> [!danger] No 9608 questions exist for this entire sub-topic
> Every entry below is 9618 or inference. Bit manipulation appears in **every 9618 series**, almost always attached to the assembly-language question.

## 4.3.1 Binary shifts: logical, arithmetic and cyclic

> [!question] 9618 | Perform a logical shift [1]
> Show the result of the logical shift described on the binary number given.
>
>> [!success]- Answer — 1 mark per shift
>> - `0100 1111` **left** logical 2 → **`0011 1100`**
>> - `1100 1100` **right** logical 3 → **`0001 1001`**
>> - `1100 1010` **left** logical 2 → **`0010 1000`**
>> - **Zeros fill** the vacated end; bits shifted off the other end are **discarded**
>>
>> *Latest: `9618_s25_qp_13_sc_7.a.i`*

> [!question] 9618 | Perform an arithmetic right shift on a two's complement negative integer [1]
> Show the result of an arithmetic right shift of 3 places on the two's complement number given.
>
>> [!success]- Answer — 1 mark per shift
>> - `1001 0011` arithmetic right 3 → **`1111 0010`**
>> - `1001 1110` arithmetic right 3 → **`1111 0011`**
>> - The **sign bit is copied** into each vacated leftmost bit, so a negative number stays negative
>>
>> *Latest: `9618_s25_qp_13_sc_7.a.ii` (also `9618_w25_qp_13_sc_2.c`)*

> [!question] 9618 | Show the result of an LSL or LSR instruction [1]
> Show the contents of the accumulator after the instruction given.
>
>> [!success]- Answer — 1 mark per instruction
>> - `0110 1011` after `LSR #5` → **`0000 0011`**
>> - `0101 0011` after `LSL #3` → **`1001 1000`**
>> - `1001 0011` after `LSR #2` → **`0010 0100`**
>> - `LSL` = logical shift **left**, `LSR` = logical shift **right**; the operand is the **number of places**
>>
>> *Latest: `9618_s25_qp_11_sc_8.b.iii`*

> [!question] 9618 | Describe the difference between a right logical and a right arithmetic shift [2]
> Describe the difference between a logical right shift and an arithmetic right shift.
>
>> [!success]- Answer — 1 mark each, 2 marks
>> - A **logical** shift moves all the bits right and **inserts zeros** into the vacated leftmost bits
>> - An **arithmetic** shift moves all the bits right but **copies the sign bit into the Most Significant Bit**
>> - … which preserves the sign of a two's complement number
>> - A **left** arithmetic shift is identical to a left logical shift
>>
>> *Latest: `9618_w24_qp_13_sc_8.c`*

> [!question] 9618 | Write a bit manipulation instruction that produces a given result [1]
> Write the single instruction that changes the accumulator from `0001 1110` to `0111 1000`.
>
>> [!success]- Answer — 1 mark
>> - **`LSL #2`**
>> - Count the places the 1-bits have **moved**, and the direction, then choose LSL or LSR
>> - Check that **no 1 bits would be lost** off the end — if any would be, the shift is not the answer
>>
>> *Latest: `9618_w25_qp_11_sc_4.a`*

> [!question] Inferred | Perform a cyclic shift [1]
> Show the result of a 3-place cyclic left shift on the binary number `1011 0001`.
>
>> [!success]- Answer — 1 mark
>> - `1011 0001` cyclic left 3 → **`1000 1101`**
>> - The bits that fall off the **left** end reappear at the **right** end, in order
>> - **Nothing is lost and no zeros are added** — the number of 1 bits is unchanged
>> - A cyclic right shift works the same way in the opposite direction
>>
>> *Inference: the syllabus notes name "**logical, arithmetic and cyclic**". Logical shifts are examined every series and arithmetic shifts twice in w25/s25 — **cyclic shifts have never been examined in 9618**, and there is no 9608 fallback. There is no cyclic opcode in the standard instruction set, so it would be asked as a written shift, exactly as above. This is the single clearest gap in Chapter 4.*

> [!question] Inferred | Explain the use of shifts for multiplication and division [3]
> Explain how binary shifts can be used to multiply and divide, and why a programmer might use a shift rather than a multiply instruction.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Each **left shift doubles** the value — `0000 1110` (14) left 2 → `0011 1000` (56)
>> - Each **right shift halves** it — `1100 1000` (200) right 3 → `0001 1001` (25)
>> - An **arithmetic right shift** divides a signed number by 2 while **preserving the sign**
>> - … `1110 1000` (−24) arithmetic right 3 → `1111 1101` (−3), rounding towards negative infinity
>> - A shift is a **single, very fast operation**, far quicker than a multiply or divide instruction
>>
>> *Inference: never asked in 9618, and it tests understanding rather than mechanics — which is exactly the kind of question the newer papers favour.*

> [!question] Inferred | Explain what is lost in a binary shift [2]
> Explain what happens to the bits that are shifted out of an 8-bit register.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Bits shifted off the end are **discarded** — they are not stored anywhere
>> - A **left shift** can therefore cause **overflow**, if a 1 is shifted out of the MSB
>> - … so the value is no longer double the original
>> - A **right shift** loses the least significant bits, so **precision is lost** on an odd number
>> - A **cyclic** shift is the exception — nothing is lost
>>
>> *Inference: `w25_qp_11_sc_4.a` requires a shift that happens **not** to lose a 1 bit; a question where it does has not been set.*

> [!question] SME | Compare the three types of shift [3]
> Describe the three types of binary shift and state when each is used.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Logical** — moves the bits and fills the gap with **0s**; used for unsigned numbers and raw bit manipulation
>> - **Arithmetic left** — identical to a logical left shift
>> - **Arithmetic right** — **copies the sign bit (MSB)** into the new leftmost bit, preserving the sign of a two's complement number
>> - **Cyclic** — rotates the bits around: **nothing is lost and no 0s are added**
>> - Worked: `0000 1110` (14) left 2 → `0011 1000` (56); `1100 1000` (200) right 3 → `0001 1001` (25)
>>
>> *Covers the whole bullet, including the untested cyclic third.*

---

## 4.3.2 Bit manipulation to monitor and control a device (masking)

> [!question] 9618 | Write an instruction to set a specific bit to 1 [2]
> Write the instruction(s) needed to set the most significant bit of the accumulator to 1, leaving all other bits at 0.
>
>> [!success]- Answer — 1–2 marks depending on the bit required
>> - To set the **least significant** bit only: `OR B00000001` // `OR #1` // `OR &1`
>> - To set **only the most significant** bit, when the register may contain any 8-bit value, **two instructions** are needed:
>> - … `AND B00000000` — clear every bit first
>> - … then `OR B10000000` — set the MSB
>> - Also accepted: `AND #0 / OR #128`, or `AND &0 / OR &80`
>> - **OR with a 1 sets that bit; OR with a 0 leaves it unchanged**
>>
>> *Latest: `9618_s25_qp_13_sc_5.b` (also `9618_s25_qp_11_sc_8.b.i`)*

> [!question] 9618 | Explain how bit manipulation can clear a register, and write the instruction [3]
> Explain how bit manipulation can be used to check that a register has been cleared, and write the instruction required.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A bit manipulation operation is required to **set all the bits to zero**
>> - The result of the masking is then **compared with 0**
>> - The result of the comparison will be **true if the register is cleared**
>> - Instruction: **`AND B00000000`** // `AND #00` // `AND &00`
>> - **AND with a 0 clears that bit; AND with a 1 leaves it unchanged**
>>
>> *Latest: `9618_w24_qp_13_sc_7.b`. The three-part structure — which bits, the mask, the comparison — is what the mark scheme rewards.*

> [!question] 9618 | Explain how bit manipulation can test a bit, and write the instruction [3]
> Explain how bit manipulation can be used to test whether the number in the accumulator is odd, and write the instruction required.
>
>> [!success]- Answer — 5 points for 3 marks
>> - An odd binary number has a **1 in the Least Significant Bit**
>> - A bit manipulation operation is required to **mask only the LSB and clear all the others**
>> - The result of the masking is **compared with denary 1**
>> - The result of the comparison will be **true if the number is odd**
>> - Instruction: **`AND B00000001`** // `AND #1` // `AND &01`
>>
>> *Latest: `9618_w24_qp_12_sc_8.b.ii`*

> [!question] 9618 | Write the accumulator contents after a bitwise instruction [1]
> Write the contents of the accumulator after the instruction shown.
>
>> [!success]- Answer — 1 mark per instruction
>> - `1111 0000` then `OR B00001111` → **`1111 1111`**
>> - `0001 1101` then `XOR #30` → **`0000 0011`** (30 = `0001 1110`)
>> - `0101 0101` then `XOR &FE` → **`1010 1011`** (FE = `1111 1110`)
>> - **Convert the operand to binary first**, then apply the operation bit by bit
>>
>> *Latest: `9618_s25_qp_12_sc_7.b.i`*

> [!question] 9618 | Complete a table of accumulator contents after each set of instructions [3]
> The accumulator is reloaded with `1001 1010` before each row. Complete the table of accumulator contents.
>
>> [!success]- Answer — 1 mark per row, 3 marks
>> - `LSL #2` → **`0110 1000`**
>> - `ADD #5` then `AND #30` → **`0001 1110`**
>> - `OR B11110010` then `INC ACC` → **`1111 1011`**
>> - The accumulator is **reset each row** — do not carry the previous result forward
>>
>> *Latest: `9618_w24_qp_12_sc_8.b.i`*

> [!question] 9618 | Trace a program mixing masks and memory addresses [3]
> The accumulator holds `1111 1111`. Address 100 holds `0000 1101` and address 103 holds `0011 0111`. Write the accumulator contents after each instruction.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - `LSL #2` → **`1111 1100`**
>> - `XOR 100` → **`1111 0010`** (XOR with `0000 1101`)
>> - `AND 103` → **`0011 0111`** (AND with `0011 0111`)
>> - Note that these operands are **addresses**, not immediate values — look up the contents first
>>
>> *Latest: `9618_s24_qp_13_sc_3.b`. Mistaking an address for a value is the most common way to lose all three.*

> [!question] Inferred | Use bit manipulation to monitor a device [3]
> Each bit of an 8-bit register corresponds to one sensor, with bit 0 the least significant. Explain how the program can test whether sensor 3 has been triggered, and write the instruction required.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Sensor 3 corresponds to the bit in **position 3**, i.e. the mask `0000 1000`
>> - A bit manipulation operation is required to **isolate that bit and clear all the others**
>> - The result is **compared with `0000 1000`** (denary 8)
>> - The result of the comparison is **true if that sensor has triggered**
>> - Instruction: **`AND B00001000`** // `AND #8` // `AND &08`
>>
>> *Inference: the bullet reads "show understanding of how bit manipulation can be used to **monitor/control a device**", yet every 9618 question so far uses an abstract register. **No question has placed the register in a device** — despite that being the literal wording and the obvious link to monitoring and control in Chapter 3.*

> [!question] Inferred | Use a mask to clear one specific bit [3]
> Explain how bit manipulation can be used to set bit 3 of the accumulator to 0 while leaving every other bit unchanged, and write the instruction required.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Only **bit 3** is to change; every other bit must keep its current value
>> - **AND with a 0 clears** a bit; **AND with a 1 leaves it unchanged**
>> - So the mask is **all 1s except a 0 in position 3** — `1111 0111`
>> - Instruction: **`AND B11110111`** // `AND #247` // `AND &F7`
>> - The result can then be compared to confirm the bit is clear
>>
>> *Inference: setting a bit (`OR`), clearing the whole register (`AND #0`) and testing a bit (`AND` + compare) have all been examined. Clearing **one** bit while leaving the others alone is the natural fourth member of the set and has not been asked.*

> [!question] Inferred | Use XOR to flip a bit [3]
> Explain how bit manipulation can be used to toggle bit 0 of the accumulator, and write the instruction required.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Toggling means a 1 becomes 0 and a 0 becomes 1, leaving the other bits unchanged
>> - **XOR with a 1 flips** that bit; **XOR with a 0 leaves it unchanged**
>> - So the mask has a **1 only in the position to be toggled** — `0000 0001`
>> - Instruction: **`XOR B00000001`** // `XOR #1` // `XOR &01`
>> - Applying the same instruction a second time **returns the bit to its original value**
>>
>> *Inference: XOR appears constantly as a traced instruction, but no question asks candidates to **use** it purposefully. Given that set, clear and test all have "explain and write the instruction" questions, toggle is the missing one.*

> [!question] SME | State the three masking rules and the answer structure they require [3]
> State the effect of using OR, AND and XOR as masks, and describe how a masking answer should be structured.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **OR** with a 1 **sets** that bit to 1; OR with a 0 leaves it unchanged
>> - **AND** with a 0 **clears** that bit to 0; AND with a 1 leaves it unchanged
>> - **XOR** with a 1 **flips** that bit; XOR with a 0 leaves it unchanged
>> - The structure 9618 rewards is three-part: say **which bits matter** · say that a **mask is applied** to isolate or change them · say that the result is **compared** with an expected value to give a true/false outcome
>> - Then **give the instruction**, in binary, denary or hex form
>>
>> *Learn these three lines and the structure, and every masking question in 4.3.2 becomes the same question.*
