---
title: Jigsaw — 3 Hardware (AS Level)
syllabus: 9618 (2026)
topics: 3.1 Computers and their components · 3.2 Logic Gates and Logic Circuits
---

# Jigsaw — 3 Hardware

Syllabus content for **9618 Topic 3**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording. Fair game — just untested in the current series. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers. Weigh it against the mark schemes.

> [!danger] Two sub-topics are new in 9618
> The 9608 Legend has **no questions at all** under *embedded systems* or under *PROM / EPROM / EEPROM*. Both are 9618-only, like AI and bit manipulation. There is no old-syllabus safety net for them.

---

# 3.1 Computers and their components

## 3.1.1 The need for input, output, primary memory and secondary storage

> [!success] Explain how the amount of RAM affects performance
> More RAM means more currently running data and instructions can be stored · without needing to use **virtual memory** · without having to fetch the data from secondary storage first · which has a slower access time · less latency / delay waiting for instructions or data. `9618_s25_qp_11_sc_6.a.ii`

> [!success] Identify what a device stores in primary memory
> Current reading / data from the sensor · current or recent video · instructions being executed · start-up / BIOS / boot-up instructions. `9618_s24_qp_11_sc_2.c.i`

> [!success] Describe two ways hardware can be upgraded to improve performance, and explain each
> Increase the number of cores … each core can **independently** carry out a process at the same time, so more instructions are performed **in parallel** · increase RAM capacity … allowing more applications to reside in memory at once, saving disk access time · increase cache memory … more data stored in fast access, so less time spent accessing RAM · increase clock speed … more Fetch-Decode-Execute cycles per unit time. `9618_s23_qp_12_sc_5.b`

> [!success] Justify magnetic storage over solid state for a given scenario
> Lower cost per unit of storage … so the high capacity required for a large number of video files is less costly · a large number of read/write operations are performed continuously … and magnetic storage is likely to have a longer life span than solid state. `9618_w25_qp_13_sc_7.d` (repeated in `9618_s23_qp_11_sc_4.b`)

> [!warning] Match a description of use to the appropriate input or output device
> Credit card number into an online form → keyboard/keypad · option at an airport kiosk → touch screen · a single high-quality photograph → inkjet printer · several hundred high-quality leaflets → **laser printer** · a hard copy image into a computer → scanner. The device-selection table is a 9608 staple and has no 9618 equivalent. `9608_s15_qp_12_sc_6.a`

> [!info] Justify solid state **over** magnetic
> Both 9618 questions run the argument one way — why magnetic beats solid state for a server. The reverse (a laptop or embedded device: no moving parts so shock-resistant, silent, faster access, lower power, smaller) has never been asked in 9618 even though every mark scheme point exists.

> [!info] Why a computer needs secondary storage at all
> Every question is a comparison between storage **types**. The bullet's actual wording — the *need* for secondary storage (non-volatile, retains data with the power off, much larger capacity, holds files not currently in use) — is untested.

> [!abstract] Choosing a storage device — the decision factors
> Storage needs (how much data) · performance needs (does the user need fast access — SSD for video editing or gaming) · portability (USB flash drive or external drive to move data between machines) · cost (higher capacity and faster devices cost more). The same four-factor structure applies to choosing input/output devices: user needs, user skills, environment, cost. A useful skeleton for any "recommend a device and justify" question.

> [!abstract] Typical capacities and trade-offs
> HDD 500 GB–2 TB, low cost per GB, low portability, moderate durability (moving parts) · SSD 120 GB–4 TB, high cost per GB, high durability (no moving parts) · USB flash 8–256 GB, very high portability · CD 700 MB, DVD 4.7–9 GB, Blu-ray 25–50 GB, low cost per disc but easily scratched. Figures are not credited, but they make "high capacity" and "cost per unit" concrete.

---

## 3.1.2 Embedded systems

> [!danger] No 9608 questions exist for this bullet
> Embedded systems is **new in 9618** and has been examined in almost every series since 2021. Everything below is 9618 or inference.

> [!success] Describe what is meant by an embedded system, using an example
> Definition: a microprocessor / microcontroller within a **larger system** // a microprocessor that performs **one specific task** · Example: the embedded system in a washing machine only controls the programs for the washing cycle // it is part of the washing machine but does not perform any other function within it. `9618_s21_qp_11_sc_5.a`

> [!success] Identify features / characteristics of an embedded system
> Dedicated to a single task // limited number of functions · **built into** / integrated into a larger system · must contain a processor, memory and an I/O capability // dedicated hardware · combination of hardware and software designed for a **specific function** · the system is **not easily changed** or updated by the owner · does not require much processing power · the system does not have its own operating system. `9618_w23_qp_12_sc_1.c.i`; `9618_w22_qp_13_sc_10.b.ii`

> [!success] Identify characteristics of a described device that suggest it is an embedded system
> The device only performs the specific tasks described · the sensors and camera are **built into** it · the CPU / memory / storage / software are all dedicated to this task only · only a dedicated microprocessor is required due to the limited processing requirements. `9618_s24_qp_11_sc_2.a`

> [!success] Give an example of an embedded system and explain why it is one
> Each reason must be **applied to the example given**: dedicated to one task · does not require much processing power · built into a larger system · contains firmware that cannot be easily updated. `9618_w23_qp_11_sc_9.b`

> [!success] Describe the drawbacks of embedded systems
> Difficult to change / update the **firmware** by the user // difficult to upgrade to take advantage of new technology · errors cannot be fixed easily // troubleshooting, fault-finding or repairing is a specialist task / expensive · functionality cannot be changed or extended easily // cannot be easily adapted for another task · faulty or outdated devices are often thrown away rather than repaired … leading to **e-waste**. `9618_w24_qp_12_sc_2.a`

> [!success] Explain the reasons why ROM is used in an embedded system
> To **store** data that does not change · data must be stored even when the device is without power · to store boot-up instructions / system software / firmware / BIOS. `9618_w22_qp_12_sc_3.c`

> [!info] The **benefits** of embedded systems
> 9618 has asked for the drawbacks (3 marks) and the characteristics repeatedly, but never for the benefits. Available: small and compact, low power consumption, cheap to produce because minimal hardware is needed, fast and reliable for repetitive tasks, real-time operation. Given the drawbacks question exists, the inverse is overdue.

> [!abstract] Benefits and drawbacks, side by side
> **Benefits:** small and compact, easy to fit into a dedicated device · low power consumption, so efficient and cost-effective · fast and reliable, designed for quick repetitive tasks · cheaper to produce, uses minimal hardware · works in **real time**, ideal for time-sensitive operations such as alarms.
> **Drawbacks:** limited functionality · hard to upgrade or repair, being built into the device · limited memory and processing power · not flexible, cannot easily be reprogrammed · may be **less secure**, with limited protection if connected to other systems.
> The security point is not in any mark scheme but is a defensible modern drawback.

> [!abstract] A stock of examples
> Heating thermostats · hospital equipment · washing machines · dishwashers · coffee machines · satnav · factory equipment · security systems · traffic lights. The examined scenarios so far are a video doorbell, a car alarm, a television, a washing machine and factory machinery — have one ready that is *not* the one in the question.

---

## 3.1.3 Principal operations of hardware devices

> [!success] Complete the description of a magnetic hard disk
> The disk has one or more **platters** that can be magnetised. These are mounted on a **spindle** and rotate at high speed. A **read/write head** is moved across the surface on an arm. When data is read, the changes in the **magnetic field** produce a change in the electric current. `9618_s25_qp_11_sc_6.a.i`

> [!success] Describe the principal operation of an optical disc reader/writer
> The disc is spun at high speed · a **laser** is shone onto the disc to read or write · using an optical head to move it into position · it follows the **spiral track** from the centre outwards · when writing, the laser burns **pits** to represent the data · when reading, the laser reflects from pits and **lands** · the reflection from a pit and a land is different · the differences are interpreted as 1 or 0. `9618_w24_qp_11_sc_3.d.i`

> [!success] Describe the principal operation of a touchscreen
> **Resistive:** the space between the conductive layers is removed / the layers touch and a circuit is completed · **Capacitive:** the electrical charge changes where the user pressed · the point of contact is identified … from the change in electrical field · the software / microprocessor **calculates** the coordinates. `9618_s24_qp_13_sc_7.d`

> [!success] Explain how a touchscreen converts the point of touch to a menu selection
> *(Max 2 for the detection method, max 2 for the selection.)* Resistive // two layers make contact and complete a circuit · capacitive // contact creates a change in charge · infrared // the beams are broken · optical imaging // a shadow is created · acoustic pulse // the wave is absorbed · then: the point of touch determines the **x and y coordinates** · the menu item corresponding to that coordinate position is recognised and added to the order. `9618_w25_qp_12_sc_8.b.i`

> [!success] Complete the description of touchscreen types (cloze)
> A **resistive** touchscreen has two layers; when touched, the layers touch and a **circuit** is completed. A **capacitive** touchscreen has several layers; when the top layer is touched there is a **change** in the electric current. A microprocessor identifies the **coordinates** of the touch. `9618_s23_qp_13_sc_3.a`

> [!success] Explain how a model is printed using a 3D printer
> **Generic (max 3):** additive manufacturing · uses a digital file created from 3D modelling or **CAD** software · the printer builds the model **one layer at a time**, starting from the bottom, using x, y and z co-ordinates · the process is repeated for each layer · the material is fused or cured together layer by layer · some materials need time to cool and set, or UV curing using LEDs.
> **Specific (max 1):** FDM — material is heated and pushed through a nozzle / extruder · SLA — photosensitive liquid resin is exposed to a UV laser beam · DLP — resin is exposed to a UV projected image of the layer · SLS — a laser forms objects from powdered material. `9618_w25_qp_11_sc_10.a`; `9618_w23_qp_11_sc_7.a`

> [!success] Describe the principal operation of a microphone
> The microphone has a **diaphragm / ribbon** · the incoming sound waves cause vibrations of the diaphragm · causing a coil to move past a magnet // a magnet to move past a coil (dynamic) // changing the capacitance (condenser) // deforming the crystal (crystal) · an **electrical signal** is produced. `9618_w21_qp_12_sc_3.a`

> [!success] Complete the description of a VR headset
> A headset can have one or two **(LCD) displays / screens / lenses** that output the image. The head movements are detected using a sensor — a **gyroscope / accelerometer**. The data is analysed by a microprocessor to identify the **direction / speed** of movement. Some headsets use **digital cameras** that record the user's eye movements. `9618_s24_qp_12_sc_2.a`

> [!success] Complete the table on solid state (flash) memory
> The two types of logic gate used to create solid state devices → **NAND** and **NOR** · the number of transistors in each cell → **2** · the type of gate that can retain electrons without power → **floating** · the type of gate that allows or stops current passing through → **control**. `9618_s24_qp_11_sc_2.c.ii`

> [!info] The laser printer's own operation
> The laser printer appears repeatedly in 9618, but only ever as the setting for a **buffer** question (`w23_qp_13_sc_7.c`). The principal operation of the laser printer itself — charged drum, laser writes the image, toner attracted to charged areas, transferred to paper, fused by hot rollers — is **named in the syllabus notes and has never been asked in 9618**.

> [!info] Speakers
> Named in the syllabus notes alongside the microphone, and the microphone has been examined. The speaker (electrical signal → electromagnet/coil → cone vibrates → sound waves) is the mirror image and is untested in 9618.

> [!abstract] The laser printer, step by step
> **Laser draws the image** — a laser beam draws the page onto a **photosensitive drum**; wherever the laser hits, it changes the electric charge on the drum. **Toner sticks to the drum** — toner powder is attracted to the charged areas, matching the shape of the text or image. **Toner is transferred to paper** — the drum rolls the toner onto the paper. **Fusing** — the paper passes through hot rollers, melting the toner onto the paper so it does not smudge. This is the content for the `!info` gap above.

> [!abstract] Solid state memory — how a cell actually works
> Memory is made of tiny cells, each holding one bit. Each cell contains a transistor acting as a switch, with two parts: the **control gate** (top layer, connects to the circuit and controls whether current flows) and the **floating gate** (holds a charge, sandwiched between two insulating oxide layers). To store data, a high voltage on the control gate pushes electrons through the oxide onto the floating gate; to erase, a high voltage in the opposite direction pulls them off. Uses **NAND and NOR** gates. The table in `s24_qp_11_sc_2.c.ii` credits the four one-word answers — this is the mechanism behind them.

> [!abstract] Magnetic hard disk — the extra detail
> Platters are divided by concentric circles into **tracks**, and by wedge shapes into **sectors**; where they intersect is a **track sector**. The disk spins at typically 5400–7200 RPM. A read/write arm controlled by an **actuator** moves the head. Data is read and written using **electromagnets**. Tracks and sectors are not in the 9618 cloze but are standard credited detail.

> [!abstract] Microphone and touchscreen types
> **Dynamic** microphones suit loud environments; **condenser** microphones are more sensitive and used in studios. **Capacitive** touchscreens react to the electrical charge in a finger (phones, tablets); **resistive** respond to pressure (ATMs, tills). Knowing which type suits which scenario turns a generic description into an applied answer.

---

## 3.1.4 The use of buffers

> [!success] Explain how a memory buffer is used when transferring data to a hard disk
> The computer and the hard disk drive transmit and receive at **different speeds** // the computer transfers data faster than the HDD can receive · the buffer is used for **temporary storage** · so that the computer can transfer data to the buffer at the higher speed · and is not held up waiting for data to transfer · and so that data is transferred to the hard disk drive from the buffer at the slower rate. `9618_w24_qp_13_sc_2.b`

> [!success] Explain the use of a buffer when writing to an optical disc
> The computer and the optical disc reader/writer send and receive at different speeds · a buffer allows temporary storage of the data · so the computer can transfer data at the higher speed · and is not held up waiting // so the computer can carry on with other tasks · so the optical disc reader/writer is not overloaded · and data is transferred from the buffer at the slower rate. `9618_w24_qp_11_sc_3.d.ii`

> [!success] Describe how a laser printer makes use of a buffer
> The print instructions and data are sent by the laptop to a buffer (at laptop speed) · the data is transferred from the buffer to the printer (at printer speed) · allowing the user to continue using the laptop // allowing the processor to continue processing · instead of waiting for the relatively slower printer · when the buffer is empty an **interrupt** is sent to the laptop · requesting more data. `9618_w23_qp_13_sc_7.c`

> [!success] Explain how a buffer is used transmitting data to a peripheral
> The buffer is a **temporary** store for data going to the device · data is **transferred** into the buffer by the computer · data is **retrieved** from the buffer by the device · when the buffer is empty or full an **interrupt** is sent to the computer requesting more data or stopping further data being sent. `9618_s24_qp_12_sc_2.b`

> [!success] Explain the purpose of a buffer, with an example
> *(Max 2 purpose + max 1 example.)* Purpose: to act as temporary storage // to store downloaded data · before it is used by the receiving device · to allow processes or devices to operate at different speeds // independently of each other. Examples: printer buffer, video buffer when streaming, keyboard buffer during data entry. `9618_w22_qp_13_sc_1.c`

> [!success] State why a 3D printer needs a buffer [1]
> To free up the processor to carry out other tasks, as the rate data is received by the printer differs from the rate at which it can be processed · to manage the mismatch in speed between the processor and the peripheral. `9618_w25_qp_11_sc_10.b`

> [!success] Describe the roles of the address bus, the data bus and buffers when writing to a device
> Buffers — temporarily hold data until it is ready to be transmitted **to the device** · Address bus — the address of the **data to be written to the device** (in RAM) is carried on the address bus · Data bus — all data to be **written to the device / buffer** is carried on the data bus. `9618_w23_qp_12_sc_8.c.ii`

> [!warning] Sequence the steps of a hard-disk file read, including the disk buffer
> The application executes a read statement → passes the request to the OS → the OS spins the disk → looks up the track and sector in the directory file → the head moves to the correct track → waits for the correct sector → reads the first cluster into the **disk buffer** → continues reading successive clusters → generates an **interrupt** when done → the OS transfers the buffer contents to the program's data memory. An 8-mark sequencing question with no 9618 equivalent. `9608_w16_qp_12_sc_3`

> [!warning] How buffering allows a streamed video to play without pausing
> The user needs high-speed broadband · data is streamed to a buffer in the computer · buffering stops the video pausing as bits are streamed · as the buffer empties it fills again so viewing is continuous · actual playback is a few seconds behind the time the data is received. Filed under buffers in 9608 and under bit streaming in Chapter 2 — see the Communications Jigsaw. `9608_w16_qp_13_sc_6`

> [!info] The interrupt half of the buffer story
> "When the buffer is empty an interrupt is sent" appears as a mark point in three separate 9618 questions but has never been the subject of one. The link between buffers and interrupts is the natural bridge to Chapter 4 and is untested as a question in its own right.

---

## 3.1.5 Differences between RAM and ROM

> [!success] Describe the contents of ROM in a computer
> Stores the **bootstrap program** // start-up instructions **for that computer** // BIOS · stores the start-up instructions for the attached system // firmware · stores the **kernel** of the operating system // parts of the operating system. `9618_s23_qp_11_sc_4.a.i`

> [!success] State the purpose of RAM and ROM in an embedded system
> **RAM:** stores the choices / program the user has entered // stores the data read from the sensors // stores the time left in the program // by example. **ROM:** stores the start-up instructions. `9618_s21_qp_11_sc_5.b`

> [!success] Explain why ROM is used in an embedded system
> To store data that does not change · data must be stored even when the device is without power · to store boot-up instructions / system software / firmware / BIOS. `9618_w22_qp_12_sc_3.c`

> [!warning] Describe two or three **differences** between RAM and ROM
> RAM loses its content when the power is turned off / volatile / temporary, whereas ROM does not / non-volatile / permanent · data in RAM can be altered, deleted, read from and written to, whereas ROM is read only and cannot be changed · RAM stores files, data and the operating system currently in use, whereas ROM stores the BIOS / bootstrap / pre-set instructions · RAM's memory size is often larger than ROM's. **9618 has only ever asked what each one stores, never the differences between them, despite the bullet being titled "explain the differences".** `9608_w16_qp_12_sc_6.a` (2 marks); `9608_s15_qp_13_sc_4.b` (3 marks)

> [!warning] Describe the purpose of RAM and ROM in a named peripheral
> *For a laser printer:* RAM stores the currently running parts of the printer software, the data being printed / the contents of the buffer, the current progress of printing, and data about the printer such as toner levels. ROM stores the printer's operating software, the boot-up instructions, and the printer **fonts**. `9608_s20_qp_13_sc_2.b`

> [!info] Volatility as the headline distinction
> The single most important RAM/ROM fact — **volatile vs non-volatile** — appears in 9618 only as an implied part of "data must be stored even when the device is without power". A direct "state two differences" question would catch anyone who has only learned the 9618 storage-contents answers.

> [!abstract] RAM and ROM compared, feature by feature
> **Speed** — RAM very fast; ROM fast but slower than RAM. **Capacity** — RAM gigabytes; ROM megabytes. **Stores** — RAM programs and data in use; ROM the bootstrap / start-up instructions. **Read/write** — RAM read and write; ROM read only. **Volatility** — RAM volatile; ROM non-volatile.
> Both are **primary memory**, directly accessible by the CPU; ROM is a small chip on the motherboard containing the **BIOS**.

---

## 3.1.6 Differences between SRAM and DRAM

> [!success] State three differences between DRAM and SRAM
> DRAM requires refreshing / recharging, SRAM does not · DRAM stores each bit as a **charge**, SRAM uses a **flip-flop** · DRAM is less expensive to manufacture, SRAM is more expensive · DRAM has slower access speeds, SRAM has faster access times · DRAM has higher storage / bit / data **density**, SRAM lower · DRAM is used in **main memory**, SRAM in **cache**. `9618_w25_qp_11_sc_6.c`

> [!success] Identify advantages of DRAM instead of SRAM
> Costs less per unit · higher storage density // more data can be stored per chip · simple design — uses fewer transistors · a fast access speed is not needed for this device. `9618_s23_qp_11_sc_4.a.ii`; `9618_w23_qp_11_sc_7.c`; `9618_w24_qp_12_sc_2.b`

> [!success] Identify disadvantages of DRAM instead of SRAM
> DRAM requires constant refresh cycles unlike SRAM · DRAM has lower access speed than SRAM. `9618_w24_qp_11_sc_3.c`

> [!success] Explain why SRAM is used instead of DRAM
> Static RAM has a **faster access time** · because it does not need to be refreshed · used on the CPU for improvement of CPU **cache** speed. `9618_w23_qp_13_sc_7.a`

> [!warning] Tick or match statements to SRAM or DRAM
> More expensive to make → SRAM · requires refreshing → DRAM · made from flip-flops → SRAM · has less complex circuitry → DRAM · mainly used in cache memory where speed is important → SRAM · requires higher power consumption under low levels of access, significant in battery-powered devices → DRAM. 9618 asks for differences in prose; the matching / tick format is 9608's. `9608_w18_qp_13_sc_6.c` (5 marks); `9608_w21_qp_11_sc_4.c`

> [!warning] The power-consumption difference
> DRAM requires **higher power consumption under low levels of access**, which is significant in battery-powered devices, because it requires more circuitry for refreshing // SRAM uses less power as it has no need to refresh. Credited repeatedly in 9608 and **absent from every 9618 mark scheme**. `9608_s19_qp_12_sc_4.c`

> [!info] Transistor counts
> 9608 credits "DRAM uses a single transistor and capacitor; SRAM uses more than one transistor to form a memory cell". 9618 accepts "simple design — uses fewer transistors" once, in `s23_qp_11_sc_4.a.ii`, but never asks for the cell structure. It is the physical reason behind cost, density and refresh, so it is worth being able to state.

> [!abstract] Why each is used where it is
> **SRAM** keeps data as long as power is on, made from **flip-flops**, no refreshing needed; very fast, uses less power, but expensive and lower capacity — so it is used where **speed matters more than size**, i.e. cache memory. **DRAM** stores each bit in a tiny **capacitor** and needs constant refreshing; cheaper, higher capacity in less space, but slower and more power-hungry during refresh — so it is used as **main memory**, where large cheap capacity is wanted. Framing the answer as "which property matters in this device" is what turns a list of differences into an applied answer.

---

## 3.1.7 Differences between PROM, EPROM and EEPROM

> [!danger] No 9608 questions exist for this bullet either
> Like embedded systems, PROM/EPROM/EEPROM is **new in 9618**.

> [!success] Match descriptions to memory technology
> Contents erased using a **voltage pulse**, changed multiple times without physically removing the memory → **EEPROM** · contents erased using **ultraviolet light**, must be physically removed to be reprogrammed → **EPROM** · contents can be written **only once** after manufacture → **PROM**. `9618_w25_qp_13_sc_4.c`

> [!success] Give two differences between EPROM and EEPROM
> EPROM uses **ultraviolet light** to erase data whilst EEPROM uses an **electrical signal** · EPROM has to be **removed from the circuit board** when changing the data whilst EEPROM remains in the circuit · EPROM erases **all** the data, EEPROM can erase **parts** of the data. `9618_w24_qp_12_sc_2.c`

> [!success] Explain the benefits of using EEPROM in a device
> EEPROM allows **frequent / multiple** read/write/erase operations · so the device can take advantage of new features · without fully erasing the contents of the firmware first // can erase a particular byte or the whole EEPROM · without removing the chip / firmware from the device · so the firmware can be changed by the user **without technical expertise** · no additional equipment is needed to change it · cheaper to manufacture, so the device is cheaper to purchase. `9618_s24_qp_12_sc_2.c`; `9618_w23_qp_13_sc_7.b`; `9618_w22_qp_11_sc_9.b`

> [!info] PROM in its own right
> PROM appears only as one row of the `w25_qp_13_sc_4.c` matching table. "Describe what is meant by PROM" or "give one situation where PROM is appropriate" (a fixed program that will never need changing, cheap for high volume) has never been asked.

> [!info] Why use a ROM variant rather than plain ROM
> Every question compares the three variants with each other. The prior question — why a manufacturer would choose a *programmable* ROM over a mask ROM fixed at manufacture — is untested and is the reason the three exist.

> [!abstract] The three compared, row by row
> **Reprogrammable?** PROM no, programmed once only · EPROM yes · EEPROM yes.
> **Erased using** — PROM cannot be erased · EPROM UV light · EEPROM electric voltage.
> **Must be removed from the device?** PROM n/a · EPROM yes · EEPROM no, erased in place.
> **Erased all at once?** EPROM yes, the entire chip · EEPROM no, specific parts can be erased.
> **Common use** — PROM permanent firmware (remote controls, basic calculators) · EPROM reprogrammable development (older arcade machines, early consoles) · EEPROM flash memory and BIOS chips (computer BIOS, smart cards, key fobs, USB sticks and SSDs).
> The "common use" column is the part no mark scheme supplies, and it is exactly what an applied question would want.

---

## 3.1.8 Monitoring and control systems

> [!success] Describe the differences between a monitoring system and a control system
> Monitoring systems do not take any action, whereas control systems **act autonomously** to change the environment if values are out of a prescribed range · control systems use **actuators**, monitoring systems do not · control systems make use of **feedback**, monitoring systems do not · the output from a monitoring system does not affect the subsequent input, whereas output from a control system affects the next input. `9618_w25_qp_11_sc_9`

> [!success] Identify whether a described system is monitoring or control, and justify
> **No marks for the identification — all marks are in the justification.**
> *Control:* the system uses an **actuator** to perform the action · the output changes the input to the sensor · the system acts **autonomously** on the feedback from a sensor · input data causes the action, the action changes the measured quantity, and this new value determines the next action.
> *Monitoring:* there is **no use of feedback** // the output is only an indicator or warning · the output does not affect the input of data from the sensors · the system does **not have any actuators**.
> `9618_w25_qp_12_sc_11`; `9618_w24_qp_12_sc_9.b`; `9618_w24_qp_11_sc_5.c`; `9618_s24_qp_11_sc_2.b`; `9618_s21_qp_11_sc_5.c`

> [!success] Explain the importance of feedback in a control system
> Feedback ensures that a system operates within set criteria / constraints · by enabling system output to affect subsequent system input · thus allowing conditions to be **automatically** adjusted. `9618_s24_qp_13_sc_7.c`; `9618_w22_qp_13_sc_10.a` (3 marks)

> [!success] Identify an appropriate sensor for a scenario and state its use
> Pressure — detects when the pressure of an item is removed from or replaced on a shelf; detects when an intruder sits in a seat; detects a hit obstacle · Infra-red — detects when a beam is broken; detects the heat of a person; measures the height of a vehicle; detects an obstacle · Light — detects when the external daylight level falls below a set amount · Sound — detects a sound inside a car; detects someone speaking · Proximity / infra-red — counts items passing on a conveyor belt. `9618_s25_qp_11_sc_4.b`; `9618_w24_qp_12_sc_9.a`; `9618_w24_qp_11_sc_5.a`; `9618_s24_qp_13_sc_7.a`; `9618_w22_qp_13_sc_10.b.i`

> [!success] Describe the role of an actuator
> The actuator generates a signal / causes an action / **converts electrical energy into a mechanical force** · to push an arm // to open a trap door // to pick up the item. `9618_w23_qp_12_sc_1.b`

> [!success] Describe the purpose of a temperature sensor in a device
> To prevent **overheating** // ensure the material is hot enough · by identifying the temperature of the object being printed · by identifying the temperature of the material being used. `9618_w23_qp_11_sc_7.b`

> [!info] The four sensors named in the syllabus
> The notes name **temperature, pressure, infra-red and sound**. 9618 has examined pressure, infra-red, sound and light; **temperature** appears only in the 3D-printer question and the refrigerator scenario, never as "identify a suitable sensor" — despite being the first one listed.

> [!info] Monitoring **and** control in the same system
> Every question asks which of the two a system is. A system that does both — monitors continuously and acts only when a threshold is crossed — has not been examined, though `s24_qp_11_sc_2.b` (the video doorbell) allows either answer if justified, which is the closest Cambridge has come.

> [!abstract] The two system types, defined
> **Monitoring** — collects data continuously through observation, passively; does not interact with or change the environment; takes no action based on the data; designed for high accuracy. Examples: weather stations, hospital patient monitoring (it records and displays, and alerts staff, but does not treat the patient).
> **Control** — automatically manages or adjusts a process based on sensor data; monitors input then takes action when conditions are met; *does* interact with the environment; keeps systems stable, safe or efficient without human input. Examples: central heating (thermostat → boiler on → target reached → heating off) and automatic irrigation (soil moisture → sprinklers → correct level → water off).
> Note the useful nuance: a patient monitor that **alerts staff** is still a monitoring system, because the alert does not change the patient's readings.

> [!abstract] A wider sensor table than the syllabus names
> Acoustic (sound levels) · accelerometer (acceleration, tilt, vibration — airbags, phone orientation) · flow (rate of gas, liquid or powder) · gas (presence of e.g. carbon monoxide) · humidity (water vapour — greenhouses) · infra-red (motion or heat source) · level (liquid levels — fuel tanks) · light · magnetic field (ABS braking, rotating machinery) · moisture (soil, damp in buildings) · pH (soil, chemical processes) · pressure · proximity (distance — robotics, collision avoidance) · temperature.
> Only temperature, pressure, infra-red and sound are named in the 9618 syllabus, so lead with those; the rest are useful when a scenario demands something specific.

> [!abstract] The feedback loop, described
> A feedback loop is when a control system uses its **output to influence its next input**. It lets the system automatically adjust and stay within set conditions, check whether it is working as expected, respond to changes in its environment, and stay within set limits or target values. This is the same content the mark scheme credits, phrased as a loop rather than a list.

---

# 3.2 Logic Gates and Logic Circuits

> [!note] This is a skills sub-topic
> Almost every question is draw / complete / write, and the tariffs are remarkably stable: **draw a circuit from an expression is always 2 marks**, **complete a truth table is always 2 marks**, and writing an expression from a circuit is 2–3. The gaps below are therefore about *formats*, not content.

## 3.2.1 Use the logic gate symbols

> [!success] Draw the symbol for a named gate
> Asked as part of "identify one logic gate **not** used in the given circuit, draw its symbol **and** complete its truth table" — 1 mark for the gate, 1 for the matching symbol, 1 for the matching truth table. `9618_w21_qp_11_sc_3.c`

> [!info] The symbols asked for on their own
> The syllabus lists all six symbols, and every 9618 question expects them **inside** a drawn circuit. A question that simply asks for the six symbols has never been set — but a wrong symbol silently costs marks in every circuit question, so they must be automatic.

## 3.2.2 Functions of NOT, AND, OR, NAND, NOR and XOR

> [!success] Describe the operation of each of four named gates
> **NAND** — the output is 0 when both inputs are 1, otherwise the output is 1 · **NOR** — the output is 1 when both inputs are 0, otherwise the output is 0 · **XOR** — the output is 1 when one input is 1 and the other is 0, otherwise the output is 0 · **OR** — the output is 0 when both inputs are 0, otherwise the output is 1. `9618_s24_qp_12_sc_1.a` (4 marks, 1 each)

> [!success] Describe the operation of a 2-input XOR gate [1]
> Output is only 1 if one input is 1 and the other is 0 // output is only 1 if both inputs are **different** // output is only 0 if both inputs are the **same**. `9618_w24_qp_13_sc_1.a`

> [!success] Tick which gate each statement describes
> The output is 1 only when both inputs are 1 → **AND** · the output is 1 only when both inputs are different → **XOR** · the output is 1 only when both inputs are 0 → **NOR**. `9618_s21_qp_11_sc_8`

> [!success] Identify errors in a given truth table
> Work the expression through for each row and name the row numbers whose output is wrong. 1 mark for one or two correct, 2 marks for all three. `9618_w25_qp_12_sc_9.b`

> [!info] NOT and AND described in words
> `s24_qp_12_sc_1.a` asks for NAND, NOR, XOR and OR; `s23_qp_11_sc_5.b` for NAND and NOR. **NOT and AND have never been the ones asked for**, presumably as too easy — but the four-gate format means any four of the six could be chosen.

## 3.2.3–3.2.5 Construct a logic circuit, a truth table and a logic expression

> [!success] Draw a logic circuit from a logic expression [2]
> Always 2 marks, split as two named halves of the circuit — e.g. "1 mark for NOT B XOR C, 1 mark for NOT A and the final AND plus NOT". Alternative correct forms are accepted (e.g. NAND drawn instead of AND followed by NOT). Marks are lost for **superfluous gates**, so draw only what the expression contains. `9618_w25_qp_13_sc_3.b`; `9618_s24_qp_11_sc_1.b`

> [!success] Complete a truth table from an expression or a circuit [2]
> Always 2 marks: **1 mark for the first four rows, 1 mark for the second four rows** (or per shaded block). A single wrong row loses the whole half, so the working-space column is worth using. `9618_w25_qp_13_sc_3.a`; `9618_s25_qp_11_sc_1.b`

> [!success] Write the logic expression for a logic circuit [3]
> Marked per named sub-expression — e.g. "A NAND B" · "NOT (B XOR C)" · "final NAND". Where the circuit has two outputs, 1 mark each. The instruction is usually "do **not** simplify the expression". `9618_w25_qp_12_sc_9.a`; `9618_s25_qp_13_sc_4.a`

> [!success] Write the logic expression for a truth table [2]
> Identify each row where the output is 1, write the AND-term for that row, and OR the terms together: 1 mark for one correct term, 1 mark for the second term **plus the OR in the correct place**. e.g. `Q = (R AND S AND NOT T) OR (NOT R AND NOT S AND T)`. `9618_w25_qp_11_sc_3.b`

> [!success] Match truth tables to logic expressions [3]
> Work each expression through the eight rows and match. 1 mark per correct line. `9618_s24_qp_13_sc_6`

> [!success] Tick the correct logic statement for a truth table [1]
> `9618_s24_qp_11_sc_1.a`

> [!success] Write logic expressions from a **problem statement** [2]
> A table defines each parameter and the condition its binary value represents, then prose states when each output is 1. e.g. floodlight turns on if the security system is on **and** daylight is low **and** a person is detected → `X = E AND A AND C`; alarm turns on if the security system is on **and** one or more doors are open **or** a person is detected → `Y = E AND (B OR C OR D)`. 1 mark per correct expression. `9618_w24_qp_11_sc_5.b`

> [!info] A **circuit** or **truth table** built directly from a problem statement
> The syllabus says all three can be constructed "from a problem statement". 9618 has only ever asked for the **expression** that way (`w24_qp_11_sc_5.b`). Being asked to draw the circuit, or fill the truth table, straight from the prose is the untested third of that bullet — and it is harder, because the parameter table must be read correctly first.

> [!info] Truth tables with four inputs
> Every 9618 truth table has three inputs and eight rows. Circuits with four inputs (A, B, C, D) are drawn regularly, so a 16-row table is possible; nothing in the syllabus rules it out.

> [!info] Identifying a redundant or equivalent circuit
> Boolean simplification is A Level (15.2), not AS — but "the instruction is *do not simplify*" implies awareness. A question asking which of two circuits produces the same output, or which gate could be removed, sits at the edge of the AS wording and has not been asked.

> [!abstract] Working from a problem statement — the method
> Read the parameter table first and note what binary 1 means for each letter, because the condition is often the reverse of the intuitive reading (e.g. `A = 1` means daylight is **low**). Then translate each bullet of the prose directly: "and" → AND, "or" → OR, "unless" → AND NOT, "is closed" when 1 = open → NOT. SME's worked example: a fan turns on if temperature **and** humidity are too high **and** the door is closed, **unless** maintenance mode is active → `F = (T AND H) AND (NOT D AND NOT M)`, marked as NOT gates on D and M, the two AND gates, then the combining AND.

> [!abstract] Filling a truth table reliably
> Build the working-space column one gate at a time, left to right through the expression, rather than trying to evaluate the whole thing per row. The marks come in **blocks of four rows**, so a systematic method protects half the marks even if one bracket is misread.
