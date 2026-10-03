---
title: Pack — 3 Hardware (AS Level)
syllabus: 9618 (2026)
topics: 3.1 Computers and their components · 3.2 Logic Gates and Logic Circuits
pairs with: Jigsaw
---

# Pack — 3 Hardware

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **9608 |** — same rule, using 9608 tariffs. Still inside the 9618 syllabus wording, but untested in the current series.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

> [!danger] Two sub-topics have no 9608 safety net
> **Embedded systems** (3.1.2) and **PROM / EPROM / EEPROM** (3.1.7) do not appear in the 9608 Legend at all. Every entry for them below is 9618 or inference — and embedded systems has been examined in almost every series since 2021.

> [!note] 3.2 is a skills sub-topic
> The tariffs there are fixed and predictable: **draw a circuit from an expression = 2**, **complete a truth table = 2** (marked in blocks of four rows), **write an expression from a circuit = 2–3**. Practise the format, not the recall.

---

# 3.1 Computers and their components

## 3.1.1 The need for input, output, primary memory and secondary storage

> [!question] 9618 | Explain how the amount of RAM affects the performance of a computer [3]
> Explain how the amount of RAM installed in a computer affects its performance.
>
>> [!success]- Answer — 5 points for 3 marks
>> - More RAM means **more of the currently running data and instructions** can be held in memory
>> - … so there is no need to use **virtual memory**
>> - … and data does not have to be fetched from **secondary storage** first
>> - Secondary storage has a much **slower access time** than RAM
>> - So there is **less latency / delay** waiting for instructions or data, and performance improves
>>
>> *Latest: `9618_s25_qp_11_sc_6.a.ii`*

> [!question] 9618 | Identify what a device stores in primary memory [2]
> Identify two items of data or instructions that a device stores in its primary memory.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **current reading / data from the sensor**
>> - The **current or recent video** footage
>> - The **instructions currently being executed**
>> - The **start-up / BIOS / boot-up instructions** (in ROM)
>>
>> *Latest: `9618_s24_qp_11_sc_2.c.i`*

> [!question] 9618 | Describe two hardware upgrades that would improve performance, and explain each [4]
> Describe two ways in which the hardware of a computer could be upgraded to improve its performance. Explain how each upgrade improves performance.
>
>> [!success]- Answer — 2 marks per upgrade (change + effect), 4 marks
>> - Increase the **number of cores**
>> - … each core can independently carry out a process at the same time, so more instructions are performed **in parallel**
>> - Increase **RAM capacity**
>> - … so more applications can reside in memory at once, saving slow disk access
>> - Increase **cache memory**
>> - … more data is held in fast-access memory, so less time is spent accessing RAM
>> - Increase the **clock speed**
>> - … so more Fetch–Decode–Execute cycles are carried out per unit of time
>>
>> *Latest: `9618_s23_qp_12_sc_5.b`*

> [!question] 9618 | Justify the use of magnetic storage rather than solid state [4]
> A server stores a large number of video files, which are read and written continuously. Justify the use of magnetic storage rather than solid-state storage.
>
>> [!success]- Answer — 2 points + expansions, 4 marks
>> - **Lower cost per unit of storage**
>> - … so the high capacity required for a large number of video files is less costly
>> - A large number of **read/write operations** are performed continuously
>> - … and magnetic storage is likely to have a **longer life span** than solid state, which has a limited number of write cycles
>> - Very large capacities are available in a single drive
>>
>> *Latest: `9618_w25_qp_13_sc_7.d` (also `9618_s23_qp_11_sc_4.b`)*

> [!question] 9608 | Identify an appropriate input or output device for each use [5]
> Complete the table by identifying the most appropriate input or output device for each described use.
>
>> [!success]- Answer — 1 mark per row, 5 marks
>> - Entering a credit card number into an online form → **keyboard / keypad**
>> - Selecting an option at an airport check-in kiosk → **touch screen**
>> - Printing a single high-quality photograph → **inkjet printer**
>> - Printing several hundred high-quality leaflets → **laser printer**
>> - Inputting a hard-copy image into a computer → **scanner**
>>
>> *Latest: `9608_s15_qp_12_sc_6.a`. The device-selection table is a 9608 staple with no 9618 equivalent — note that the printer answer flips on **volume**, not quality.*

> [!question] Inferred | Justify the use of solid-state storage rather than magnetic [4]
> A laptop is used by a field engineer who travels constantly. Justify the use of solid-state storage rather than magnetic storage.
>
>> [!success]- Answer — 2 points + expansions, 4 marks
>> - Solid state has **no moving parts**
>> - … so it is far more resistant to being dropped or knocked while travelling
>> - It has a **faster access time**
>> - … so files open and the laptop boots more quickly
>> - It uses **less power**, so the battery lasts longer
>> - It is **smaller, lighter and silent**, suiting a portable device
>>
>> *Inference: both 9618 questions run the argument one way — why magnetic beats solid state for a server. Every point above already exists in those mark schemes as the rejected side, so the reverse question is set-ready at the same 4-mark tariff.*

> [!question] Inferred | Explain why a computer needs secondary storage [3]
> Explain why a computer system needs secondary storage.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Secondary storage is **non-volatile**
>> - … so data and programs are **retained when the power is turned off**, unlike RAM
>> - It has a much **larger capacity** than primary memory
>> - … so it holds all the files and software **not currently in use**
>> - It costs far **less per unit of storage** than RAM
>>
>> *Inference: every 9618 question here is a comparison between storage **types**. The bullet's actual wording — the *need* for secondary storage — is untested.*

> [!question] SME | Describe the factors to consider when choosing a storage device [4]
> Describe the factors a user should consider when choosing a storage device.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Capacity** — how much data must be stored, now and in future
>> - **Performance** — whether fast access is needed (SSD for video editing or gaming)
>> - **Portability** — whether the data must be moved between machines (USB flash or external drive)
>> - **Cost** — higher capacity and faster devices cost more per unit
>> - **Durability** — moving parts make magnetic drives vulnerable to shock
>> - The same structure fits input/output devices: **user needs, user skills, environment, cost**
>>
>> *A skeleton for any "recommend a device and justify" question; 9618 marks such justifications at up to 4.*

> [!question] SME | State typical capacities and trade-offs of the main storage media [4]
> State a typical capacity for each of four storage media and give one trade-off for each.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **HDD** 500 GB – 2 TB — low cost per GB, but moving parts make it fragile
>> - **SSD** 120 GB – 4 TB — very durable and fast, but a high cost per GB
>> - **USB flash drive** 8 – 256 GB — very portable, but small capacity and easily lost
>> - **CD** 700 MB, **DVD** 4.7 – 9 GB, **Blu-ray** 25 – 50 GB — cheap per disc, but easily scratched
>> - Optical media are read-only or write-once in many formats
>> - Figures are not themselves credited, but they make "high capacity" and "cost per unit" concrete
>>
>> *SME supplies the numbers; the trade-off half is what 9618 actually marks.*

---

## 3.1.2 Embedded systems

> [!question] 9618 | Describe what is meant by an embedded system, using an example [3]
> Describe what is meant by an embedded system. Use an example in your answer.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A **microprocessor / microcontroller within a larger system**
>> - … that performs **one specific task**
>> - **Example:** the embedded system in a washing machine only controls the programs for the washing cycle
>> - … it is part of the washing machine but performs **no other function** within it
>> - It is a combination of dedicated hardware and software
>>
>> *Latest: `9618_s21_qp_11_sc_5.a`*

> [!question] 9618 | Identify the features of an embedded system [3]
> Identify three characteristics of an embedded system.
>
>> [!success]- Answer — 7 points for 3 marks
>> - **Dedicated to a single task** // has a limited number of functions
>> - **Built into / integrated into a larger system**
>> - Contains a processor, memory and I/O capability // uses **dedicated hardware**
>> - Hardware and software are designed together for a **specific function**
>> - **Not easily changed or updated** by the owner
>> - Does **not require much processing power**
>> - Usually has **no operating system** of its own
>>
>> *Latest: `9618_w23_qp_12_sc_1.c.i` (also `9618_w22_qp_13_sc_10.b.ii`)*

> [!question] 9618 | Identify the characteristics of a described device that make it an embedded system [3]
> A device contains sensors, a camera and software dedicated to one task. Identify the characteristics that suggest it is an embedded system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The device only performs the **specific tasks described**
>> - The sensors and camera are **built into** it
>> - The CPU, memory, storage and software are **dedicated to this task only**
>> - Only a **dedicated microprocessor** is needed, because the processing requirements are limited
>> - The user cannot install other software on it
>>
>> *Latest: `9618_s24_qp_11_sc_2.a`. Each point must be **applied to the device given** — generic characteristics score nothing.*

> [!question] 9618 | Give an example of an embedded system and explain why it is one [3]
> Give one example of an embedded system and explain why it is an embedded system.
>
>> [!success]- Answer — 5 points for 3 marks, each applied to the example
>> - **Example:** a central heating thermostat / satnav / traffic light controller
>> - It is **dedicated to one task** — for example, maintaining the set room temperature
>> - It does **not require much processing power**
>> - It is **built into a larger system** (the heating system), not used on its own
>> - It contains **firmware that cannot easily be updated** by the user
>>
>> *Latest: `9618_w23_qp_11_sc_9.b`. Have an example ready that is **not** the one in the question — examined scenarios so far are a video doorbell, a car alarm, a television, a washing machine and factory machinery.*

> [!question] 9618 | Describe the drawbacks of embedded systems [3]
> Describe the drawbacks of using embedded systems.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The **firmware is difficult to change or update** by the user // hard to upgrade to newer technology
>> - **Errors cannot be fixed easily** // troubleshooting and repair are specialist and expensive
>> - **Functionality cannot be extended** // it cannot be adapted for another task
>> - Faulty or outdated devices are often **thrown away rather than repaired**
>> - … contributing to **e-waste**
>>
>> *Latest: `9618_w24_qp_12_sc_2.a`*

> [!question] 9618 | Explain why ROM is used in an embedded system [3]
> Explain the reasons why ROM is used in an embedded system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - To **store data that does not change**
>> - The data must be **retained when the device has no power** // it is non-volatile
>> - It stores the **boot-up instructions / system software / firmware / BIOS**
>> - The contents cannot be accidentally overwritten by the user
>> - Only a small capacity is needed, so it is cheap
>>
>> *Latest: `9618_w22_qp_12_sc_3.c`*

> [!question] Inferred | Describe the benefits of embedded systems [3]
> Describe the benefits of using an embedded system in a device.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Small and compact**, so it fits easily inside the host device
>> - **Low power consumption**, so it is efficient and cheap to run
>> - **Cheaper to produce**, because minimal dedicated hardware is needed
>> - **Fast and reliable** at the repetitive task it is designed for
>> - Operates in **real time**, which suits time-critical jobs such as alarms and braking
>>
>> *Inference: 9618 has asked for the drawbacks at 3 marks and the characteristics repeatedly, but never for the benefits. The inverse of an existing question, at the same tariff, is overdue.*

> [!question] SME | Compare the benefits and drawbacks of embedded systems [4]
> Discuss the benefits and drawbacks of using embedded systems.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Benefit:** small, compact and easily fitted into a dedicated device
>> - **Benefit:** low power consumption and cheap to produce, using minimal hardware
>> - **Benefit:** fast, reliable and real-time for repetitive, time-sensitive tasks
>> - **Drawback:** limited functionality, memory and processing power
>> - **Drawback:** hard to upgrade or repair, being built into the device
>> - **Drawback:** may be **less secure**, with limited protection if connected to other systems
>>
>> *The security point is in no mark scheme but is a defensible modern drawback. 9618 marks two-sided "discuss" questions at 4.*

---

## 3.1.3 Principal operations of hardware devices

> [!question] 9618 | Complete the description of a magnetic hard disk [4]
> Complete the description of the principal operation of a magnetic hard disk drive.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The disk has one or more **platters** that can be magnetised
>> - These are mounted on a **spindle** and rotate at high speed
>> - A **read/write head** is moved across the surface on an arm
>> - When data is read, changes in the **magnetic field** produce a change in the electric current
>> - When data is written, the head magnetises areas of the platter
>> - The platters are divided into **tracks and sectors**, so data can be addressed
>>
>> *Latest: `9618_s25_qp_11_sc_6.a.i`*

> [!question] 9618 | Describe the principal operation of an optical disc reader/writer [5]
> Describe the principal operation of an optical disc reader/writer.
>
>> [!success]- Answer — 7 points for 5 marks
>> - The disc is **spun at high speed**
>> - A **laser** is shone onto the surface of the disc to read or write
>> - An **optical head** moves the laser into position
>> - It follows the **spiral track**, from the centre outwards
>> - When writing, the laser **burns pits** to represent the data
>> - When reading, the laser **reflects** from the pits and lands
>> - The reflection from a pit differs from that of a land, and the difference is interpreted as **1 or 0**
>>
>> *Latest: `9618_w24_qp_11_sc_3.d.i`*

> [!question] 9618 | Describe the principal operation of a touchscreen [4]
> Describe the principal operation of a touchscreen.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Resistive:** the screen has two conductive layers separated by a gap
>> - … pressure makes the layers touch, **completing a circuit** at that point
>> - **Capacitive:** the screen holds an electrical charge
>> - … a finger changes the **charge / electric field** where it touches
>> - The **point of contact is identified** from that change
>> - The microprocessor / software **calculates the coordinates** of the touch
>>
>> *Latest: `9618_s24_qp_13_sc_7.d`*

> [!question] 9618 | Explain how a touchscreen converts a touch into a menu selection [4]
> Explain how a touchscreen detects a user's touch and converts it into a menu selection.
>
>> [!success]- Answer — max 2 for detection, max 2 for selection, 4 marks
>> - **Detection — resistive:** two layers make contact and complete a circuit
>> - **Detection — capacitive:** the contact creates a change in charge
>> - **Detection — infra-red:** the beams across the screen are broken
>> - **Detection — optical imaging / acoustic pulse:** a shadow is created // the wave is absorbed
>> - **Selection:** the point of touch determines the **x and y coordinates**
>> - The menu item **corresponding to those coordinates** is recognised and added to the order
>>
>> *Latest: `9618_w25_qp_12_sc_8.b.i`. Two halves — an answer that only describes the technology caps at 2.*

> [!question] 9618 | Complete the description of touchscreen types [4]
> Complete the description of resistive and capacitive touchscreens.
>
>> [!success]- Answer — 5 points for 4 marks
>> - A **resistive** touchscreen has **two layers**
>> - … when touched, the layers make contact and a **circuit** is completed
>> - A **capacitive** touchscreen has several layers
>> - … when the top layer is touched there is a **change in the electric current / charge**
>> - A **microprocessor** identifies the **coordinates** of the touch
>>
>> *Latest: `9618_s23_qp_13_sc_3.a`*

> [!question] 9618 | Explain how a model is printed using a 3D printer [4]
> Explain how a model is produced using a 3D printer.
>
>> [!success]- Answer — max 3 generic + max 1 specific, 4 marks
>> - It uses **additive manufacturing**
>> - The design comes from a digital file created with 3D modelling or **CAD** software
>> - The printer builds the model **one layer at a time**, from the bottom up, using x, y and z coordinates
>> - The process is **repeated for each layer**, fusing or curing it to the one below
>> - Some materials need time to **cool and set**, or UV curing using LEDs
>> - **Specific (max 1):** FDM — material is heated and pushed through a nozzle / extruder
>> - **Specific:** SLA — photosensitive liquid resin is exposed to a UV laser; DLP — resin exposed to a projected UV image; SLS — a laser fuses powdered material
>>
>> *Latest: `9618_w25_qp_11_sc_10.a` (also `9618_w23_qp_11_sc_7.a`). Only **one** mark is available for the named technology — the generic process carries the answer.*

> [!question] 9618 | Describe the principal operation of a microphone [3]
> Describe the principal operation of a microphone.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The microphone contains a **diaphragm / ribbon**
>> - Incoming **sound waves cause it to vibrate**
>> - The vibration causes a **coil to move past a magnet** (dynamic)
>> - … or changes the **capacitance** (condenser), or deforms a **crystal** (crystal microphone)
>> - This produces an **electrical signal**, which varies with the sound
>>
>> *Latest: `9618_w21_qp_12_sc_3.a`*

> [!question] 9618 | Complete the description of a VR headset [4]
> Complete the description of how a virtual reality headset works.
>
>> [!success]- Answer — 6 points for 4 marks
>> - A headset has one or two **LCD displays / screens / lenses** that output the image
>> - Head movements are detected using a **sensor**
>> - … a **gyroscope** and/or **accelerometer**
>> - The data is analysed by a **microprocessor**
>> - … to identify the **direction and speed** of movement
>> - Some headsets use **digital cameras** that record the user's eye movements
>>
>> *Latest: `9618_s24_qp_12_sc_2.a`*

> [!question] 9618 | Complete the table on solid state (flash) memory [4]
> Complete the table about the construction of solid-state memory.
>
>> [!success]- Answer — 1 mark per row, 4 marks
>> - The two types of logic gate used to create solid-state devices → **NAND** and **NOR**
>> - The number of transistors in each cell → **2**
>> - The type of gate that retains electrons without power → **floating** gate
>> - The type of gate that allows or stops current passing through → **control** gate
>>
>> *Latest: `9618_s24_qp_11_sc_2.c.ii`*

> [!question] Inferred | Describe the principal operation of a laser printer [4]
> Describe the principal operation of a laser printer.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The page image is drawn by a **laser** onto a **photosensitive drum**
>> - … the laser changes the **electric charge** wherever it strikes the drum
>> - **Toner powder** is attracted to the charged areas of the drum
>> - … forming the shape of the text or image
>> - The drum **rolls the toner onto the paper** as it passes
>> - The paper passes through **hot fusing rollers**, melting the toner permanently onto it
>>
>> *Inference: the laser printer appears repeatedly in 9618, but only ever as the setting for a **buffer** question (`w23_qp_13_sc_7.c`). Its own operation is named in the syllabus notes and has never been asked — an obvious gap at the same 4-mark tariff as the other device questions.*

> [!question] Inferred | Describe the principal operation of a speaker [3]
> Describe the principal operation of a loudspeaker.
>
>> [!success]- Answer — 5 points for 3 marks
>> - An **electrical signal** is sent to the speaker
>> - … and passed through a **coil that acts as an electromagnet**
>> - The changing current changes the magnetic field, making the coil **move back and forth** against a permanent magnet
>> - The coil is attached to a **cone / diaphragm**, which vibrates with it
>> - The vibrating cone moves the air, producing **sound waves**
>>
>> *Inference: named in the syllabus notes alongside the microphone, and the microphone **has** been examined. The speaker is its mirror image and is untested in 9618.*

> [!question] SME | Describe how a solid-state memory cell stores data [4]
> Describe how one cell of solid-state memory stores a bit of data.
>
>> [!success]- Answer — 6 points for 4 marks
>> - Each cell contains a **transistor acting as a switch**, holding one bit
>> - The **control gate** is the top layer — it connects to the circuit and controls whether current flows
>> - The **floating gate** sits between two **insulating oxide layers** and holds the charge
>> - To **store** data, a high voltage on the control gate pushes electrons through the oxide onto the floating gate
>> - To **erase**, a high voltage in the opposite direction pulls the electrons off
>> - The charge stays on the floating gate **without power**, which is why the memory is non-volatile
>>
>> *SME supplies the mechanism behind the four one-word answers credited in `s24_qp_11_sc_2.c.ii`.*

> [!question] SME | Describe how a hard disk is organised [3]
> Describe how the surface of a magnetic hard disk is organised and accessed.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Each platter is divided by concentric circles into **tracks**
>> - … and by wedge shapes into **sectors**
>> - The intersection of a track and a sector is a **track sector**, the smallest addressable unit
>> - The disk spins at typically **5400–7200 RPM**
>> - A read/write arm controlled by an **actuator** positions the head, which reads and writes using **electromagnets**
>>
>> *Tracks and sectors are not in the 9618 cloze but are standard credited detail elsewhere.*

> [!question] SME | Match the type of microphone and touchscreen to a scenario [4]
> For each scenario, identify the most suitable type of microphone or touchscreen and justify your choice.
>
>> [!success]- Answer — 2 marks per scenario (choice + justification), 4 marks
>> - **Loud live environment → dynamic microphone** … it is robust and handles high sound levels without distorting
>> - **Recording studio → condenser microphone** … it is far more sensitive and captures fine detail
>> - **Smartphone or tablet → capacitive touchscreen** … it reacts to the charge in a finger, supports multi-touch and gives a brighter image
>> - **ATM or till → resistive touchscreen** … it responds to pressure, so it works with gloves or a stylus and is cheaper and more durable
>>
>> *Knowing which type suits which scenario is what turns a generic description into an applied answer.*

---

## 3.1.4 The use of buffers

> [!question] 9618 | Explain how a memory buffer is used when transferring data to a hard disk [3]
> Explain how a memory buffer is used when data is transferred from a computer to a hard disk drive.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The computer and the hard disk transmit and receive at **different speeds**
>> - … the computer transfers data faster than the drive can receive it
>> - The buffer provides **temporary storage** for the data
>> - … so the computer can transfer data into the buffer at the higher speed, and is **not held up waiting**
>> - Data is then transferred from the buffer to the hard disk at its own **slower rate**
>>
>> *Latest: `9618_w24_qp_13_sc_2.b`*

> [!question] 9618 | Explain the use of a buffer when writing to an optical disc [3]
> Explain how a buffer is used when data is written to an optical disc.
>
>> [!success]- Answer — 6 points for 3 marks
>> - The computer and the optical disc reader/writer send and receive at **different speeds**
>> - The buffer allows **temporary storage** of the data
>> - … so the computer transfers data at the higher speed and is not held up
>> - … and can **carry on with other tasks** meanwhile
>> - The optical drive is **not overloaded** with data it cannot yet write
>> - Data is transferred from the buffer to the drive at the **slower rate**
>>
>> *Latest: `9618_w24_qp_11_sc_3.d.ii`*

> [!question] 9618 | Describe how a laser printer makes use of a buffer [4]
> Describe how a laser printer makes use of a buffer when printing a document from a laptop.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The print instructions and data are sent by the laptop to the **buffer**, at laptop speed
>> - The data is transferred from the buffer to the printer at **printer speed**
>> - This allows the user to **continue using the laptop**
>> - … and the processor to continue processing other tasks
>> - … instead of waiting for the relatively **slower printer**
>> - When the buffer is **empty**, an **interrupt** is sent to the laptop requesting more data
>>
>> *Latest: `9618_w23_qp_13_sc_7.c`*

> [!question] 9618 | Explain how a buffer is used when transmitting data to a peripheral [4]
> Explain how a buffer is used when a computer transmits data to a peripheral device.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The buffer is a **temporary store** for data on its way to the device
>> - Data is **transferred into** the buffer by the computer
>> - Data is **retrieved from** the buffer by the device
>> - … each working at its own speed, independently of the other
>> - When the buffer is **empty**, an **interrupt** is sent to the computer requesting more data
>> - When the buffer is **full**, an interrupt stops further data being sent
>>
>> *Latest: `9618_s24_qp_12_sc_2.b`*

> [!question] 9618 | Explain the purpose of a buffer and give an example of its use [3]
> Explain the purpose of a buffer and give one example of where a buffer is used.
>
>> [!success]- Answer — max 2 purpose + max 1 example, 3 marks
>> - **Purpose:** to act as **temporary storage** for data // to store downloaded data
>> - … before it is used by the receiving device
>> - … so that processes or devices can operate at **different speeds**, independently of each other
>> - **Example:** a printer buffer holding a document while the processor moves on
>> - **Example:** a video buffer while streaming; a keyboard buffer during data entry
>>
>> *Latest: `9618_w22_qp_13_sc_1.c`. Three purpose points will still only score 2 — the example mark must be taken.*

> [!question] 9618 | State why a 3D printer needs a buffer [1]
> State one reason why a 3D printer needs a buffer.
>
>> [!success]- Answer — 3 points for 1 mark
>> - To **free up the processor** to carry out other tasks
>> - … because the rate at which the printer receives data differs from the rate at which it can process it
>> - To manage the **mismatch in speed** between the processor and the peripheral
>>
>> *Latest: `9618_w25_qp_11_sc_10.b`*

> [!question] 9618 | Describe the roles of the address bus, the data bus and buffers when writing to a device [3]
> Describe the role of the address bus, the data bus and buffers when data is written to a device.
>
>> [!success]- Answer — 1 mark per component, 3 marks
>> - **Buffers** — temporarily hold the data until it is ready to be transmitted **to the device**
>> - **Address bus** — carries the address (in RAM) of the **data to be written to the device**
>> - **Data bus** — carries all the **data to be written to the device / buffer**
>> - Each mark must name what is carried **to the device**, not generically
>>
>> *Latest: `9618_w23_qp_12_sc_8.c.ii`*

> [!question] 9608 | Describe the sequence of events when a file is read from a hard disk [8]
> Describe the sequence of events that takes place when an application program reads a file from the hard disk, including the use of the disk buffer.
>
>> [!success]- Answer — 10 points for 8 marks
>> - The application program **executes a read statement**
>> - … which passes the request to the **operating system**
>> - The OS **spins the disk** up to speed
>> - It **looks up the track and sector** in the directory file
>> - The read/write **head moves to the correct track**
>> - It **waits for the correct sector** to rotate beneath it
>> - The first **cluster is read into the disk buffer**
>> - Successive clusters continue to be read into the buffer
>> - An **interrupt is generated** when the transfer is complete
>> - The OS **transfers the buffer contents** into the program's data area in memory
>>
>> *Latest: `9608_w16_qp_12_sc_3`. An 8-mark sequencing question with no 9618 equivalent — the same question also anchors the Chapter 5 Pack.*

> [!question] 9608 | Explain how buffering allows a streamed video to play without pausing [4]
> Explain how buffering allows a streamed video to play without pausing.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The user needs a **high-speed broadband** connection
>> - Data is **streamed into a buffer** in the computer before it is played
>> - Playback begins only once the buffer holds **enough data**
>> - Buffering stops the video pausing as further bits are streamed
>> - As the buffer **empties it is refilled**, so viewing is continuous
>> - Actual playback is a **few seconds behind** the time the data is received
>>
>> *Latest: `9608_w16_qp_13_sc_6`. Filed under buffers in 9608 and under bit streaming in Chapter 2 — cross-check with the Communications Pack.*

> [!question] Inferred | Explain the relationship between buffers and interrupts [3]
> Explain how buffers and interrupts work together when a computer sends data to a peripheral.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Data is placed in the **buffer** by the computer and drawn from it by the device
>> - When the buffer becomes **empty**, the device raises an **interrupt**
>> - … which is a signal to the processor requesting **more data**
>> - The processor **finishes its current instruction**, saves its state, and runs the interrupt service routine to refill the buffer
>> - When the buffer is **full**, an interrupt tells the computer to **stop sending**, so no data is lost
>>
>> *Inference: "when the buffer is empty an interrupt is sent" is a mark point in three separate 9618 questions but has never been the subject of one. It is the natural synoptic bridge to Chapter 4.*

---

## 3.1.5 Differences between RAM and ROM

> [!question] 9618 | Describe the contents of ROM in a computer [2]
> Describe what is stored in the ROM of a computer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The **bootstrap program** // the start-up instructions for that computer
>> - The **BIOS**
>> - The start-up instructions for the **attached system** // the **firmware**
>> - The **kernel** // parts of the operating system
>>
>> *Latest: `9618_s23_qp_11_sc_4.a.i`*

> [!question] 9618 | State the purpose of RAM and ROM in an embedded system [2]
> State the purpose of the RAM and of the ROM in an embedded system.
>
>> [!success]- Answer — 1 mark each, 2 marks
>> - **RAM** — stores the choices / program the user has entered
>> - … stores the data read from the sensors, and the time left in the current program
>> - **ROM** — stores the **start-up instructions / firmware**
>> - Any answer given **by example from the scenario** is credited
>>
>> *Latest: `9618_s21_qp_11_sc_5.b`*

> [!question] 9608 | Describe three differences between RAM and ROM [3]
> Describe three differences between RAM and ROM.
>
>> [!success]- Answer — 5 points for 3 marks
>> - RAM is **volatile** — it loses its contents when the power is off; ROM is **non-volatile**
>> - RAM can be **written to and altered**; ROM is **read only** and cannot be changed in normal use
>> - RAM stores the **files, data and operating system currently in use**; ROM stores the **BIOS / bootstrap / pre-set instructions**
>> - RAM is usually **much larger in capacity** than ROM
>> - RAM is **faster** to access than ROM
>>
>> *Latest: `9608_s15_qp_13_sc_4.b` (3 marks; also `9608_w16_qp_12_sc_6.a` at 2). **9618 has only ever asked what each one stores — never the differences — despite the bullet being titled "explain the differences".** This is the most likely gap in the whole chapter to be filled.*

> [!question] 9608 | Describe the purpose of the RAM and ROM in a named peripheral [4]
> Describe the purpose of the RAM and the ROM inside a laser printer.
>
>> [!success]- Answer — max 2 for each, 4 marks
>> - **RAM** — stores the currently running parts of the **printer software**
>> - … stores the **data being printed** / the contents of the buffer
>> - … stores the **current progress** of the print job and data such as toner levels
>> - **ROM** — stores the printer's **operating software** and **boot-up instructions**
>> - … stores the printer's built-in **fonts**
>>
>> *Latest: `9608_s20_qp_13_sc_2.b`*

> [!question] Inferred | State two differences between RAM and ROM, focusing on volatility [2]
> State two differences between RAM and ROM.
>
>> [!success]- Answer — 4 points for 2 marks
>> - RAM is **volatile** — its contents are lost when power is removed
>> - ROM is **non-volatile** — its contents are retained without power
>> - RAM can be **read from and written to**; ROM is normally **read only**
>> - RAM holds what is **currently in use**; ROM holds **permanent start-up instructions**
>>
>> *Inference: volatile vs non-volatile — the single most important RAM/ROM fact — appears in 9618 only implicitly, as "data must be stored even when the device is without power". A direct "state two differences" would catch anyone who has learned only the 9618 storage-contents answers.*

> [!question] SME | Compare RAM and ROM feature by feature [4]
> Compare RAM and ROM in terms of speed, capacity, contents, access and volatility.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Speed** — RAM very fast; ROM fast but slower than RAM
>> - **Capacity** — RAM gigabytes; ROM megabytes
>> - **Contents** — RAM the programs and data in use; ROM the bootstrap / start-up instructions
>> - **Access** — RAM read and write; ROM read only
>> - **Volatility** — RAM volatile; ROM non-volatile
>> - Both are **primary memory**, directly accessible by the CPU; ROM is a small chip on the motherboard holding the **BIOS**
>>
>> *SME's table form; 9608 marks the equivalent comparison at up to 3, and the extra rows make 4 defensible.*

---

## 3.1.6 Differences between SRAM and DRAM

> [!question] 9618 | State three differences between DRAM and SRAM [3]
> State three differences between DRAM and SRAM.
>
>> [!success]- Answer — 6 points for 3 marks
>> - DRAM requires **refreshing / recharging**; SRAM does not
>> - DRAM stores each bit as a **charge**; SRAM uses a **flip-flop**
>> - DRAM is **less expensive** to manufacture; SRAM is more expensive
>> - DRAM has **slower access speeds**; SRAM is faster
>> - DRAM has a **higher storage density**; SRAM lower
>> - DRAM is used in **main memory**; SRAM in **cache**
>>
>> *Latest: `9618_w25_qp_11_sc_6.c`*

> [!question] 9618 | Identify the advantages of using DRAM instead of SRAM [2]
> Identify two advantages of using DRAM rather than SRAM in a device.
>
>> [!success]- Answer — 4 points for 2 marks
>> - It **costs less** per unit of storage
>> - It has a **higher storage density** // more data can be stored per chip
>> - It has a **simpler design**, using fewer transistors per cell
>> - A **fast access speed is not needed** for this device, so the cheaper option is suitable
>>
>> *Latest: `9618_w24_qp_12_sc_2.b` (also `9618_s23_qp_11_sc_4.a.ii`, `9618_w23_qp_11_sc_7.c`)*

> [!question] 9618 | Identify the disadvantages of using DRAM instead of SRAM [2]
> Identify two disadvantages of using DRAM rather than SRAM.
>
>> [!success]- Answer — 4 points for 2 marks
>> - DRAM requires **constant refresh cycles**, unlike SRAM
>> - … which uses processor time and power
>> - DRAM has a **lower access speed** than SRAM
>> - Its contents are lost more quickly without refreshing, so it is unsuitable for cache
>>
>> *Latest: `9618_w24_qp_11_sc_3.c`*

> [!question] 9618 | Explain why SRAM is used instead of DRAM [3]
> Explain why SRAM is used rather than DRAM in a particular part of a computer.
>
>> [!success]- Answer — 5 points for 3 marks
>> - SRAM has a **faster access time**
>> - … because it does **not need to be refreshed**
>> - It is used on the CPU to improve **cache** speed
>> - … where speed matters far more than capacity or cost
>> - The small capacity needed for cache makes the higher price acceptable
>>
>> *Latest: `9618_w23_qp_13_sc_7.a`*

> [!question] 9608 | Tick whether each statement describes SRAM or DRAM [5]
> Tick to show whether each statement describes SRAM or DRAM.
>
>> [!success]- Answer — 1 mark per row, 5 marks
>> - More expensive to make → **SRAM**
>> - Requires refreshing → **DRAM**
>> - Made from flip-flops → **SRAM**
>> - Has less complex circuitry → **DRAM**
>> - Mainly used in cache memory, where speed is important → **SRAM**
>> - Requires higher power consumption under low levels of access → **DRAM**
>>
>> *Latest: `9608_w18_qp_13_sc_6.c` (5 marks; also `9608_w21_qp_11_sc_4.c`). 9618 asks for the differences in prose; the tick/match format is 9608's.*

> [!question] 9608 | Explain the difference in power consumption between SRAM and DRAM [2]
> Explain the difference in power consumption between SRAM and DRAM, and why it matters.
>
>> [!success]- Answer — 4 points for 2 marks
>> - DRAM requires **higher power consumption under low levels of access**
>> - … because it needs extra circuitry to carry out the constant **refreshing**
>> - SRAM uses **less power** when idle, as it has no need to refresh
>> - This is significant in **battery-powered devices**, where idle time is common
>>
>> *Latest: `9608_s19_qp_12_sc_4.c`. Credited repeatedly in 9608 and **absent from every 9618 mark scheme** — a genuine content difference, not just a format one.*

> [!question] Inferred | Describe the cell structure of SRAM and DRAM [3]
> Describe how one memory cell of SRAM differs from one memory cell of DRAM.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A **DRAM** cell uses a **single transistor and a capacitor**
>> - … the capacitor leaks charge, which is why the cell must be **refreshed** thousands of times a second
>> - An **SRAM** cell uses **several transistors** forming a **flip-flop**
>> - … which holds its state as long as power is applied, so no refresh is needed
>> - The extra transistors make SRAM **larger, costlier and lower density**
>>
>> *Inference: 9608 credits the transistor counts directly, and 9618 accepts "simple design — uses fewer transistors" once in `s23_qp_11_sc_4.a.ii`, but never asks for the cell structure. It is the physical reason behind cost, density and refresh.*

> [!question] SME | Explain why SRAM is used for cache and DRAM for main memory [4]
> Explain why SRAM is used for cache memory and DRAM for main memory.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **SRAM** keeps data as long as power is on, using flip-flops, with no refreshing
>> - … so it is very fast and uses little idle power
>> - … but it is expensive and low density, so only a small amount is affordable
>> - … which suits **cache**, where speed matters more than size
>> - **DRAM** stores each bit in a tiny capacitor and needs constant refreshing
>> - … so it is cheaper and far denser, but slower — which suits **main memory**, where large cheap capacity is wanted
>>
>> *Framing the answer as "which property matters in this device" is what turns a list of differences into an applied answer; 9618 marks applied justifications at up to 4.*

---

## 3.1.7 Differences between PROM, EPROM and EEPROM

> [!question] 9618 | Match each description to the correct memory technology [3]
> Complete the table by writing PROM, EPROM or EEPROM against each description.
>
>> [!success]- Answer — 1 mark per row, 3 marks
>> - Contents erased using a **voltage pulse**, and changed many times without removing the chip → **EEPROM**
>> - Contents erased using **ultraviolet light**, and the chip must be physically removed to be reprogrammed → **EPROM**
>> - Contents can be written **only once** after manufacture → **PROM**
>>
>> *Latest: `9618_w25_qp_13_sc_4.c`*

> [!question] 9618 | Give two differences between EPROM and EEPROM [2]
> Give two differences between EPROM and EEPROM.
>
>> [!success]- Answer — 4 points for 2 marks
>> - EPROM is erased using **ultraviolet light**; EEPROM uses an **electrical signal**
>> - EPROM must be **removed from the circuit board** to be changed; EEPROM stays in the circuit
>> - EPROM erases **all** the data; EEPROM can erase **selected parts** (a byte at a time)
>> - EEPROM can therefore be reprogrammed by the **user**, without special equipment
>>
>> *Latest: `9618_w24_qp_12_sc_2.c`*

> [!question] 9618 | Explain the benefits of using EEPROM in a device [4]
> Explain the benefits of using EEPROM in a device.
>
>> [!success]- Answer — 7 points for 4 marks
>> - EEPROM allows **frequent read, write and erase** operations
>> - … so the device can be updated to take advantage of **new features**
>> - The firmware need **not be fully erased** first — a particular byte or the whole chip can be erased
>> - The chip does **not have to be removed** from the device
>> - … so the firmware can be changed by the **user, without technical expertise**
>> - **No additional equipment** (such as a UV eraser) is needed
>> - It is **cheaper to manufacture**, so the device is cheaper to buy
>>
>> *Latest: `9618_s24_qp_12_sc_2.c` (also `9618_w23_qp_13_sc_7.b`, `9618_w22_qp_11_sc_9.b`)*

> [!question] Inferred | Describe PROM and give a situation where it is appropriate [3]
> Describe what is meant by PROM and give one situation in which it would be the appropriate choice.
>
>> [!success]- Answer — 5 points for 3 marks
>> - PROM is supplied **blank** and is programmed **once** after manufacture
>> - … after which the contents **cannot be changed or erased**
>> - It is **non-volatile**, retaining its contents without power
>> - **Appropriate when** the program will never need to change — a remote control, a basic calculator
>> - … and when producing **high volumes cheaply**, since it is cheaper than EPROM or EEPROM
>>
>> *Inference: PROM appears only as one row of the `w25_qp_13_sc_4.c` matching table. Neither "describe PROM" nor an applied "where would you use it" has been asked.*

> [!question] Inferred | Explain why a programmable ROM is used rather than plain ROM [3]
> Explain why a manufacturer would use a programmable ROM rather than a ROM fixed at manufacture.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A mask ROM is **written during manufacture** and can never be altered
>> - … so any error in the firmware makes the whole chip **scrap**
>> - A programmable ROM can be written **after manufacture**
>> - … so the same blank chips can be used for **different products or versions**, and in small volumes
>> - EPROM and EEPROM additionally allow the firmware to be **corrected or updated** later
>>
>> *Inference: every 9618 question compares the three variants with each other. The prior question — why programmable ROMs exist at all — is untested.*

> [!question] SME | Compare PROM, EPROM and EEPROM row by row [4]
> Compare PROM, EPROM and EEPROM.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Reprogrammable?** PROM no (once only) · EPROM yes · EEPROM yes
>> - **Erased using** — PROM cannot be erased · EPROM **UV light** · EEPROM **electric voltage**
>> - **Removed from the device?** EPROM yes · EEPROM no, erased in place
>> - **Erased all at once?** EPROM yes, the whole chip · EEPROM no, selected parts
>> - **Typical use** — PROM permanent firmware (remote controls, basic calculators)
>> - **Typical use** — EPROM reprogrammable development work (older arcade machines, early consoles); EEPROM flash memory and BIOS (smart cards, key fobs, USB sticks, SSDs)
>>
>> *The "typical use" row is the part no mark scheme supplies, and it is exactly what an applied question would want.*

---

## 3.1.8 Monitoring and control systems

> [!question] 9618 | Describe the differences between a monitoring system and a control system [4]
> Describe the differences between a monitoring system and a control system.
>
>> [!success]- Answer — 6 points for 4 marks
>> - A monitoring system **takes no action**; a control system **acts autonomously** to change the environment when values fall outside a prescribed range
>> - A control system uses **actuators**; a monitoring system does not
>> - A control system makes use of **feedback**; a monitoring system does not
>> - The output of a monitoring system **does not affect the subsequent input**
>> - … whereas the output of a control system **changes the next input** from the sensor
>> - A monitoring system only **records, displays or warns**
>>
>> *Latest: `9618_w25_qp_11_sc_9`*

> [!question] 9618 | Identify whether a system is monitoring or control, and justify [3]
> For the system described, identify whether it is a monitoring system or a control system. Justify your answer.
>
>> [!success]- Answer — **no mark for the identification** — all 3 marks are in the justification
>> - **Control:** the system uses an **actuator** to perform an action
>> - … the output **changes the input** to the sensor
>> - … the system acts **autonomously** on the feedback from the sensor
>> - … input data causes the action, the action changes the measured quantity, and that new value determines the next action
>> - **Monitoring:** there is **no feedback** — the output is only an indicator or warning
>> - … the output does **not affect the input** from the sensors, and there are **no actuators**
>>
>> *Latest: `9618_w25_qp_12_sc_11` (also `w24_qp_12_sc_9.b`, `w24_qp_11_sc_5.c`, `s24_qp_11_sc_2.b`, `s21_qp_11_sc_5.c`). The most repeated question in the chapter, and the one candidates most often answer with the choice alone.*

> [!question] 9618 | Explain the importance of feedback in a control system [3]
> Explain the importance of feedback in a control system.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Feedback ensures the system operates **within set criteria / constraints**
>> - … by enabling the system **output to affect the subsequent input**
>> - … so conditions are adjusted **automatically**, without human intervention
>> - The system can check whether the action it took **had the intended effect**
>> - … and respond to further changes in the environment as they occur
>>
>> *Latest: `9618_s24_qp_13_sc_7.c` (also `9618_w22_qp_13_sc_10.a`, 3 marks)*

> [!question] 9618 | Identify an appropriate sensor for a scenario and state its use [2]
> Identify a suitable sensor for the system described and state how it is used.
>
>> [!success]- Answer — 1 mark for the sensor, 1 for its applied use
>> - **Pressure** — detects when an item is removed from or replaced on a shelf; detects an intruder sitting in a seat; detects a hit obstacle
>> - **Infra-red** — detects when a beam is broken; detects the heat of a person; measures the height of a vehicle
>> - **Light** — detects when the external daylight level falls below a set amount
>> - **Sound** — detects a sound inside a car; detects someone speaking
>> - **Proximity / infra-red** — counts items passing on a conveyor belt
>> - The use **must be tied to the scenario** — "measures pressure" alone scores nothing
>>
>> *Latest: `9618_s25_qp_11_sc_4.b` (also `w24_qp_12_sc_9.a`, `w24_qp_11_sc_5.a`, `s24_qp_13_sc_7.a`, `w22_qp_13_sc_10.b.i`)*

> [!question] 9618 | Describe the role of an actuator [2]
> Describe the role of an actuator in a control system.
>
>> [!success]- Answer — 4 points for 2 marks
>> - The actuator **generates a signal / causes an action** when instructed by the microprocessor
>> - … by **converting electrical energy into a mechanical force / movement**
>> - For example, to **push an arm**, open a trap door or pick up an item
>> - It is what makes a system a **control** system rather than a monitoring one
>>
>> *Latest: `9618_w23_qp_12_sc_1.b`*

> [!question] 9618 | Describe the purpose of a temperature sensor in a device [2]
> Describe the purpose of the temperature sensor in the device described.
>
>> [!success]- Answer — 4 points for 2 marks
>> - To prevent the device **overheating**
>> - … or to ensure the material is **hot enough** to work correctly
>> - By identifying the temperature of the **object being printed / processed**
>> - By identifying the temperature of the **material being used**
>>
>> *Latest: `9618_w23_qp_11_sc_7.b`*

> [!question] Inferred | Identify a suitable sensor for a temperature-based system and justify it [3]
> A greenhouse must be kept between 18 °C and 24 °C. Identify a suitable sensor, state what it measures and explain how the system uses its readings.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A **temperature sensor** is used
>> - It measures the **current air temperature** inside the greenhouse, continuously
>> - The reading is converted to digital by an **ADC** and compared with the **stored range** by the microprocessor
>> - If the temperature is too high, an **actuator opens the vents** (or too low, turns on the heater)
>> - The change alters the next reading — **feedback** — so the system adjusts automatically
>>
>> *Inference: the syllabus notes name **temperature, pressure, infra-red and sound**. 9618 has examined pressure, infra-red, sound and light; temperature appears only inside the 3D-printer and refrigerator scenarios, never as "identify a suitable sensor" — despite being listed first.*

> [!question] Inferred | Describe a system that both monitors and controls [3]
> Describe a system that both monitors an environment and controls it, explaining which parts do which.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Sensors take readings **continuously**, and the readings are **displayed or logged** — this is the monitoring part
>> - The microprocessor **compares** each reading with a stored range
>> - While readings stay in range, the system only **records** them and takes no action
>> - When a **threshold is crossed**, an actuator is operated — this is the control part
>> - The resulting change alters the next reading, so **feedback** closes the loop
>>
>> *Inference: every question asks which of the two a system is. `s24_qp_11_sc_2.b` (the video doorbell) accepts either answer if justified, which is the closest Cambridge has come to setting this.*

> [!question] SME | Define monitoring and control systems with examples [4]
> Define a monitoring system and a control system, giving an example of each.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Monitoring** — collects data continuously through observation, **passively**
>> - … it does not interact with or change the environment, and takes no action on the data
>> - … **example:** a weather station; hospital patient monitoring, which records, displays and alerts staff
>> - **Control** — automatically manages or adjusts a process based on sensor data
>> - … it monitors input, then **acts when conditions are met**, keeping the system stable without human input
>> - … **example:** central heating (thermostat → boiler on → target reached → heating off); automatic irrigation
>>
>> *The useful nuance: a patient monitor that **alerts staff** is still a monitoring system, because the alert does not change the patient's readings.*

> [!question] SME | Name sensors beyond those in the syllabus and state what each measures [4]
> Name four sensors other than temperature and state what each measures.
>
>> [!success]- Answer — 1 mark per sensor with its measurement, 4 marks
>> - **Accelerometer** — acceleration, tilt and vibration (airbags, phone orientation)
>> - **Gas** — presence of a specific gas, such as carbon monoxide
>> - **Humidity** — water vapour in the air (greenhouses)
>> - **Flow** — rate of movement of a gas, liquid or powder
>> - **Level, moisture, pH, magnetic field, proximity, acoustic** are also credited
>> - Lead with the four the syllabus names — **temperature, pressure, infra-red, sound** — and use these when a scenario demands something specific
>>
>> *Only four sensors are named in the 9618 syllabus, so the rest are insurance rather than core.*

---

# 3.2 Logic Gates and Logic Circuits

## 3.2.1–3.2.2 Symbols and functions of the six gates

> [!question] 9618 | Identify a gate not used in a circuit, draw its symbol and complete its truth table [3]
> Identify one logic gate that is **not** used in the circuit shown, draw its symbol, and complete its truth table.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - **1 mark** for naming a gate genuinely absent from the circuit
>> - **1 mark** for a symbol that matches the gate named
>> - **1 mark** for a truth table that matches the gate named
>> - The symbol and table are marked **against your own answer** — a wrong gate can still earn 2
>>
>> *Latest: `9618_w21_qp_11_sc_3.c`*

> [!question] 9618 | Describe the operation of four named gates [4]
> Describe the operation of the NAND, NOR, XOR and OR gates.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - **NAND** — the output is 0 when **both inputs are 1**, otherwise the output is 1
>> - **NOR** — the output is 1 when **both inputs are 0**, otherwise the output is 0
>> - **XOR** — the output is 1 when **one input is 1 and the other is 0**, otherwise 0
>> - **OR** — the output is 0 when **both inputs are 0**, otherwise the output is 1
>> - **AND** — the output is 1 only when **both inputs are 1**
>> - **NOT** — the output is the **opposite** of the input
>>
>> *Latest: `9618_s24_qp_12_sc_1.a` (also `9618_s23_qp_11_sc_5.b` for NAND and NOR). Any four of the six can be chosen — NOT and AND have never yet been the ones asked.*

> [!question] 9618 | Describe the operation of a 2-input XOR gate [1]
> Describe the operation of a two-input XOR gate.
>
>> [!success]- Answer — 3 phrasings for 1 mark
>> - The output is 1 only if **one input is 1 and the other is 0**
>> - The output is 1 only if the two inputs are **different**
>> - The output is 0 only if the two inputs are the **same**
>>
>> *Latest: `9618_w24_qp_13_sc_1.a`*

> [!question] 9618 | Tick which gate each statement describes [3]
> Tick to show which logic gate each statement describes.
>
>> [!success]- Answer — 1 mark per row, 3 marks
>> - The output is 1 only when both inputs are 1 → **AND**
>> - The output is 1 only when both inputs are different → **XOR**
>> - The output is 1 only when both inputs are 0 → **NOR**
>> - The output is 0 only when both inputs are 1 → **NAND**
>>
>> *Latest: `9618_s21_qp_11_sc_8`*

> [!question] 9618 | Identify the errors in a given truth table [2]
> The truth table shown for the given logic expression contains errors. Identify the rows that are incorrect.
>
>> [!success]- Answer — block marked, 2 marks
>> - Work the **expression** through for each row, using the working-space column
>> - Name the **row numbers** whose output value is wrong
>> - **1 mark** for one or two rows correctly identified; **2 marks** for all three
>> - Do not change the table — the answer is the list of row numbers
>>
>> *Latest: `9618_w25_qp_12_sc_9.b`*

> [!question] Inferred | Draw the symbols for all six logic gates [3]
> Draw the symbol for each of the NOT, AND, OR, NAND, NOR and XOR gates.
>
>> [!success]- Answer — 6 symbols, marked in pairs, 3 marks
>> - **NOT** — a triangle with a small circle on the output
>> - **AND** — a flat-backed D shape
>> - **OR** — a curved-back shape with a pointed output
>> - **NAND** — the AND shape with a **circle** on the output
>> - **NOR** — the OR shape with a **circle** on the output
>> - **XOR** — the OR shape with an **extra curved line** across the input side
>>
>> *Inference: the syllabus lists all six symbols, and every 9618 question expects them **inside** a drawn circuit. A question asking for them alone has never been set — but a wrong symbol silently costs marks in every circuit question, so they must be automatic.*

## 3.2.3–3.2.5 Constructing circuits, truth tables and expressions

> [!question] 9618 | Draw a logic circuit from a logic expression [2]
> Draw the logic circuit for the logic expression given.
>
>> [!success]- Answer — always 2 marks, split into two named halves
>> - **1 mark** for the first half of the circuit — e.g. `NOT B XOR C` correctly drawn
>> - **1 mark** for the second half — e.g. `NOT A`, the final AND, and the closing NOT
>> - **Alternative correct forms are accepted** — a NAND gate drawn in place of AND followed by NOT
>> - Marks are lost for **superfluous gates**, so draw only what the expression contains
>> - Work **outwards from the brackets**, and label each wire with the sub-expression it carries
>>
>> *Latest: `9618_w25_qp_13_sc_3.b` (also `9618_s24_qp_11_sc_1.b`)*

> [!question] 9618 | Complete a truth table from an expression or a circuit [2]
> Complete the truth table for the logic expression / circuit given.
>
>> [!success]- Answer — always 2 marks, marked in blocks
>> - **1 mark** for the **first four rows** correct
>> - **1 mark** for the **second four rows** correct (or per shaded block)
>> - A **single wrong row loses the whole half**, so the working-space column is worth using
>> - Build the working column **one gate at a time**, left to right through the expression
>> - … rather than trying to evaluate the whole expression per row
>>
>> *Latest: `9618_w25_qp_13_sc_3.a` (also `9618_s25_qp_11_sc_1.b`)*

> [!question] 9618 | Write the logic expression for a logic circuit [3]
> Write the logic expression for the logic circuit shown. Do not simplify the expression.
>
>> [!success]- Answer — marked per named sub-expression, up to 3 marks
>> - **1 mark** per correct sub-expression — e.g. `A NAND B`
>> - … e.g. `NOT (B XOR C)`
>> - … e.g. the final `NAND` combining them
>> - Where the circuit has **two outputs**, 1 mark for each output expression
>> - The instruction is usually "**do not simplify**" — a simplified answer can lose marks
>>
>> *Latest: `9618_w25_qp_12_sc_9.a` (also `9618_s25_qp_13_sc_4.a`)*

> [!question] 9618 | Write the logic expression for a truth table [2]
> Write the logic expression represented by the truth table shown.
>
>> [!success]- Answer — 2 marks
>> - Identify **each row where the output is 1**
>> - Write the **AND-term** for that row, using NOT for each input that is 0
>> - **OR** the terms together
>> - **1 mark** for one correct term; **1 mark** for the second term **plus the OR in the correct place**
>> - e.g. `Q = (R AND S AND NOT T) OR (NOT R AND NOT S AND T)`
>>
>> *Latest: `9618_w25_qp_11_sc_3.b`*

> [!question] 9618 | Match each truth table to its logic expression [3]
> Draw a line to match each truth table to the logic expression it represents.
>
>> [!success]- Answer — 1 mark per correct line, 3 marks
>> - Work **each expression** through all eight rows and compare the output column
>> - Match on the **whole column**, not on one or two rows
>> - Eliminate as you go — a wrong match usually costs two marks, not one
>>
>> *Latest: `9618_s24_qp_13_sc_6`*

> [!question] 9618 | Tick the correct logic statement for a truth table [1]
> Tick the logic statement that matches the truth table shown.
>
>> [!success]- Answer — 1 mark
>> - Evaluate each offered statement against the **output column**
>> - One row where the statement disagrees is enough to rule it out
>>
>> *Latest: `9618_s24_qp_11_sc_1.a`*

> [!question] 9618 | Write logic expressions from a problem statement [2]
> A table defines each parameter and the condition its binary value 1 represents. Write the logic expression for each output described.
>
>> [!success]- Answer — 1 mark per expression, 2 marks
>> - Read the **parameter table first** — note what binary 1 means for each letter
>> - The floodlight turns on if the security system is on **and** daylight is low **and** a person is detected → `X = E AND A AND C`
>> - The alarm sounds if the security system is on **and** one or more doors are open **or** a person is detected → `Y = E AND (B OR C OR D)`
>> - The **brackets carry the mark** in the second expression
>>
>> *Latest: `9618_w24_qp_11_sc_5.b`*

> [!question] Inferred | Draw a logic circuit directly from a problem statement [3]
> Using the parameter table given, draw the logic circuit for the system described in the prose.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Read the **parameter table first**, noting what 1 means for each letter — it is often the reverse of the intuitive reading (`A = 1` means daylight is **low**)
>> - Translate the prose directly: "and" → **AND**, "or" → **OR**, "unless" → **AND NOT**, "is closed" when 1 = open → **NOT**
>> - Draw the **inner conditions first**, then the gate that combines them
>> - Marks go to each named sub-circuit, and **superfluous gates lose marks**
>> - Worked example: a fan turns on if temperature **and** humidity are too high **and** the door is closed, **unless** maintenance mode is active → `F = (T AND H) AND (NOT D AND NOT M)`
>>
>> *Inference: the syllabus says all three — circuit, truth table and expression — can be constructed "from a problem statement". 9618 has only ever asked for the **expression** that way (`w24_qp_11_sc_5.b`). The circuit version is harder, because the parameter table must be read correctly first.*

> [!question] Inferred | Complete a 16-row truth table for a four-input circuit [2]
> Complete the truth table for the four-input logic circuit shown.
>
>> [!success]- Answer — 2 marks, marked in blocks
>> - Sixteen rows: count in binary from `0000` to `1111` down the input columns
>> - Use a **working column per gate**, filled top to bottom, rather than evaluating row by row
>> - Marks are expected in **blocks of eight rows**, mirroring the three-input pattern
>> - The circuit is drawn the same way — only the number of rows changes
>>
>> *Inference: every 9618 truth table so far has three inputs and eight rows, but four-input **circuits** are drawn regularly and nothing in the syllabus rules out the table.*

> [!question] Inferred | Identify a redundant gate or an equivalent circuit [2]
> Two logic circuits are shown. State whether they produce the same output for all inputs, and justify your answer.
>
>> [!success]- Answer — 4 points for 2 marks
>> - Build the **truth table for each circuit** and compare the output columns
>> - They are equivalent only if the outputs match for **every** row
>> - A single differing row is enough to justify "not equivalent" — **quote that row**
>> - A gate is redundant if removing it leaves the output column **unchanged** (e.g. a double NOT)
>>
>> *Inference: Boolean simplification is A Level (15.2), not AS — but the recurring instruction "do not simplify" implies awareness. A question asking whether two circuits are equivalent sits at the edge of the AS wording and has not been asked.*
