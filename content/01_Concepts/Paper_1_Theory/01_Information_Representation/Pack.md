---
title: Pack — 1 Information Representation (AS Level)
syllabus: 9618 (2026)
topics: 1.1 Data Representation · 1.2 Multimedia · 1.3 Compression
pairs with: Jigsaw
---

# Pack — 1 Information Representation

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **9608 |** — same rule, using 9608 tariffs. Still inside the 9618 syllabus wording, but untested in the current series.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

> [!note] This Pack is a drill, not a reading
> Topic 1 is the most **procedural** topic in the paper — most of it is conversions and calculations. Do not read the answers; cover them, write the working, then check. A correct answer with no working caps at **1 mark** in almost every calculation question here.

> [!danger] The three slips that cost the most marks
> **1 — The unit.** The divisor changes with the unit asked for: ÷1000 for kB/MB/GB, ÷1024 for KiB/MiB/GiB. Right arithmetic, wrong unit = working mark only.
> **2 — Bit depth given in bytes.** `s24_qp_13_sc_2.a` gives a bit depth of "4 bytes". There is then **no ÷ 8**.
> **3 — Justification questions.** Several carry **no mark for the choice** — all the marks are in the reasoning.

---

# 1.1 Data Representation

## 1.1.1 Binary magnitudes and prefixes

> [!question] 9618 | State one difference between a tebibyte and a gigabyte [1]
> State **one** difference between a tebibyte and a gigabyte.
>
>> [!success]- Answer — 2 routes, 1 mark
>> - **By value:** a tebibyte = 1024 gibibytes // 1 048 576 kibibytes // **2⁴⁰ bytes**, whereas a gigabyte = 1000 megabytes // 1 000 000 kilobytes // **10⁹ bytes**
>> - **By prefix type:** **tebi is a binary prefix and giga is a denary prefix**
>> - The second route is one line and scores the same mark — use it under time pressure
>> - Same answer shape for kibibyte vs megabyte and kibibyte vs kilobyte
>>
>> *Latest: `9618_w24_qp_11_sc_1.a` (also `w23_qp_12_sc_3.a`, `s23_qp_11_sc_3.d.i`)*

> [!question] 9618 | Complete the description of binary and denary prefixes [4]
> Complete the following description. A kibibyte has a ______ prefix. Three kibibytes is the same as ______ bytes. A megabyte has a ______ prefix. Two terabytes is the same as ______ gigabytes.
>
>> [!success]- Answer — 1 mark for each correct answer
>> - A kibibyte has a **binary** prefix
>> - Three kibibytes is the same as **3072** bytes (3 × 1024)
>> - A megabyte has a **decimal / denary** prefix
>> - Two terabytes is the same as **2000** gigabytes (2 × 1000)
>> - Note the question mixes **prefix-type** answers with **arithmetic** answers in the same four marks
>>
>> *Latest: `9618_s24_qp_13_sc_1.a`*

> [!question] 9618 | Tick the largest file size [1]
> Tick **one** box only to identify the largest file size: 3300 kibibytes · 0.3 megabytes · 3 mebibytes · 3300 kilobytes.
>
>> [!success]- Answer — 1 mark
>> - **3300 kibibytes** = 3300 × 1024 = **3 379 200 bytes**
>> - 3 mebibytes = 3 × 1 048 576 = 3 145 728 bytes
>> - 3300 kilobytes = 3 300 000 bytes
>> - 0.3 megabytes = 300 000 bytes
>> - The trap is that "mebibytes" sounds larger — **convert everything to bytes before comparing**
>>
>> *Latest: `9618_s24_qp_12_sc_7.a`*

> [!question] 9618 | Match each binary value to its equivalent unit [5]
> Draw one line from each binary value to its equivalent value: 8 bits · 8000 bits · 1000 kilobytes · 1024 mebibytes · 8192 bits.
>
>> [!success]- Answer — 1 mark per correct line
>> - 8 bits → **1 byte**
>> - 8000 bits → **1 kilobyte** (8000 ÷ 8 = 1000 bytes)
>> - 1000 kilobytes → **1 megabyte**
>> - 1024 mebibytes → **1 gibibyte**
>> - 8192 bits → **1 kibibyte** (8192 ÷ 8 = 1024 bytes)
>> - **1 gigabyte and 1 mebibyte are distractors** with no matching value
>>
>> *Latest: `9618_w21_qp_11_sc_1.a`*

> [!question] Inferred | Explain why both binary and denary prefixes exist [3]
> Explain why computer systems use both binary prefixes and denary prefixes.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Computers **address memory in powers of 2**, so memory sizes are naturally multiples of 1024
>> - … so **binary prefixes** (kibi, mebi, gibi) describe memory **exactly**
>> - Denary prefixes are based on the assumption that **1 kilo = 1000**, from the base-10 system humans use
>> - Storage manufacturers quote capacity in **denary** prefixes, partly because the numbers are larger
>> - This is why a drive sold as "1 TB" shows as roughly **0.91 TiB** on a computer — the same bytes, two naming systems
>>
>> *Inference: every question in either series tests the **difference** between the two systems; none asks the **reason** they both exist.*

> [!question] SME | State the binary and denary value of each prefix [4]
> Complete the table giving the number of bytes represented by each of kilo/kibi, mega/mebi, giga/gibi and tera/tebi.
>
>> [!success]- Answer — 1 mark per row, 4 marks
>> - **kilobyte** 10³ = 1000 · **kibibyte** 2¹⁰ = **1024**
>> - **megabyte** 10⁶ = 1 000 000 · **mebibyte** 2²⁰ = **1 048 576**
>> - **gigabyte** 10⁹ · **gibibyte** 2³⁰ = **1 073 741 824**
>> - **terabyte** 10¹² · **tebibyte** 2⁴⁰
>> - The next row, not in the syllabus: **petabyte** 10¹⁵ · **pebibyte** 2⁵⁰
>>
>> *SME's rule: be precise about **memory** (binary prefixes); a rough estimate is acceptable for **storage** (denary prefixes).*

---

## 1.1.2 Number systems

> [!question] 9618 | Tick the minimum number of bits used to store each example of data [3]
> Put one tick in each row to identify the minimum number of bits used to store each example of data.
>
>> [!success]- Answer — 3 marks for 6 correct ticks, 2 for 4–5, 1 for 2–3
>> - The hexadecimal value F139 → **16** (4 hex digits × 4 bits)
>> - 16 000 000 unique amplitude values → **24** (2²⁴ = 16 777 216)
>> - An **IPv4** address → **32**
>> - 256 unique colours → **8** (2⁸ = 256)
>> - An **IPv6** address → **128**
>> - The denary value 65 000 → **16** (2¹⁶ = 65 536)
>> - Synoptic: needs IP addressing from Topic 2 and colour depth from 1.2
>>
>> *Latest: `9618_w25_qp_13_sc_2.a`*

> [!question] 9618 | State the number of unique binary values representable in 16 bits [1]
> State the number of unique binary values that can be represented in 16 bits.
>
>> [!success]- Answer — 1 mark
>> - **2¹⁶ // 65 536**
>> - The general rule: *n* bits give **2ⁿ** distinct values
>> - The same rule gives colour depth (2ⁿ colours) and sampling resolution (2ⁿ amplitudes)
>>
>> *Latest: `9618_s23_qp_12_sc_4.a`*

> [!question] 9618 | Match each description to its denary value [3]
> Draw one line from each description to its matching denary value: the smallest integer in 8-bit two's complement · the largest integer in 8-bit two's complement · the largest unsigned integer in 8 bits.
>
>> [!success]- Answer — 1 mark per correct line
>> - The smallest integer in 8-bit two's complement → **−128**
>> - The largest integer in 8-bit two's complement → **127**
>> - The largest unsigned integer in 8 bits → **255**
>> - The distractors (−127, −255, −256, 256, 128) are all near-misses
>> - Remember: the two's complement range is **−2ⁿ⁻¹ to +2ⁿ⁻¹ − 1** — **not** symmetrical
>>
>> *Latest: `9618_s23_qp_13_sc_7.a`*

> [!question] 9618 | Write the smallest and largest two's complement integers in 8 bits [2]
> Write the smallest **and** the largest two's complement binary integers that can be represented in 8 bits.
>
>> [!success]- Answer — 1 mark each
>> - Smallest: **1000 0000** (= −128)
>> - Largest: **0111 1111** (= +127)
>> - Read carefully whether the **binary pattern** or the **denary value** is wanted — both versions are set
>>
>> *Latest: `9618_s25_qp_12_sc_2.b.ii` (also `s23_qp_11_sc_3.d.iv`)*

> [!question] 9618 | State two benefits of using Binary Coded Decimal [2]
> State **two** benefits of using Binary Coded Decimal (BCD) to represent values.
>
>> [!success]- Answer — 1 mark per benefit, max 2
>> - It is **straightforward to convert to and from denary**
>> - … so it is **less complex to encode and decode** for programmers
>> - It is **easier for digital equipment** that uses BCD to display output information
>> - It can represent **monetary values exactly**
>>
>> *Latest: `9618_w22_qp_13_sc_9.b`*

> [!question] 9618 | State why a value cannot be interpreted as BCD [1]
> State why the value in the register cannot be interpreted as Binary Coded Decimal (BCD).
>
>> [!success]- Answer — 1 mark
>> - **The denary value in each group of 4 bits is greater than 9**
>> - … // the denary value in each **nibble** is greater than 9
>> - Any nibble from `1010` to `1111` is **invalid BCD**, because BCD only uses 0000–1001
>>
>> *Latest: `9618_w21_qp_12_sc_4.d`*

> [!question] 9618 | Give the 8-bit one's complement representation of a negative number [2]
> Give the 8-bit one's complement representation of the denary number −120. Show your working.
>
>> [!success]- Answer — 1 mark for working, 1 for the answer
>> - **Working:** +120 = **0111 1000**
>> - **Answer:** **1000 0111**
>> - One's complement is just **invert every bit** — no "add 1"
>> - This is the **only** one's complement question in the 9618 series
>>
>> *Latest: `9618_s23_qp_12_sc_4.b`*

> [!question] Inferred | Explain the weakness of one's complement [2]
> Explain one disadvantage of using one's complement rather than two's complement to represent negative numbers.
>
>> [!success]- Answer — 4 points for 2 marks
>> - One's complement has **two representations for zero**
>> - … `0000 0000` (positive zero) and `1111 1111` (negative zero)
>> - … which wastes a value and **complicates comparison and arithmetic**
>> - Two's complement has only **one** representation of zero, and the range is one value larger
>>
>> *Inference: the syllabus names **one's and two's complement**. 9618 has asked one's complement exactly once, as a conversion. Its defining weakness has never been examined in either series, though SME teaches it.*

> [!question] Inferred | Explain why two's complement is used for negative numbers [3]
> Explain why computers use two's complement rather than sign-and-magnitude to represent negative numbers.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Subtraction can be carried out as **addition of the negative**
>> - … so the **same adder circuit** handles both operations, and no separate subtraction hardware is needed
>> - The process is the **same for any combination of signs** — no special logic to detect the signs first
>> - There is only **one representation of zero**
>> - The **leftmost column simply becomes negative** (−128 in 8 bits), so the normal column-value method still works
>>
>> *Inference: untested in either series. SME makes the hardware-simplicity point explicitly; no mark scheme does.*

> [!question] SME | Describe what is meant by a number base [2]
> Describe what is meant by a number base, and state the base of binary, denary and hexadecimal.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A number base is the **number of distinct digits or symbols** the number system uses
>> - Each **column** represents a **power of the base**, increasing from the right
>> - **Binary** is base 2 (digits 0–1) · **denary** is base 10 (0–9) · **hexadecimal** is base 16 (0–9 then A–F)
>> - One hexadecimal digit represents exactly **four bits** — one nibble
>>
>> *Inference/SME: every question uses the bases; none asks what a base means. The nibble relationship is what makes binary↔hex conversion instant.*

---

## 1.1.3 Converting between bases and representations

> [!question] 9618 | Convert a binary number into hexadecimal [1]
> Convert the binary number `101100111010` into hexadecimal.
>
>> [!success]- Answer — 1 mark
>> - Split into nibbles **from the right**: `1011 | 0011 | 1010`
>> - 1011 = 11 = **B** · 0011 = **3** · 1010 = 10 = **A**
>> - Answer: **B3A**
>> - More: `110001100111` → **C67** · `1110001100111011` → **E33B**
>>
>> *Latest: `9618_w25_qp_13_sc_2.d` (also `w25_qp_11_sc_1.a.i`, `w24_qp_11_sc_1.b.i`)*

> [!question] 9618 | Convert a hexadecimal number into denary [2]
> Convert the hexadecimal number C0F into denary. Show your working.
>
>> [!success]- Answer — 1 mark for working, 1 for the answer
>> - **Working:** C = 12, so (12 × 16²) + (0 × 16¹) + (15 × 16⁰)
>> - = 3072 + 0 + 15
>> - **Answer: 3087**
>> - Also: `1FAB` → **8107**
>>
>> *Latest: `9618_s24_qp_12_sc_7.c` (also `w24_qp_13_sc_8.a`)*

> [!question] 9618 | Convert a denary number to hexadecimal [1]
> Convert the denary number 241 to hexadecimal.
>
>> [!success]- Answer — 1 mark
>> - 241 ÷ 16 = **15 remainder 1**
>> - First digit = 15 = **F**, second digit = **1**
>> - Answer: **F1**
>> - Alternative route: 241 = `1111 0001` in binary → F1
>>
>> *Latest: `9618_s24_qp_13_sc_1.b`*

> [!question] 9618 | Convert a denary integer into 12-bit binary and hexadecimal [2]
> Convert the denary integer 558 into 12-bit binary and hexadecimal.
>
>> [!success]- Answer — 1 mark each
>> - Binary: 558 = 512 + 32 + 8 + 4 + 2 = **0010 0010 1110**
>> - Hexadecimal: group the nibbles — 0010 = 2, 0010 = 2, 1110 = E → **22E**
>> - Doing the **binary first** gives the hexadecimal free
>>
>> *Latest: `9618_s25_qp_12_sc_2.a`*

> [!question] 9618 | Convert a denary number into a 12-bit two's complement binary number [1]
> Convert the denary number −108 into a 12-bit two's complement binary number.
>
>> [!success]- Answer — 1 mark
>> - +108 = **0000 0110 1100** (pad to 12 bits **first**)
>> - Invert: `1111 1001 0011`
>> - Add 1: **1111 1001 0100**
>> - Also: −196 → **1111 0011 1100**
>> - **Pad to the full width before inverting** — inverting 8 bits then padding gives the wrong answer
>>
>> *Latest: `9618_w25_qp_13_sc_2.b` (also `w23_qp_12_sc_3.b.i`)*

> [!question] 9618 | Convert a two's complement binary integer into denary [2]
> Convert the 12-bit two's complement binary integer `111110111100` into denary. Show your working.
>
>> [!success]- Answer — 1 mark for the working, 1 for the denary value
>> - **Method 1:** flip the bits → `0000 0100 0011`, add 1 → `0000 0100 0100` = 68, so the value is **−68**
>> - **Method 2:** treat the MSB as negative — −2048 + 1024 + 512 + 256 + 128 + 32 + 16 + 8 + 4 = **−68**
>> - Both methods are credited
>> - More: `11100010` → **−30** · `10010110` → **−106** · `100110010111` → **−1641** · `11001101` → **−51**
>>
>> *Latest: `9618_w25_qp_11_sc_1.a.iii` (also `s25_qp_12_sc_2.b.i`, `w24_qp_11_sc_1.b.ii`)*

> [!question] 9618 | Explain how to convert two's complement to denary, and give the value [3]
> Explain how to convert the two's complement integer `10011111` into denary. Give the denary value after conversion.
>
>> [!success]- Answer — 1 mark per method bullet (max 2) + 1 for the conversion
>> - **Flip each bit then add 1** …
>> - … then use the **method of converting the new binary number into denary** (and make it negative)
>> - *or:* the **most significant 1 bit is treated as the corresponding negative denary value** …
>> - … then **add the other positive corresponding denary values**
>> - **Denary value: −97**
>> - The command word is **explain** — the method must be written out, not just the answer
>>
>> *Latest: `9618_w24_qp_13_sc_8.b`*

> [!question] 9618 | Convert a denary number into Binary Coded Decimal [1]
> Convert the denary number 964 into Binary Coded Decimal (BCD).
>
>> [!success]- Answer — 1 mark
>> - 9 → `1001` · 6 → `0110` · 4 → `0100`
>> - Answer: **1001 0110 0100**
>> - Also: 108 → **0001 0000 1000** — the leading zeros of `0001` must be written
>> - BCD codes **each digit separately**; it is not the binary value of the whole number
>>
>> *Latest: `9618_s23_qp_11_sc_3.d.ii` (also `w25_qp_11_sc_1.a.ii`)*

> [!question] 9618 | Convert Binary Coded Decimal into denary [1]
> Convert the Binary Coded Decimal value `100001100101` into denary.
>
>> [!success]- Answer — 1 mark
>> - Split into nibbles: `1000 | 0110 | 0101`
>> - 1000 = 8 · 0110 = 6 · 0101 = 5
>> - Answer: **865**
>> - Also: `010101110011` → **573**
>>
>> *Latest: `9618_w23_qp_12_sc_3.b.ii` (also `w24_qp_11_sc_1.b.iii`)*

> [!question] 9618 | Convert an unsigned binary integer into BCD, showing working [2]
> Convert the unsigned binary integer `10010101` into Binary Coded Decimal (BCD). Show your working.
>
>> [!success]- Answer — 1 mark for each bullet
>> - **Working:** `10010101` = 128 + 16 + 4 + 1 = **149 decimal**
>> - **Answer:** 1 → `0001`, 4 → `0100`, 9 → `1001` = **0001 0100 1001**
>> - The intermediate **denary value is itself a mark** — always write it down
>>
>> *Latest: `9618_w22_qp_12_sc_2.a.iii`*

> [!question] 9618 | Complete a character table across denary, binary and hexadecimal [3]
> Complete the table by filling in the missing numbers for each extended ASCII character.
>
>> [!success]- Answer — 1 mark for each correctly completed space
>> - `!` denary 33, hex 21 → 8-bit binary **0010 0001**
>> - `L` binary `0100 1100`, hex 4C → denary **76**
>> - `ü` denary 252, binary `1111 1100` → hexadecimal **FC**
>> - Three conversions, each in a **different direction** — read which column is blank
>>
>> *Latest: `9618_s25_qp_13_sc_1.c.ii`*

> [!question] Inferred | Convert a hexadecimal number into binary [1]
> Convert the hexadecimal number 5F into binary.
>
>> [!success]- Answer — 1 mark
>> - Each hex digit becomes **one nibble**
>> - 5 → `0101` · F = 15 → `1111`
>> - Answer: **0101 1111**
>> - The easiest of the nine conversions, and the only one 9618 has never set on its own
>>
>> *Inference: 9618 asks binary→hex repeatedly and hex→denary repeatedly, but a bare "convert this hexadecimal into binary" appears only **inside** character tables, never as its own question.*

> [!question] Inferred | Convert a negative denary number into hexadecimal [2]
> Convert the denary number −68 into a 12-bit two's complement value, and give that value in hexadecimal.
>
>> [!success]- Answer — 1 mark for the two's complement, 1 for the hex
>> - +68 = `0000 0100 0100`
>> - Invert and add 1 → **1111 1011 1100**
>> - Group into nibbles: 1111 = F, 1011 = B, 1100 = C
>> - Hexadecimal: **FBC**
>>
>> *Inference: all hexadecimal conversions in 9618 use positive values, though both halves of this have been separately examined.*

---

## 1.1.4 Binary addition and subtraction

> [!question] 9618 | Perform binary addition, showing working [2]
> Perform the following binary addition. Show your working. `10101010 + 00110111`
>
>> [!success]- Answer — 1 mark for the answer, 1 for the working
>> - ```
>>     1010 1010
>>   + 0011 0111
>>   ───────────
>>     1110 0001
>>      1 1 1 1 1   ← carries
>>   ```
>> - **Answer: 1110 0001**
>> - **Write the carry row** — it is literally the working mark
>>
>> *Latest: `9618_w21_qp_11_sc_1.b.i`*

> [!question] 9618 | Add a denary number to a binary number, in binary [3]
> Add the denary number 15 to the binary number `00100011`. Perform the addition in binary and give your answer in binary. Show your working.
>
>> [!success]- Answer — 1 mark per bullet
>> - **Converting 15 to binary:** `0000 1111`
>> - **Method for the addition** (the carry row shown)
>> - ```
>>     0010 0011
>>   + 0000 1111
>>   ───────────
>>     0011 0010
>>        1  111   ← carries
>>   ```
>> - **Final answer: 0011 0010**
>> - The **conversion step is a separate mark** from the addition
>>
>> *Latest: `9618_s21_qp_11_sc_1.c.ii`*

> [!question] 9618 | Subtract a denary number from a two's complement binary number [3]
> Subtract the denary number 10 from the two's complement representation `00100011`. Give your answer in binary and show your working.
>
>> [!success]- Answer — 1 mark per bullet
>> - **Converting −10 to two's complement binary:** 10 = `0000 1010`, so −10 = **1111 0110**
>> - **Adding the values**
>> - ```
>>     0010 0011
>>   + 1111 0110
>>   ───────────
>>     0001 1001
>>       11   11   ← carries
>>   ```
>> - **Final answer: 0001 1001**
>> - The carry out of the top bit is **discarded** — that is normal, not an overflow
>>
>> *Latest: `9618_s21_qp_11_sc_1.c.iii` (also `w24_qp_11_sc_1.c`)*

> [!question] 9618 | Subtract one denary number from another using binary subtraction [3]
> Subtract the denary number 10 from the denary number 100 using binary subtraction. Show your working.
>
>> [!success]- Answer — 1 mark each
>> - **Converting both:** 100 = **0110 0100** and 10 = **0000 1010**
>> - **Subtraction method** — convert 10 to −10 and add, **or** direct subtraction
>> - **Correct answer: 0101 1010**
>> - *Method 1 (two's complement):* −10 = `1111 0110`; `0110 0100 + 1111 0110` = (1)`0101 1010`
>> - *Method 2 (direct):* borrow as in denary — `0110 0100 − 0000 1010` = `0101 1010`
>> - **Both methods are equally credited** — direct borrowing is not penalised
>>
>> *Latest: `9618_s24_qp_12_sc_7.b`*

> [!question] 9618 | State how an overflow can occur when adding two binary integers [1]
> State how an overflow can occur when adding two binary integers.
>
>> [!success]- Answer — 2 phrasings for 1 mark
>> - **The result is a larger number than can be stored in the given number of bits**
>> - … // the result is **greater than 255** (for 8 unsigned bits)
>>
>> *Latest: `9618_w21_qp_11_sc_1.b.ii`*

> [!question] Inferred | Explain how overflow affects a signed addition [3]
> Explain how overflow can occur when adding two signed binary integers, and describe its effect.
>
>> [!success]- Answer — 5 points for 3 marks
>> - In a signed representation the **leftmost bit is the sign bit**
>> - Adding two large positive numbers can **carry into the sign bit**
>> - … which **flips the sign**, so the result appears **negative**
>> - … e.g. in 8 bits, 127 + 1 gives `1000 0000` = **−128**
>> - The extra bits are **truncated or wrapped around**, so the result is incorrect or unpredictable
>> - The same applies adding two large negatives, which can produce a positive
>>
>> *Inference: the syllabus says "show understanding of **how overflow can occur**", but there is exactly one 9618 question on it — 1 mark, in w21. Sign-bit overflow is in SME and in no mark scheme.*

> [!question] SME | Explain why the extra bit is discarded in two's complement subtraction [2]
> When 48 − 12 is performed in 8-bit two's complement, a ninth bit is produced. Explain why this is ignored.
>
>> [!success]- Answer — 4 points for 2 marks
>> - 48 = `0011 0000`, −12 = `1111 0100`; adding gives **(1)0010 0100**
>> - `0010 0100` = **36**, which is the correct answer
>> - The ninth bit is a **by-product of the two's complement method**, not part of the value
>> - True **overflow** is different — that is when the result itself will not fit in the available bits
>>
>> *SME's worked example; the distinction between a discarded carry and a genuine overflow is in no mark scheme.*

---

## 1.1.5 Practical applications of BCD and hexadecimal

> [!question] 9618 | Give one application where BCD is used and justify its use [2]
> Give **one** application where Binary Coded Decimal (BCD) is used and justify its use.
>
>> [!success]- Answer — 1 mark for the application, 1 for a **corresponding** justification
>> - **Financial / banking calculations** … because transactions use only **two decimal places and must be accurate**, with no accumulating or rounding errors, and it is difficult to represent decimal values exactly in normal binary
>> - **Electronic displays** (calculators, digital clocks) … because visual displays only need to show **individual digits**
>> - … and because conversion between denary and BCD is **straightforward**
>> - **Storage of the date and time in the BIOS** of a PC … because conversion between denary and BCD is more straightforward
>> - **Barcode systems** … because conversion between denary and BCD can be **accurately completed**
>> - The justification must **match the application named** — a mismatched pair scores 1
>>
>> *Latest: `9618_s25_qp_12_sc_2.c` (also `w23_qp_12_sc_3.c`)*

> [!question] 9608 | Describe a use of BCD number representation [2]
> Describe a use of BCD number representation.
>
>> [!success]- Answer — 3 points for 2 marks
>> - When **denary numbers need to be electronically coded**
>> - … e.g. to operate the displays on a **calculator**, where each digit is represented separately
>> - **Decimal fractions can be accurately represented**
>> - Also credited: any scenario where a **single digit needs to be transmitted or displayed** — a calculator, a digital clock
>>
>> *Latest: `9608_s15_qp_13_sc_1.b.ii` (also `w19_qp_11_sc_5.c.ii`, `w17_qp_13_sc_1.b.iii`). The "electronically coded" framing is 9608-only.*

> [!question] Inferred | Describe two practical applications of hexadecimal and justify them [4]
> Describe **two** practical applications where hexadecimal is used, and justify its use in each.
>
>> [!success]- Answer — 2 marks per application (use + justification), 4 marks
>> - **MAC addresses and IPv6 addresses** … a 48-bit or 128-bit address written in binary would be enormously long and error-prone; hexadecimal is far shorter and easier to read and transcribe
>> - **Colour codes in HTML / CSS** (e.g. `#FF0000`) … two hex digits give the 0–255 value of each of red, green and blue in a compact form
>> - **Memory addresses and memory dumps** … hexadecimal is a compact shorthand for long binary addresses, and **one hex digit maps exactly to four bits**, so conversion is trivial
>> - **Assembly language operands and error codes** … values can be written compactly and converted to binary at a glance
>> - **Character code tables** (ASCII and Unicode) … codes are conventionally quoted in hexadecimal
>> - The underlying justification in every case: hexadecimal is **easier for humans to read and less error-prone than binary**, while converting to and from binary instantly
>>
>> *Inference: **the single clearest gap in Topic 1.** The bullet is titled "practical applications where Binary Coded Decimal (BCD) **and Hexadecimal** are used", yet every question in **both** series asks only about BCD. Several of these applications are already examined elsewhere (MAC and IPv6 in Topic 2, memory addresses in Topic 4), which makes a synoptic question easy to set.*

> [!question] Inferred | State two drawbacks of using BCD [2]
> State **two** drawbacks of using Binary Coded Decimal to represent values.
>
>> [!success]- Answer — 4 points for 2 marks
>> - BCD **wastes storage space**
>> - … because 4 bits can represent 16 patterns but BCD uses only **10** of them
>> - **Arithmetic is more complex** than in pure binary
>> - … so it needs more processing, or dedicated hardware, to perform calculations
>>
>> *Inference: both series ask only for the **benefits** of BCD. The costs are the obvious counterweight and have never been asked.*

> [!question] SME | Give four use cases for BCD and the reason for each [4]
> Give four situations where BCD is used and explain why BCD suits each.
>
>> [!success]- Answer — 1 mark per use with its reason, 4 marks
>> - **Electronic calculators** — keeps numbers in decimal format for easier display and accuracy
>> - **Digital clocks and watches** — time is naturally decimal (12:45), so the display logic is simpler
>> - **Banking and financial systems** — avoids rounding errors in decimal calculations, especially with money
>> - **Older digital and embedded systems** — simpler to implement with hardware that drives one digit at a time
>>
>> *9618's own BCD question is marked at 2 (application + justification); four pairs justifies 4.*

---

## 1.1.6 Character sets

> [!question] 9618 | Explain how text is represented by a character set [2]
> Explain how text is represented by the ASCII character set.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - Each character has a **unique** code
>> - Each character in the text is **replaced sequentially / in order** by its code
>> - The codes are **stored in the order they appear** in the word
>> - The same three-part shape as the bitmap and sound answers: **unit → unique code → stored in sequence**
>>
>> *Latest: `9618_w25_qp_13_sc_1.b` (also `s24_qp_13_sc_1.d.ii`, `s21_qp_12_sc_6.b`)*

> [!question] 9618 | Give one similarity and two differences between ASCII and Unicode [3]
> Give **one** similarity and **two** differences between the ASCII and Unicode character sets.
>
>> [!success]- Answer — 1 mark for the similarity, 2 for differences
>> - **Similarity (max 1):** both **can** use 8 bits
>> - … // both represent each character using a **unique code**
>> - … // Unicode contains all the characters ASCII contains — **ASCII is a subset of Unicode**
>> - **Difference:** Unicode can go **up to 32 bits** per character whereas ASCII is **7 or 8**
>> - **Difference:** Unicode can represent a **wider range of characters** than ASCII
>> - **Difference:** different **languages** are represented in Unicode; ASCII is only for one
>> - A similarity written in the difference box scores nothing — the boxes are marked separately
>>
>> *Latest: `9618_w22_qp_11_sc_1.c`*

> [!question] 9618 | Give two differences between ASCII and Unicode [2]
> Give **two** differences between the ASCII and Unicode character sets.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - **ASCII uses 7 or 8 bits; Unicode can use many more — up to 32**
>> - Unicode can represent a **wider range of characters, including different languages**
>>
>> *Latest: `9618_w25_qp_13_sc_1.c`*

> [!question] 9618 | Give two advantages of Unicode instead of ASCII [2]
> Give **two** advantages of using the Unicode character set instead of the ASCII character set.
>
>> [!success]- Answer — 1 mark each to max 2
>> - A **wider range of characters** can be represented
>> - … so characters from **more languages** can be represented
>> - … and symbols such as **emojis** can be used
>>
>> *Latest: `9618_s25_qp_11_sc_3.b.i`*

> [!question] 9618 | Give two characteristics of the Unicode character set [2]
> Give **two** characteristics of the Unicode character set.
>
>> [!success]- Answer — 1 mark each to max 2
>> - **8 / 16 / 32 bits** per character
>> - Represents **2⁸ / 2¹⁶** etc. characters
>> - Represents **every language** and other characters such as **emojis**
>>
>> *Latest: `9618_s25_qp_13_sc_1.c.i`*

> [!question] 9618 | Identify and describe one character set [2]
> A character set is used to represent characters in a computer. Identify **and** describe **one** character set.
>
>> [!success]- Answer — 1 mark for identification, 1 for a **matching** description
>> - **ASCII** — 7/8 bits per character // represents 128/256 characters // represents all characters from the **Latin alphabet**
>> - **UNICODE** — 8/16/32 bits per character // represents 256/65 536+ characters // represents **all characters in all languages**
>> - The description must match the set **named** — describing Unicode after naming ASCII scores 1
>>
>> *Latest: `9618_w24_qp_13_sc_6.a`*

> [!question] 9618 | State the number of bits each character set allocates [1]
> Complete the table by identifying the number of bits each character set allocates to each character: ASCII, extended ASCII, Unicode.
>
>> [!success]- Answer — 1 mark for **all three** correct
>> - ASCII → **7**
>> - extended ASCII → **8**
>> - Unicode → **16 / 32**
>> - All-or-nothing — two right and one wrong scores zero
>>
>> *Latest: `9618_s24_qp_13_sc_1.d.i`*

> [!question] 9618 | State how many characters ASCII and extended ASCII can represent [2]
> State the number of characters that can be represented by the ASCII character set and by the extended ASCII character set.
>
>> [!success]- Answer — 1 mark each
>> - ASCII = **128 // 2⁷**
>> - Extended ASCII = **256 // 2⁸**
>>
>> *Latest: `9618_s21_qp_12_sc_6.a`*

> [!question] 9618 | Convert a character's code between representations [1]
> The ASCII value for the character 'h' has the denary value 104. Write the BCD value and the hexadecimal value for 'h'.
>
>> [!success]- Answer — 1 mark each
>> - **BCD:** 1 → `0001`, 0 → `0000`, 4 → `0100` = **0001 0000 0100**
>> - **Hexadecimal:** 104 ÷ 16 = 6 remainder 8 = **68**
>> - More: Unicode `ɮ` = `0010 0111 0110 1110` → denary **10 094** · Unicode `∑` = hex 2140 → denary **8512** · Unicode `1` = denary 49 → hex **31** · Unicode `5` → denary **53**
>> - Character-set questions are usually **conversion questions in disguise**
>>
>> *Latest: `9618_w25_qp_12_sc_7.c.i`/`c.ii` (also `s25_qp_11_sc_3.b.ii`/`b.iii`, `s21_qp_12_sc_6.c`)*

> [!question] 9618 | Use a code table to decode received binary values [1]
> Use the table of words and denary values to find the words corresponding to the binary values `00111000`, `00111100` and `00111110`.
>
>> [!success]- Answer — 1 mark for correct words **in the correct order**
>> - `0011 1000` = 56 → **Science**
>> - `0011 1100` = 60 → **is**
>> - `0011 1110` = 62 → **Amazing!**
>> - Convert each binary value to denary **first**, then look it up
>>
>> *Latest: `9618_w25_qp_12_sc_6.b`*

> [!question] 9608 | Define the term character set [1]
> Define the term **character set**.
>
>> [!success]- Answer — 1 mark from
>> - The **symbols that the computer recognises / uses**
>> - A **list of characters** recognised by the computer hardware and software
>> - … each one given a **unique binary code**
>>
>> *Latest: `9608_s18_qp_12_sc_4.b.i`. 9618 has never asked for the definition itself — only for how one works.*

> [!question] 9608 | Give two disadvantages of using ASCII [2]
> Give **two** disadvantages of using ASCII code.
>
>> [!success]- Answer — 1 mark each, any two
>> - Only **128 / 256** characters can be represented
>> - It uses values **0 to 127** (or 255 if extended) / one byte
>> - **Many characters used in other languages cannot be represented**
>> - In extended ASCII, the characters from **128 to 255 may be coded differently in different systems**
>> - That last point — extended ASCII is **not consistently standardised** — appears in no 9618 mark scheme
>>
>> *Latest: `9608_w16_qp_13_sc_8.c.i`*

> [!question] 9608 | Describe how Unicode overcomes the disadvantages of ASCII [2]
> Describe how Unicode is designed to overcome the disadvantages of ASCII.
>
>> [!success]- Answer — 1 mark each, any two
>> - Uses **16, 24 or 32 bits** / two, three or four bytes
>> - Unicode is designed to be a **superset of ASCII**
>> - Designed so that **most characters in other languages** can be represented
>> - **Superset** is the sharp version of 9618's "ASCII is a subset of Unicode"
>>
>> *Latest: `9608_w16_qp_13_sc_8.c.ii`*

> [!question] 9608 | Calculate a character code from another character's code [2]
> The ASCII code for 'A' is 41 in hexadecimal. Calculate the ASCII code in hexadecimal for 'Z'. Show your working.
>
>> [!success]- Answer — 1 mark for working, 1 for the answer
>> - **Working:** code for Z = code for A + 25₁₀ (A is the 1st letter, Z the 26th)
>> - 25₁₀ = 19₁₆
>> - 41₁₆ + 19₁₆ = **5A₁₆**
>> - This works **only because character sets are ordered logically** — each letter's code is one more than the last
>>
>> *Latest: `9608_s18_qp_12_sc_4.b.iii` (also `9608_s19_qp_12_sc_3.d.iii`, Unicode 'G' = 0047 so 'D' = **0044**)*

> [!question] Inferred | Explain the logical ordering of a character set [3]
> Explain what is meant by saying a character set is logically ordered, and give one benefit.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Codes are assigned in **sequence**, so the code for 'B' is **one more than** the code for 'A'
>> - … which means characters can be **sorted alphabetically** by comparing their codes directly
>> - … and a character's code can be **calculated** from another's rather than looked up
>> - In ASCII, **only the sixth bit differs** between a capital and its lower-case letter (`A` = `0100 0001`, `a` = `0110 0001`)
>> - … so **case conversion is a single bit operation**, which is fast
>>
>> *Inference: 9608 exploits the ordering in a calculation question, but **neither series has ever asked about the property itself** — even though it is why character sets are designed this way.*

> [!question] SME | Compare ASCII and Unicode feature by feature [4]
> Compare the ASCII and Unicode character sets in terms of bits, characters, uses, benefits and drawbacks.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Bits:** ASCII 7 · extended ASCII 8 · Unicode minimum 16
>> - **Characters:** 128 · 256 · 65 536+
>> - **Covers:** ASCII the standard English keyboard; extended ASCII adds operators and symbols such as ©; Unicode all major world languages and emoji
>> - **Benefit of ASCII:** uses far **less storage space**
>> - **Benefit of Unicode:** represents **all common characters worldwide**, including special characters
>> - **Drawback of Unicode:** uses considerably **more storage space**
>> - The first **128 Unicode code points are identical to ASCII**, which is what makes it backward compatible
>>
>> *9618's own comparison question carries 3; the full table justifies 4.*

---

# 1.2 Multimedia

## 1.2.1 How bitmap data is encoded

> [!question] 9618 | Describe how the data for a bitmapped image is encoded [3]
> Describe how the data for a bitmapped image is encoded.
>
>> [!success]- Answer — 1 mark each
>> - The image is **made of pixels** and **each pixel has one colour**
>> - Each colour has a **unique binary code**
>> - The **code for the colour of each pixel is stored in sequence**
>> - Identical structure to the character-set and sound answers — learn the shape once
>>
>> *Latest: `9618_s24_qp_12_sc_2.d.i`*

> [!question] 9618 | Define the bitmap terms [3]
> Complete the table by defining the image terms: pixel, colour depth, file header.
>
>> [!success]- Answer — 1 mark for each correct definition
>> - **Pixel** — the smallest part of the image // one square or dot of **one colour** // the smallest **addressable** element in an image
>> - **Colour / bit depth** — the number of **bits per pixel** // the number of bits used to represent each colour // determines the **number of colours** that can be represented
>> - **File header** — stores **data about the image file** / **metadata**
>> - **Drawing list** (if asked alongside) — all the drawing objects in an image // a list storing the commands required to draw each object
>>
>> *Latest: `9618_s23_qp_11_sc_1.a` (also `w24_qp_12_sc_7.a.i`, `s21_qp_11_sc_1.a.i`)*

> [!question] 9618 | Complete the statements about bitmap images [2]
> Complete the statements about bitmap images by writing the missing words.
>
>> [!success]- Answer — 1 mark per correctly completed term
>> - The **bit depth** of a bitmap image is the number of bits that are used to store each pixel
>> - Metadata about the image is stored in the **header** of the file
>>
>> *Latest: `9618_w22_qp_13_sc_2.e`*

> [!question] 9618 | Complete the table of bitmap statements [3]
> Complete the table by writing the answer for each statement about a bitmapped image.
>
>> [!success]- Answer — 1 mark for each correct answer
>> - The term for the smallest element that makes up an image → **pixel**
>> - The largest number of different colours representable with a bit depth of 8 bits → **256 // 2⁸**
>> - The term for the dots per inch (dpi) when an image is displayed → **screen resolution**
>> - The third row is the only place **screen resolution** has ever been the answer in 9618
>>
>> *Latest: `9618_s25_qp_11_sc_3.a`*

> [!question] 9618 | Identify two other items in a bitmap file header [2]
> Colour depth and image resolution are both included in the file header of a bitmap image. Identify **two other** items that could be included.
>
>> [!success]- Answer — 1 mark each to max 2
>> - **Confirmation that it is a bitmap // the file type**
>> - The **compression type** used
>> - The **location / offset of the data** within the file
>> - The **dimensions**, e.g. 100 × 100 pixels
>> - Colour depth and image resolution are **excluded by the question**
>>
>> *Latest: `9618_s23_qp_11_sc_1.b.i`*

> [!question] 9618 | Explain why the actual file size is larger than the calculated estimate [2]
> Explain why the actual file size of a bitmap image may be larger than the one you calculated.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - The file will contain **metadata**
>> - The file will have a **header**
>> - … which stores the file type, dimensions, colour depth and compression type, none of which the formula counts
>> - This is why every file-size question asks for an **estimate**
>>
>> *Latest: `9618_w25_qp_11_sc_7.d.ii`*

> [!question] Inferred | Explain the difference between image resolution and screen resolution [3]
> Explain the difference between image resolution and screen resolution.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Image resolution** is a property of the **file** — the number of pixels making up the image, width × height
>> - … so it directly affects the **file size**
>> - **Screen resolution** is a property of the **display** — the number of pixels the monitor can show
>> - … so changing it has **no effect on the file size** of the image
>> - If the image resolution exceeds the screen resolution, the image is **scaled down to fit**, and detail is not visible
>>
>> *Inference: both terms are named in the syllabus. Image resolution is examined constantly; screen resolution appears once as a one-word answer and once as a distractor. The distinction has never been the subject of a question.*

> [!question] SME | Explain what pixel density is and why it matters [3]
> Explain what is meant by pixel density and why it affects perceived image quality.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Pixel density is the number of **pixels per inch (PPI)** of a display
>> - It depends on the screen resolution **and the physical size** of the screen
>> - … so a large screen and a small screen with the same resolution have **different densities**
>> - A 65″ 4K television works out at roughly **68 PPI**; a modern smartphone exceeds **300 PPI**
>> - At low density and close viewing distance the **pixel grid becomes visible** and fine detail is lost
>>
>> *SME's extension of the screen-resolution row that 9618 does examine; it explains why "dpi" is the credited term.*

---

## 1.2.2 Calculating bitmap file size

> [!question] 9618 | Calculate the file size of a bitmap image in megabytes [2]
> A bitmap image has a resolution of 1000 pixels wide by 2000 pixels high. The colour depth is 16 bits. Calculate an estimate of the file size in megabytes. Show your working.
>
>> [!success]- Answer — 1 mark for the working, 1 for the answer
>> - **Working:** (1000 × 2000 × 16) ÷ (8 × 1000 × 1000)
>> - … // (1000 × 2000 × 2) ÷ (1000 × 1000)
>> - **Answer: 4 megabytes**
>> - Others: 2 000 000 pixels × 16 bits ÷ (8 × 1000 × 1000) = **4 MB**
>> - … 1500 × 3000 × **8 bytes** ÷ 1000 ÷ 1000 = **36 MB** — note **no ÷ 8**, the depth is in bytes
>>
>> *Latest: `9618_w25_qp_12_sc_6.d` (also `s25_qp_13_sc_1.a.i`, `s23_qp_11_sc_1.b.ii`)*

> [!question] 9618 | Calculate the file size where the bit depth is given in bytes [2]
> A photograph has a resolution of 4000 pixels wide by 3000 pixels high. The bit depth is 4 bytes. Calculate an estimate for the file size in megabytes. Show your working.
>
>> [!success]- Answer — 1 mark for the working, 1 for the answer
>> - **Working:** 4000 × 3000 × 4
>> - **Answer: 48 MB**
>> - **There is no ÷ 8** — the depth is already in **bytes**, so the product is already in bytes
>> - 48 000 000 bytes ÷ 1 000 000 = 48 MB
>> - The single most common slip in this bullet: dividing by 8 anyway gives 6 MB and loses the answer mark
>>
>> *Latest: `9618_s24_qp_13_sc_2.a`*

> [!question] 9618 | Calculate the file size of a bitmap image in kibibytes [2]
> Calculate the file size of a bitmap image with an image resolution of 2048 × 1024 pixels and a bit depth of 16 bits. Give your answer in kibibytes. Show your working.
>
>> [!success]- Answer — 1 mark for the answer, 1 for the working
>> - **Working:** (2048 × 1024 × 16) ÷ (8 × **1024**)
>> - **Answer: 4096 kibibytes**
>> - Kibibytes → divide by **1024**, not 1000
>> - Also: 512 × 2048 × 8 ÷ (8 × 1024) = **1024 kibibytes // 2¹⁰ kibibytes** — "a maximum of 256 colours" means a bit depth of **8**
>>
>> *Latest: `9618_w23_qp_13_sc_2.b` (also `w25_qp_11_sc_7.d.i`)*

> [!question] 9618 | Calculate the file size of a bitmap image in mebibytes [3]
> The image is scanned with an image resolution of 1024 × 512 pixels and a colour depth of 8 bits per pixel. Calculate an estimate for the file size in mebibytes. Show your working.
>
>> [!success]- Answer — 1 mark per working bullet, 1 for the answer
>> - **Working:** 1024 × 512 = **524 288** pixels/bytes (at 8 bits = 1 byte per pixel)
>> - **Working:** 524 288 ÷ 1024 ÷ 1024
>> - **Answer: 0.50 mebibytes**
>> - Also: (2048 × 1024 × 10) ÷ (8 × 1024 × 1024) = **2.5 mebibytes**
>> - Mebibytes → divide by 1024 **twice**
>>
>> *Latest: `9618_s21_qp_11_sc_1.a.ii` (also `w23_qp_12_sc_6.c`)*

> [!question] 9618 | Calculate the file size of one second of video [2]
> A video is made of many bitmap images called frames. 30 frames are recorded every second. Each frame is 4000 pixels wide by 3000 pixels high, using 16-bit colour depth. Calculate an estimate for the file size for one second of video in gigabytes. Show your working.
>
>> [!success]- Answer — 1 mark for the working, 1 for the answer
>> - **Working:** (4000 × 3000 × 30 × 16) ÷ (8 × 1000 × 1000 × 1000)
>> - … // (4000 × 3000 × 30 × 2) ÷ (1000 × 1000 × 1000)
>> - **Answer: 0.72 gigabytes**
>> - A video is just a sequence of bitmaps — the **frame rate is one more multiplier**
>>
>> *Latest: `9618_w25_qp_13_sc_7.b`*

> [!question] Inferred | Work backwards from a file size to find the bit depth [3]
> A bitmap image of 800 × 600 pixels has a file size of 1.44 MB. Calculate the bit depth used. Show your working.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Total pixels = 800 × 600 = **480 000**
>> - File size in bits = 1.44 × 1 000 000 × 8 = **11 520 000 bits**
>> - Bit depth = 11 520 000 ÷ 480 000 = **24 bits**
>> - … which is **true colour**, 2²⁴ = 16 777 216 colours
>> - The same formula rearranged — and the same marking structure, working then answer
>>
>> *Inference: every 9618 question gives resolution and depth and asks for the size. The inverse — find the depth, or find how many images fit in a given capacity — has never been set, though it is the standard way to raise difficulty.*

> [!question] SME | Calculate the file size of a sound recording [2]
> An audio message is recorded with a sampling rate of 50 kHz and a sampling resolution of 16 bits. The recording is 20 minutes long. Calculate the file size in megabytes. Show your working.
>
>> [!success]- Answer — 1 mark for the answer, 1 for the working
>> - **Formula:** sampling rate × sampling resolution × duration in **seconds**
>> - **Working:** 50 000 × (20 × 60) × 16 bits
>> - = 50 000 × 1200 × 16 = **960 000 000 bits**
>> - = 120 000 000 bytes = 120 000 kilobytes = **120 megabytes**
>> - Convert the duration to **seconds** first — minutes is the usual trap
>>
>> *Latest: `9618_w22_qp_13_sc_1.b`. Filed under Data Representation in the Legend, not Multimedia, but it is the same discipline as the bitmap formula.*

---

## 1.2.3 Effects of changing bitmap elements

> [!question] 9618 | Explain the effect of decreasing the bit depth on the image and on the file [4]
> A second photograph is taken with a lower bit depth. Explain the effect of decreasing the bit depth on the image and on the image file.
>
>> [!success]- Answer — 1 mark each, two per half, 4 marks
>> - **Image:** there will be **fewer shades of colour available**
>> - … so the image **does not match the original**, as **detail is lost**
>> - **Image file:** **fewer bits are used to store each pixel**
>> - … so **less data is stored**, therefore the **file size is reduced**
>> - Two marks are reserved for each half — four points about the image alone scores 2
>>
>> *Latest: `9618_s25_qp_13_sc_1.a.ii`*

> [!question] 9618 | State what is meant by bit depth and explain how changing it affects the image [3]
> State what is meant by the **bit depth** of a bitmap image **and** explain how changing the bit depth affects the image.
>
>> [!success]- Answer — 1 mark for the definition + 1 per explanation bullet
>> - **Definition:** the number of bits used to represent **each colour**
>> - **Explanation:** an increase means the image has a **greater range of colours** // a decrease means a smaller range
>> - **Explanation:** an increase makes the image **closer to the original / more realistic** // a decrease makes it less like the original / less realistic
>>
>> *Latest: `9618_w23_qp_11_sc_1.b`*

> [!question] 9618 | Explain why changing the image resolution affects quality and file size [2]
> Explain why changing the image resolution will affect the image quality and the file size.
>
>> [!success]- Answer — 1 mark for each correct explanation
>> - **Image quality:** decreasing the resolution means **details are lost because there are fewer pixels**
>> - … // increasing means the image is **more detailed because there are more pixels**
>> - **File size:** decreasing the resolution **decreases** the file size **because there are fewer pixels therefore less data**
>> - … // increasing **increases** it because there are more pixels therefore more data
>> - Each half must carry its **because** — the bare statement scores nothing
>>
>> *Latest: `9618_w24_qp_12_sc_7.a.ii`*

> [!question] 9618 | Describe the impact of increasing the image resolution on quality [2]
> Describe the impact of increasing the image resolution on the quality of a bitmap graphic.
>
>> [!success]- Answer — 1 mark for each bullet
>> - **More pixels can be stored / are available**
>> - The image is **sharper / less pixelated**
>>
>> *Latest: `9618_w23_qp_13_sc_2.a`*

> [!question] 9618 | Identify two elements that can be changed to reduce file size [2]
> Identify **two** elements of a bitmap image that can be changed to reduce its file size.
>
>> [!success]- Answer — 1 mark each to max 2
>> - **Colour / bit depth**
>> - **Image resolution**
>> - Only these two are credited — offering compression or screen resolution scores nothing
>> - Related: one drawback of **increasing** the bits per pixel is simply **increased file size** (`w24_qp_13_sc_6.b.ii`)
>>
>> *Latest: `9618_s24_qp_13_sc_2.c`*

> [!question] 9618 | Tick the effect of each action on the file size [2]
> Tick one box in each row to identify the effect of each action on the image file size.
>
>> [!success]- Answer — 1 mark for one or two correct rows, 2 marks for all three
>> - Change the colour depth to 16 bits per pixel (from 24) → **decreases the file size**
>> - Change the **screen** resolution to 1366 × 768 → **no change to the file size**
>> - Change the colour of the rectangle from black to red → **no change to the file size**
>> - **Screen resolution is a property of the display**, not the file
>> - **Changing which colour is used** does not change how many bits store it
>>
>> *Latest: `9618_w22_qp_12_sc_8.a`*

> [!question] Inferred | Recommend a resolution and bit depth for a stated purpose, and justify [4]
> A company needs images for a website that must load quickly on mobile connections. Recommend a suitable image resolution and bit depth, and justify your choices.
>
>> [!success]- Answer — 2 marks per choice (recommendation + justification), 4 marks
>> - A **lower image resolution**, matched to the size the image is displayed at
>> - … because extra pixels beyond the display size add file size without visible benefit, and a smaller file **loads faster over a mobile connection**
>> - A **moderate bit depth** (e.g. 24-bit for photographs, 8-bit for simple graphics)
>> - … because photographs need a wide range of colours to look realistic, but a logo or icon with few colours needs far fewer bits per pixel
>> - The justification must be tied to the **stated purpose** — generic "smaller is better" scores nothing
>>
>> *Inference: every question asks what happens when a value changes; none asks the candidate to **recommend and justify** — the format used constantly for storage devices in Chapter 3, and already used in 1.2.5 for bitmap vs vector.*

---

## 1.2.4 How vector graphic data is encoded

> [!question] 9618 | Define the vector graphic terms [3]
> Complete the table by defining the vector graphic terms: drawing list, drawing object, property.
>
>> [!success]- Answer — 1 mark for each correct definition
>> - **Drawing list** — **all the drawing objects in an image** // a list that stores the **commands / descriptions / mathematical equations** required to draw each object
>> - **Drawing object** — a **component created using a formula**
>> - **Property** — an **attribute of a drawing object** // data about a shape // **defines one aspect of the appearance** of a drawing object
>>
>> *Latest: `9618_w24_qp_12_sc_7.b` (also `w23_qp_11_sc_1.a`, `s23_qp_11_sc_1.a`)*

> [!question] 9618 | Describe the contents of a vector graphic drawing list [2]
> Describe the contents of a vector graphic drawing list.
>
>> [!success]- Answer — 1 mark each to max 2
>> - A **list of the objects** in the drawing
>> - A list that stores the **command / description / equation required to draw each object**
>> - The **properties of each object**, e.g. the fill colour, the line weight or colour
>>
>> *Latest: `9618_s24_qp_12_sc_2.d.ii`*

> [!question] 9618 | Describe each vector term and give an example from a given logo [4]
> Complete the table by writing a description of each vector graphic term **and** giving an example for the logo shown.
>
>> [!success]- Answer — 1 mark for each description, 1 for each valid example
>> - **Property** — data about the shapes // defines one aspect of the appearance of the drawing object
>> - … *example:* black line // white fill // black fill // solid line // font of the letter // colour of the triangle
>> - **Drawing list** — the list of shapes involved in an image // a list that stores the command or description required to draw each object
>> - … *example:* triangle // capital letter R // rectangle // line
>> - The example must be **read off the image given** — a generic example scores nothing
>>
>> *Latest: `9618_w21_qp_12_sc_5.a`*

> [!question] 9618 | Match each vector graphic term to its description [2]
> Draw one line from each vector graphic term to its most appropriate description.
>
>> [!success]- Answer — 2 marks for all 3 correct, 1 mark for 1 correct
>> - **Drawing list** → data required to create all components in the graphic
>> - **Drawing object** → a component created using a formula
>> - **Property** → defines one characteristic of a component
>> - The lines **cross** — the terms are not listed in the same order as the descriptions
>>
>> *Latest: `9618_w23_qp_11_sc_1.a`*

> [!question] Inferred | Explain why a vector graphic can be enlarged without loss of quality [3]
> Explain why a vector graphic can be enlarged without any loss of quality, whereas a bitmap image cannot.
>
>> [!success]- Answer — 5 points for 3 marks
>> - A vector file stores **mathematical equations and coordinates**, not pixels
>> - … so when the image is enlarged the shapes are **recalculated at the new size**
>> - … and the lines are redrawn at full sharpness, so **no detail is invented or lost**
>> - A bitmap stores a **fixed grid of pixels**, so enlarging makes **each pixel bigger**
>> - … which is why the image **pixelates** — the detail was never in the file to begin with
>>
>> *Inference: credited as a bare point inside the comparison questions ("recalculated and does not pixelate"), but the mechanism has never been the subject of its own question.*

> [!question] SME | Describe what is stored in a vector graphic file [3]
> Describe what is stored in a vector graphic file.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Only the **mathematical equations and points** needed to create the image
>> - … e.g. for a circle, the **centre point (x, y) and the radius** — nothing else
>> - A **drawing list**, held in the **file header**
>> - … containing the **commands** to create each object, the **properties** of each object, and the **relative position** of each object
>> - **No dimensions are defined**, which is why scaling up causes no loss of quality
>>
>> *The **relative position** point is SME-only — 9618 credits commands and properties repeatedly but never mentions position, even though it is what makes a drawing list reproducible.*

---

## 1.2.5 Justifying bitmap or vector

> [!question] 9618 | Describe two differences between a vector graphic and a bitmap image [4]
> Describe **two** differences between a vector graphic and a bitmap image.
>
>> [!success]- Answer — 1 mark per bullet to **max 2 for each difference**
>> - **Composition:** a bitmap is made up of **pixels** // colours stored for individual pixels
>> - … a vector graphic stores a **set of instructions** about how to draw the shape
>> - **Scaling:** when a bitmap is enlarged **the pixels get bigger and it pixelates**
>> - … when a vector is enlarged it is **recalculated and does not pixelate**
>> - **File size:** bitmap files are usually **bigger**, because of the need to store data about **each pixel**
>> - … vector graphics have a **smaller file size** because they contain just the instructions
>> - **Compression:** bitmaps **compress well**, with significant reduction in file size; vector graphics **do not compress well, because there is little redundant data**
>>
>> *Latest: `9618_w21_qp_12_sc_5.b.i`*

> [!question] 9618 | State two benefits of creating a vector graphic instead of a bitmap image [2]
> State **two** benefits of creating a vector graphic instead of a bitmap image.
>
>> [!success]- Answer — 1 mark each to max 2
>> - Can be **enlarged without pixelation / loss of quality**
>> - **Individual components** of the image can be edited
>> - Generally a **smaller file size**
>>
>> *Latest: `9618_w22_qp_12_sc_8.b`. The **only** 9618 question under this bullet.*

> [!question] 9608 | Describe two drawbacks of using a bitmap for a logo instead of a vector [4]
> Describe **two** drawbacks of using a bitmapped image for a logo instead of a vector graphic.
>
>> [!success]- Answer — 1 mark per drawback, 1 for its expansion, max 2 each
>> - A bitmap file is likely to take up **more storage space**
>> - … because the **colour of each pixel** needs to be stored
>> - A bitmap **cannot be enlarged** // is difficult to use in different types of document
>> - … **without the image pixelating**
>> - A bitmap would be **more difficult to edit**
>> - … because **each pixel would need to be edited separately**
>> - The **editability** drawback appears in no 9618 mark scheme
>>
>> *Latest: `9608_s21_qp_11_sc_2.c`*

> [!question] 9608 | Describe two reasons why a vector graphic suits a logo [4]
> A company has created a logo for its website as a vector graphic. Describe **two** reasons why a vector graphic is a sensible choice for the logo.
>
>> [!success]- Answer — 1 mark per bullet, max 2 per reason
>> - **Smaller file size**
>> - … so it can be **transferred / downloaded more quickly**
>> - **Enlarges without pixelation**
>> - … because it needs to be used on **different screens / devices / resolutions**
>> - Also credited: it needs to be **large for signs** without pixelating · a smaller file size **reduces storage** when the logo is stored on many documents
>>
>> *Latest: `9608_w18_qp_12_sc_1.c` (also `s18_qp_11_sc_2.d`, `s20_qp_13_sc_7.c`, `s20_qp_12_sc_1.b.ii`)*

> [!question] Inferred | Justify the use of a bitmap image rather than a vector graphic [4]
> A wildlife photographer stores photographs on a website. Justify the use of bitmap images rather than vector graphics.
>
>> [!success]- Answer — 2 points + expansions, 4 marks
>> - A photograph has **continuous tone and millions of subtly different colours**
>> - … which cannot be described as a set of shapes and equations, so a vector graphic could not reproduce it
>> - A photograph has **no discrete objects** to store in a drawing list
>> - … every pixel is independent, which is exactly what a bitmap stores
>> - A camera sensor **produces pixel data directly**, so a bitmap needs no conversion
>> - Bitmaps also **compress well** (lossy, e.g. JPEG), so the large file size is manageable
>>
>> *Inference: every question in both series runs the argument one way — why vector beats bitmap for a **logo**. The reverse is half of what the bullet says and has never been asked.*

> [!question] SME | State the questions that decide between bitmap and vector [3]
> State three questions that should be considered when choosing between a bitmap image and a vector graphic.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Does the image need to be resized?** — if yes, vector
>> - **Does the image need to be drawn to scale?** — if yes, vector
>> - **Does the image need to look real?** — if yes, bitmap
>> - Vector suits **logos, icons and text graphics**; bitmap suits **photographs and detailed images**
>> - File types: vector `.svg`, `.ai`, `.eps` · bitmap `.jpg`, `.png`, `.bmp`, `.gif`
>>
>> *SME's decision framework; 9618 marks justification questions at up to 2 and 9608 at up to 4.*

---

## 1.2.6 How sound is represented and encoded

> [!question] 9618 | Describe how sound is represented in a computer [3]
> Describe how sound is represented in a computer.
>
>> [!success]- Answer — 1 mark each
>> - The **amplitude is recorded a set number of times a second**
>> - Each instance of an amplitude is given a **corresponding binary number**
>> - The binary number of each amplitude is **saved in sequence**
>> - Same three-part shape as the bitmap and character-set answers
>>
>> *Latest: `9618_s23_qp_13_sc_3.c.i`*

> [!question] 9618 | Explain how an analogue sound wave is converted into digital data [2]
> Explain how an analogue sound wave is converted into digital data.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - The **value / magnitude / size of the analogue sound wave is measured** a set number of times each second / at set intervals
>> - Each **sample / reading / measurement is given a binary number and stored in sequence**
>>
>> *Latest: `9618_w24_qp_13_sc_6.c.i`*

> [!question] 9618 | Complete the table of sound terms [3]
> Complete the table by giving the term for each description about sound representation.
>
>> [!success]- Answer — 1 mark for each correct term
>> - The number of times the amplitude is measured per time interval → **sampling rate**
>> - The number of bits used to store each amplitude measurement → **sampling resolution**
>> - The type of sound wave before it is recorded by a computer → **analogue**
>>
>> *Latest: `9618_s25_qp_13_sc_1.b`*

> [!question] 9618 | Match the sound terms to their descriptions [2]
> Draw one line from each term to its most appropriate description: sampling, sampling rate, sampling resolution.
>
>> [!success]- Answer — 1 mark for 1 correct line, 2 marks for all 3
>> - **Sampling** → taking measurements at regular intervals and storing the values
>> - **Sampling rate** → the number of samples taken per second
>> - **Sampling resolution** → the number of bits used to store each sample
>> - The lines **cross** — sampling is not the first description
>>
>> *Latest: `9618_w23_qp_13_sc_1.b`*

> [!question] 9618 | State what is meant by sampling rate, and by analogue data [2]
> (i) State what is meant by **sampling rate**. (ii) State what is meant by **analogue data**.
>
>> [!success]- Answer — 1 mark each
>> - **Sampling rate** — the number of samples taken **per unit time / per second**
>> - **Analogue data** — data values that are **continuously changing** // variable // can take **any** value
>> - … as opposed to digital data, which takes only discrete values
>>
>> *Latest: `9618_w22_qp_11_sc_1.d.i` and `9618_w23_qp_13_sc_1.a`*

> [!question] 9608 | Define sampling, sampling rate and sampling resolution [3]
> Complete the table by writing the definitions for each term: sampling, sampling resolution, sampling rate.
>
>> [!success]- Answer — 1 mark per correct definition
>> - **Sampling** — measuring the **amplitude of the wave at regular / set time intervals**
>> - **Sampling resolution** — the number of bits used to represent **each sample**
>> - **Sampling rate** — the number of samples taken **per unit of time**
>> - 9618 asks these as a **matching** exercise; 9608 requires them **written out**
>>
>> *Latest: `9608_w21_qp_11_sc_2.a` (also `s20_qp_12_sc_2.a`)*

> [!question] 9608 | State what is meant by a given sampling rate and resolution [2]
> A sound track has a sampling rate of 88.2 kHz and a sampling resolution of 32 bits. State what each of these means.
>
>> [!success]- Answer — 1 mark per bullet
>> - **88.2 kHz** — the sound wave is sampled **88 200 times per second**
>> - **32 bits** — each sample is stored as a **32-bit binary number**
>> - Reading the units off an actual specification is never asked in 9618
>>
>> *Latest: `9608_s19_qp_13_sc_5.c`*

> [!question] 9608 | Describe how images and sound are encoded into digital form [4]
> A video is made of a sequence of images and a sound file. Describe how the images and the sound are encoded into digital form.
>
>> [!success]- Answer — 1 mark per bullet, max 4; **max 3 for image, max 3 for sound**
>> - **Images:** stored as **bitmaps**; each image is **made up of pixels**
>> - … each pixel is a **single colour**, and each colour has a **unique binary number**
>> - … **store the sequence of binary numbers** for each image / frame
>> - **Sound:** measure the **height / amplitude** of the sound wave
>> - … a **set number of times per second** / at **regular** time intervals
>> - … each amplitude has a **unique binary number**, and the sequence of numbers is **stored**
>> - One question covering **both** encodings, which 9618 has never set
>>
>> *Latest: `9608_w19_qp_12_sc_6.d.i`*

> [!question] 9608 | Describe two features of sound editing software [4]
> Describe **two** features of sound editing software that can be used to edit a sound file.
>
>> [!success]- Answer — 1 mark for naming, 1 for describing, max 2 per feature
>> - **Cut / delete** — remove part of the sound file, e.g. background noise
>> - **Copy and paste** — replicate part of the sound
>> - **Amplify** — increase the volume of a section of sound
>> - **Fading** — change the volume of a section so it gets louder or quieter
>> - **Change pitch** — increase or decrease the frequency of a section
>> - **Change sampling resolution** — to change the accuracy of the sound or the file size
>> - Sound **editing** appears nowhere in the 9618 syllabus notes — background, not a likely question
>>
>> *Latest: `9608_w18_qp_11_sc_1.c` (also `s18_qp_12_sc_5.d`, `w19_qp_13_sc_2.b.iii`)*

> [!question] Inferred | Explain how a stored sound file is played back [3]
> Explain how a sound file stored in binary is played back through a speaker.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The stored **binary values are read back in sequence**, at the same rate they were sampled
>> - Each value is converted into a **voltage** by a **digital-to-analogue converter (DAC)**
>> - … reconstructing an **approximation of the original analogue waveform**
>> - The varying voltage drives the **speaker cone**, which vibrates
>> - … producing **sound waves** in the air
>> - The reconstruction is only an approximation — **quantisation errors** from recording remain
>>
>> *Inference: every question describes **recording**. The reverse path is never asked, though SME describes it and the speaker is in the Chapter 3 syllabus.*

---

## 1.2.7 Impact of changing sampling rate and resolution

> [!question] 9618 | Explain why increasing the sampling rate and resolution improves precision [4]
> Explain the reasons why increasing the sampling rate and the sampling resolution will improve the precision of a recording.
>
>> [!success]- Answer — 1 mark each; **max 2 for rate, max 2 for resolution**
>> - **Sampling rate:** there are **smaller 'gaps' in the sound wave** // sound is recorded **more often**
>> - … the **digital waveform is closer to the analogue waveform**
>> - … the **quantisation errors are smaller**
>> - **Sampling resolution:** there are **more bits per sample** // a wider range of amplitudes can be stored
>> - … each **binary amplitude is closer to the analogue amplitude**
>> - … the digital waveform is closer to the analogue waveform, and quantisation errors are smaller
>> - Four points about the rate alone caps at 2
>>
>> *Latest: `9618_s23_qp_13_sc_3.c.ii`*

> [!question] 9618 | Explain the impact of changing the sampling resolution on accuracy [3]
> Explain the impact of changing the sampling resolution on the accuracy of a sound recording.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - **Increasing:** the number of bits used for each sample is **increased**
>> - … there will be **more values available** to represent each sample // more amplitudes can be represented
>> - … each binary amplitude in the digital recording is **closer to the analogue amplitude**
>> - … **quantisation errors are reduced**
>> - … the digital soundwave is **closer to the original analogue soundwave**
>> - **Decreasing:** the exact mirror of each point above
>>
>> *Latest: `9618_w23_qp_12_sc_6.b`*

> [!question] 9618 | Explain the effect of increasing the sampling rate on accuracy [2]
> Explain the effect of increasing the sampling rate on the accuracy of a sound recording.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - It **improves** the accuracy of the sound file
>> - … because the **digital waveform more closely resembles the analogue waveform**
>> - **Quantisation errors are reduced**
>> - It increases the **amount of detail stored**
>>
>> *Latest: `9618_w22_qp_12_sc_6.b.i`*

> [!question] 9618 | Explain the effect of changing the sampling resolution on the file [2]
> (i) Explain the effect of increasing the sampling resolution on the sound file. (ii) Explain the effect of decreasing the sampling resolution on the file size.
>
>> [!success]- Answer — 1 mark per bullet, max 2 each
>> - **Increasing:** increases the **number of bits per sample** // a larger range of values
>> - … which means the **file size increases**
>> - … makes the sound file **more accurate** // digital waveform closer to the original
>> - … **smaller quantisation errors**
>> - **Decreasing:** **decreases the file size** of the sound file
>> - … because **fewer bits are used to store each sample**
>>
>> *Latest: `9618_w22_qp_11_sc_1.d.ii` and `9618_w22_qp_12_sc_6.b.ii`*

> [!question] 9618 | Describe why a higher sample rate sounds closer to the original, and increases file size [4]
> (i) Describe the reasons why the sound is closer to the original when a higher sample rate is used. (ii) Describe the reasons why the file size increases when a higher sample rate is used.
>
>> [!success]- Answer — 1 mark per bullet, 2 marks each part
>> - **(i)** **Smaller time gaps** between the samples
>> - … makes the **digital** sound wave more accurate
>> - … **smaller quantisation errors**
>> - **(ii)** **More samples / data are taken or recorded**
>> - … so **more bits are stored altogether**
>>
>> *Latest: `9618_w21_qp_11_sc_7.a.i` and `a.ii`*

> [!question] 9618 | Draw lines from each change to its impacts on a sound file [3]
> Draw **two** lines from each change to the impacts it has on the sound file.
>
>> [!success]- Answer — 1 mark per correctly connected change box, max 3
>> - Increase the **duration** → the file size gets **bigger** · **no change** to the accuracy
>> - Increase the **sampling rate** → the file size gets **bigger** · the accuracy **improves**
>> - Decrease the **sampling resolution** → the file size gets **smaller** · the accuracy **worsens**
>> - Each change box needs **two** lines — one for size, one for accuracy
>>
>> *Latest: `9618_w25_qp_13_sc_1.a`*

> [!question] 9618 | Tick the effect of each action on the accuracy of a recording [2]
> Tick one box in each row to identify the effect of each action on the accuracy of the recording.
>
>> [!success]- Answer — 1 mark for 1–2 correct, 2 marks for all 3
>> - Change the sampling rate from 40 kHz to 60 kHz → accuracy **increases**
>> - Change the duration from 20 minutes to 40 minutes → accuracy **does not change**
>> - Change the sampling resolution from 24 bits to 16 bits → accuracy **decreases**
>> - The duration row is the trap: **a longer recording is bigger, not more accurate**
>>
>> *Latest: `9618_w22_qp_13_sc_1.a`*

> [!question] 9618 | Describe how a change in sampling rate affects a device's performance [3]
> The user changes the sampling rate the microphone uses from 44.1 kHz to 88.2 kHz. Describe how this change will affect the performance of the video doorbell.
>
>> [!success]- Answer — 1 mark each to max 3
>> - **Data transmission** to the user's smartphone will **take longer**
>> - … because there is **more data to transmit**
>> - The **secondary storage device will fill faster**
>> - … so **fewer videos can be stored long-term** // videos are **overwritten more often**
>> - This is the applied, **consequences** version of the bullet — the answer must be about the device, not about waveforms
>>
>> *Latest: `9618_s24_qp_11_sc_2.d`*

> [!question] 9608 | Define sampling rate and explain its influence on accuracy [2]
> Define the term **sampling rate**. Explain how the sampling rate will influence the accuracy of the digitised sound.
>
>> [!success]- Answer — 1 mark for the definition, 1 for the explanation
>> - **Definition:** the number of samples taken **per unit time** // the number of times the amplitude is measured per unit time
>> - **Explanation:** increasing the sampling rate will **increase the accuracy / precision** of the digitised sound
>> - … // increasing the sampling rate will result in **smaller quantisation errors**
>> - 9618 asks the definition and the effect in **separate** questions; 9608 combines them
>>
>> *Latest: `9608_s17_qp_13_sc_3.a` (also `s17_qp_11_sc_3.a`)*

> [!question] 9608 | Define sampling resolution and explain its effect on accuracy [3]
> Define the term **sampling resolution**. Explain how the sampling resolution will affect the accuracy of the digitised sound.
>
>> [!success]- Answer — max 2 for the definition, max 2 for the explanation, 3 marks
>> - **Definition:** the number of **distinct values available** to encode / represent each sample
>> - … specified by the **number of bits** used to encode the data for one sample
>> - … sometimes referred to as **bit depth**
>> - **Explanation:** a larger resolution means there are **more values available** to store each sample
>> - … it will **improve the accuracy** of the digitised sound // **decrease the distortion** of the sound
>> - … increased sampling resolution means a **smaller quantisation error**
>> - Two pieces of vocabulary are 9608-only: **"distinct values available"** and **"distortion"**
>>
>> *Latest: `9608_s17_qp_12_sc_3.a`*

> [!question] Inferred | Explain what is meant by a quantisation error [3]
> Explain what is meant by a quantisation error in a digital sound recording.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The sampling resolution gives only a **fixed number of possible values** (2ⁿ for n bits)
>> - The true amplitude of the wave at the moment of sampling usually falls **between two of those values**
>> - … so it must be **rounded to the nearest available value**
>> - The **difference between the true amplitude and the stored value** is the quantisation error
>> - **Increasing the sampling resolution reduces it**, because the available values are closer together
>>
>> *Inference: "quantisation errors" is a credited mark point in **six separate 9618 mark schemes** — the most-credited term in 1.2.7 — yet **no question in either series asks what one is**.*

> [!question] SME | State the impact of each sampling setting on quality and file size [3]
> State the effect of increasing the sampling rate, the sampling resolution and the duration on playback quality and file size.
>
>> [!success]- Answer — 1 mark per row, 3 marks
>> - **Sampling rate ↑** → more detail, **better sound quality** · more data, **larger file size**
>> - **Sampling resolution ↑** → bigger range of amplitudes, **better sound quality** · more data per sample, **larger file size**
>> - **Duration ↑** → **larger file size**, but **no change to accuracy**
>> - For reference, a typical audio CD: sampling rate **44.1 kHz**, sampling resolution **16 bits**, recorded in stereo
>>
>> *SME's table; 9618's own tick-table question (`w22_qp_13_sc_1.a`) marks exactly these three rows.*

---

# 1.3 Compression

## 1.3.1 The need for compression

> [!question] 9618 | Explain why a video is compressed before real-time bit streaming [4]
> Explain the reasons why a video is compressed before it is transmitted using real-time bit streaming.
>
>> [!success]- Answer — 1 mark each to max 4
>> - Video is **data-intensive**
>> - The file size needs reducing in order to **reduce the amount of bandwidth used**
>> - … and to **reduce buffering**
>> - This means people are **not behind in the conversation**
>> - … and people with **lower bandwidth can still take part**
>> - The highest-tariff compression question in the chapter, and the one most tied to Topic 2
>>
>> *Latest: `9618_s25_qp_11_sc_2.b.i`*

> [!question] 9618 | Explain the benefits of a compressed email attachment [3]
> Explain the benefits to the recipient of an email attachment being a compressed file.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - **Less of the recipient's storage space** is used
>> - … so more work can be stored
>> - **Transmission time is reduced**
>> - … so the recipient does not have to wait as long for it to arrive
>> - **Bandwidth usage is reduced**
>> - … so other transmissions are not adversely affected
>> - **Less data allowance** is used on the email system
>> - Each benefit has its own **consequence**, and the consequence is a separate mark
>>
>> *Latest: `9618_w24_qp_11_sc_4.b.i`*

> [!question] 9618 | Explain why a bitmap image is compressed before being emailed [2]
> Explain why a bitmap image is often compressed before it is attached to an email.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - **Reduced bandwidth usage** when transmitting the message
>> - **Reduced transmission time** from email client to email server
>> - **Reduced storage space on the email**
>> - **Email accounts often have a maximum size for an attachment**
>> - That last point is specific to email and is easily missed
>>
>> *Latest: `9618_w23_qp_11_sc_1.c`*

> [!question] 9618 | Explain why compressing files benefits the customers who download them [3]
> Photographs are compressed before being uploaded to a web server. Explain the reasons why compressing the photographs will benefit the customers.
>
>> [!success]- Answer — 1 mark each, max 3
>> - The customers will be able to **download the photographs in less time**
>> - … and they will take **less of the customer's bandwidth**
>> - The photographs will take up **less space on the customer's storage medium**
>> - … therefore the customers can **store more images**
>> - … and will have **more space for other files**
>> - Every point must be framed from the **customer's** side, not the server's
>>
>> *Latest: `9618_s23_qp_11_sc_1.c.i`*

> [!question] 9618 | Explain the reasons for compressing files on a web server [2]
> A program is distributed by downloading its files from a web server. Explain the reasons for compressing the files.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - To reduce the **time it takes to download** the files from the web server
>> - … // to **upload** them to the server in the first place
>> - To reduce the amount of **storage space used on the web server** // on the user's device
>> - Related: compressing a sound file before emailing it — **reduces the file size** · **faster to transmit / download** · the **original file is too large** for email storage (`w21_qp_11_sc_7.b.i`)
>>
>> *Latest: `9618_w23_qp_13_sc_5.b.i`*

> [!question] 9618 | Give two reasons why a video does not need to be compressed [2]
> The bitmap video is **not** compressed before transmission to the VR headset. Give **two** reasons why the video does not need to be compressed.
>
>> [!success]- Answer — 1 mark each to max 2
>> - A **dedicated connection** to the headset // not sharing bandwidth
>> - An **already fast connection** that can transmit the data without slowing
>> - The video **may already be a small file size** and does not need further reduction
>> - The video is **not saved**, so **storage is not an issue** in the headset
>> - The inverted question — the marks are for reasons compression is **unnecessary**, not for its drawbacks
>>
>> *Latest: `9618_s24_qp_12_sc_2.d.iii`*

> [!question] Inferred | State the drawbacks of compressing a file [3]
> State three drawbacks of compressing a file.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Compression and decompression take **processing time**
>> - … so there is a delay before the file can be used, and extra CPU load on both devices
>> - **Lossy compression permanently destroys data**, so the original cannot be recovered
>> - … and repeatedly compressing the same file degrades it further each time
>> - An **already-compressed file cannot usefully be compressed again** — the redundancy has gone
>>
>> *Inference: every question in both series asks for the **benefits**. The costs are never asked — the closest is "why does this video not need compressing", which is argued from bandwidth rather than from the cost of compressing.*

> [!question] SME | Name three compression formats and state what each does [3]
> Name three common compression formats and describe briefly how each reduces file size.
>
>> [!success]- Answer — 1 mark per format with its method, 3 marks
>> - **MP3** — audio; reduces a file by up to **90%** using **perceptual music shaping**, removing frequencies outside human hearing and quieter sounds **masked** by louder ones; **lossy**
>> - **MP4** — multimedia (audio, video, photos, animations); the standard for streaming, keeping file size small without noticeable loss
>> - **JPEG** — the standard **lossy** bitmap format; it **creates a new file**, so the original can no longer be used
>> - **SVG** — vector files are **XML text**, which is why they can be compressed at all (as `.svgz`)
>>
>> *Named formats are not required by the syllabus, but they are the obvious "give an example" answers.*

---

## 1.3.2 Lossy and lossless, and justifying a method

> [!question] 9618 | State whether a described method is lossy or lossless, and justify [1]
> A sound file is compressed by reducing the sampling rate. State whether this is lossless or lossy compression. Justify your choice.
>
>> [!success]- Answer — 1 mark for the correct answer **with** justification
>> - Type of compression: **lossy**
>> - Justification: there will be **fewer samples per second, so data will be permanently lost**
>> - … // there will be fewer samples per second, so the **original sound cannot be re-created**
>> - The **justification carries the mark** — the label alone scores nothing
>>
>> *Latest: `9618_w25_qp_12_sc_6.a`*

> [!question] 9618 | Identify the appropriate compression method for real-time streaming, and justify [3]
> Identify whether the lossy or lossless compression method is more appropriate for real-time bit streaming. Justify your answer.
>
>> [!success]- Answer — **no mark for the choice**; 1 mark each to max 3
>> - (**Lossy** is the expected answer)
>> - **Reduces file size more than lossless**
>> - … so **significantly less bandwidth / data** is needed
>> - … so **buffering is reduced even more than with lossless**
>> - **Data can be removed which cannot be seen**
>> - … reducing quality **without impacting the experience**
>> - … for example, the **resolution of the video** can be reduced // the **sample rate of the audio** can be reduced
>>
>> *Latest: `9618_s25_qp_11_sc_2.b.ii`. Ticking the box and writing nothing scores **zero**.*

> [!question] 9618 | Tick the appropriate compression type for a scenario, and justify [3]
> A real-time video of a music concert needs to be streamed to subscribers. Tick one box to identify the most appropriate type of compression **and** justify your answer.
>
>> [!success]- Answer — 1 mark per bullet, max 3; **both choices credited if justified**
>> - **Lossy (ticked):** loss of quality **will not be noticed**
>> - … needs to be viewed in **real time**, so less bandwidth is needed if the file size is smaller
>> - … smaller file sizes **reduce buffering**, so the video plays more smoothly
>> - … viewers may watch on **different devices**, so may not need high quality resolution
>> - **Lossless (ticked):** the original recording **may not have been made in high resolution**
>> - … could be streaming to **high bandwidth** devices
>> - … the reduction in file size is **sufficient** for the receiving device // viewers **do not want any loss of quality**
>> - Unusually, **either tick can score full marks** — the justification decides it
>>
>> *Latest: `9618_w23_qp_12_sc_6.a`*

> [!question] 9618 | Explain why lossy compression is suitable for a bitmap image [2]
> A bitmap image can be compressed using lossy compression. Explain the reasons why lossy compression is often suitable for a bitmap image.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - The change **may not be noticeable** // data removed is usually **not noticed by the human eye**
>> - … for example, changes in **shade or detail**
>> - It produces a **larger decrease in file size** compared to lossless // lossy decreases file size considerably
>>
>> *Latest: `9618_w24_qp_13_sc_6.b.iii`*

> [!question] 9618 | Give three benefits of lossy instead of lossless for a photograph [3]
> Give **three** benefits of a photograph being compressed using lossy compression instead of lossless compression.
>
>> [!success]- Answer — 1 mark each to max 3 — **every point must be comparative**
>> - The file takes **less storage space on the web server** than if lossless was used
>> - The file is **faster to upload / download** to and from the server than if lossless was used
>> - The file uses **less bandwidth** to transmit than if lossless was used
>> - The file **consumes less data allowance** than if lossless was used
>> - Dropping "than if lossless was used" turns each point into a generic benefit of compression and loses the mark
>>
>> *Latest: `9618_s24_qp_13_sc_2.b.i`*

> [!question] 9618 | Explain why lossless is more appropriate than lossy for a text file [2]
> RLE is an example of lossless compression. Explain why lossless compression is more appropriate than lossy compression for a text file.
>
>> [!success]- Answer — 1 mark for each bullet
>> - **All the data is required** // **no data can be lost**
>> - … otherwise the text file will be **corrupted / not make sense**
>>
>> *Latest: `9618_w22_qp_12_sc_8.c.ii`*

> [!question] Inferred | Define lossy and lossless compression [2]
> Define what is meant by lossy compression and by lossless compression.
>
>> [!success]- Answer — 1 mark each
>> - **Lossy** — data is **permanently removed** to reduce the file size; the process is **irreversible**, so the original file **cannot be recovered**
>> - **Lossless** — the data is **encoded** rather than discarded, by finding patterns and repetition; the process is **reversible**, so the file can be **restored exactly** to its original state
>> - Lossy achieves a much greater reduction; lossless a smaller one
>>
>> *Inference: both terms are used in every question in this sub-topic, and **neither has ever been asked for as a definition** in 9618.*

> [!question] Inferred | Justify using lossless compression for a sound file [3]
> A recording studio archives master audio recordings. Identify the more appropriate compression method and justify your answer.
>
>> [!success]- Answer — 5 points for 3 marks (lossless)
>> - The recording is a **master that will be edited further**
>> - … and each lossy compression would **permanently remove data**, degrading it with every save
>> - **No loss of quality is acceptable** in a professional recording
>> - … and lossless is **reversible**, so the exact original waveform can be restored
>> - Storage is **not the constraint** here — the archive is not being streamed in real time
>>
>> *Inference: the justification questions cover lossy for video, lossy for photographs and lossless for text. **Lossless for audio** — the fourth combination — is never set, despite sound being examined heavily elsewhere in the topic.*

> [!question] SME | Describe how lossy and lossless compression work in practice [4]
> Describe how lossy compression works on a photograph and how lossless compression works on a document.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Lossy on a photograph:** groups **similar colours together**
>> - … reducing the number of colours in the image **without compromising the overall quality**
>> - … the data removed is **permanently lost**, but the difference is hard to see
>> - **Lossless on a document:** uses algorithms to **analyse the contents for patterns and repetition**
>> - … encoding those repetitions more compactly rather than discarding anything
>> - … opening the file **reverses the algorithm** and returns the data to its original state
>> - Lossless is applied **automatically** to formats such as DOCX and PDF
>>
>> *SME's worked explanation; 9618 marks "describe a method" questions at 2–4.*

---

## 1.3.3 How text, bitmap, vector and sound files are compressed

> [!question] 9618 | Identify one lossless method of compressing an image [1]
> Identify **one** lossless method of compressing an image.
>
>> [!success]- Answer — 1 mark
>> - **Run-Length Encoding (RLE)**
>>
>> *Latest: `9618_w24_qp_12_sc_7.a.iii`*

> [!question] 9618 | Identify a lossless method and describe how it reduces the file size [3]
> Identify **one** method of lossless compression that can be used to compress the image **and** describe how the method will reduce the file size.
>
>> [!success]- Answer — 1 mark for naming the method, 1 per description bullet to max 2
>> - **Run-length encoding**
>> - Replaces **sequences of the same colour** pixel
>> - … with the **colour code and the number of identical pixels**
>> - The two words the mark scheme bolds are **sequences** and **same colour**
>>
>> *Latest: `9618_s21_qp_11_sc_1.b`*

> [!question] 9618 | Explain how a bitmap image is compressed using RLE [2]
> Explain how a bitmap image is compressed using run-length encoding (RLE).
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - **Sequences of consecutive identical colours / pixels**
>> - … are stored as the **colour value and the number of times it occurs consecutively**
>> - The two credited words are **consecutive** and **repeating** — "the same colours are stored once" is not enough
>>
>> *Latest: `9618_w25_qp_11_sc_7.d.iii` (also `s24_qp_13_sc_2.b.ii`)*

> [!question] 9618 | Describe one lossless method of compressing a text file [3]
> Describe **one** lossless method of compressing a text file.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - **Run-Length Encoding // RLE**
>> - **Repeated sequences of the same characters** are replaced by
>> - … **a single copy of the character**
>> - … **and a count of the number of characters**
>> - The four-bullet structure is worth copying exactly — naming it is one mark, and the mechanism is two more
>>
>> *Latest: `9618_w24_qp_11_sc_4.b.ii` (also `w22_qp_11_sc_7.c`)*

> [!question] 9618 | Complete an RLE compression table [2]
> The table shows compressed and uncompressed values for parts of an image file, where each colour is represented by a hexadecimal value. Complete the table.
>
>> [!success]- Answer — 1 mark for each correctly completed part
>> - Given: `EA F1 F1 F2 F2 F2 EA` → `1EA 2F1 3F2 1EA`
>> - **Backwards:** `2AB 2FF 11D 167` → **`AB AB FF FF 1D 67`**
>> - **Forwards:** `32 32 80 81 81` → **`232 180 281`**
>> - The question runs in **both directions** — expansion must be as fluent as compression
>> - Note the count comes **first**, then the colour value
>>
>> *Latest: `9618_w22_qp_12_sc_8.c.i`*

> [!question] 9618 | Explain why RLE may not reduce the file size, with an example [3]
> An image can be compressed using run-length encoding (RLE). Explain the reasons why RLE may **not** reduce the file size of a bitmap image. Give **one** example in your answer.
>
>> [!success]- Answer — 1 mark each to max 2 for the explanation + 1 for an image-related example
>> - RLE stores a **colour and the number of times it occurs consecutively**
>> - An image may **not have many sequences of the same colour**
>> - It would need to store **each colour and then the count / number 1**, which **adds data**
>> - **Example:** Red-Green-Blue would become **Red 1 Green 1 Blue 1**
>> - The sharpest question in the sub-topic — and the only one that tests the **limits** of the method
>>
>> *Latest: `9618_s23_qp_11_sc_1.c.ii`*

> [!question] 9618 | Describe two lossy methods of compressing an image [4]
> Describe **two** lossy methods that can be used to compress an image.
>
>> [!success]- Answer — 1 mark per bullet to **max 2 for each method**
>> - **Reduce bit depth**
>> - … reduces the number of bits per colour / pixel, which means each pixel has **fewer bits**
>> - **Reduce colour palette** // reduce the number of colours
>> - … **fewer colours mean fewer bits** needed to store each colour
>> - **Reduce image resolution**
>> - … **fewer pixels per unit measurement** means less binary to store
>> - Three methods are credited, but only **two** can score — each needs its expansion
>>
>> *Latest: `9618_w21_qp_12_sc_5.b.ii`*

> [!question] 9618 | Describe one method of compressing a sound file using lossy compression [2]
> Describe **one** method of compressing a sound file using lossy compression.
>
>> [!success]- Answer — 1 mark for the point, 1 for a **matching** expansion
>> - **Decrease the sample rate**
>> - … fewer samples / readings / measurements stored per second // fewer bits per second stored
>> - **Decrease the sample resolution**
>> - … fewer bits per sample / reading / measurement // each sample has fewer bits
>> - **Sound outside the set / human hearing range is removed**
>> - … fewer measurements are stored // decreases the number of possible binary values so fewer bits are stored
>>
>> *Latest: `9618_w24_qp_13_sc_6.c.ii`*

> [!question] 9618 | Describe how lossless compression can compress a sound file [2]
> Describe how lossless compression can compress a sound file.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - **Reduce the amplitude to only the range used**
>> - … limited amplitudes mean **fewer bits per sample**
>> - **Run-length encoding**
>> - … where consecutive sounds are the same, record the **binary value of the sound and the number of times it repeats**
>> - **Record the changes instead of the actual sounds**
>> - That last method — storing **deltas** — is credited here and nowhere else in the chapter
>>
>> *Latest: `9618_w21_qp_11_sc_7.b.ii`*

> [!question] Inferred | Explain how a vector graphic can be compressed [3]
> Explain how a vector graphic file can be compressed, and why it compresses less well than a bitmap.
>
>> [!success]- Answer — 5 points for 3 marks
>> - An **SVG file is an XML text file**, so it can be compressed with the same **lossless text methods** as any document
>> - … producing a compressed `.svgz` file that can be restored exactly
>> - A vector image can also be simplified by **reducing the number of objects or control points**
>> - … which is **lossy**, because the removed detail cannot be recovered
>> - It compresses **less well than a bitmap** because a drawing list contains **little redundant data**
>> - … whereas a bitmap stores long runs of identical pixels, which is exactly what RLE exploits
>>
>> *Inference: the bullet names "a text file, bitmap image, **vector graphic** and sound file". Text, bitmap and sound each have multiple 9618 questions; **vector graphics have none, in either series**. The only trace is one line inside a comparison mark scheme. **The clearest gap in 1.3.**

> [!question] Inferred | Express an RLE compression in binary [3]
> The text "AAAABBBCCDAA" is compressed using run-length encoding. Show the compressed form, and show how the first pair would be stored in binary.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Compressed form: **4A 3B 2C 1D 2A**
>> - … four A's, three B's, two C's, one D, two A's
>> - The **count** is stored in a fixed-size binary field (e.g. 7 or 8 bits)
>> - The **character** is stored using its **ASCII value** (7 bits)
>> - So `4A` = **`0000100 1000001`** — 4 as the count, 65 (`A`) as the character
>>
>> *Inference: 9618 asks for RLE in hexadecimal pairs and in prose. **The binary form has never appeared in a question in either series**, though SME teaches it and it is the only version that shows why RLE actually saves bits.*

> [!question] SME | Work through RLE on a one-bit image [3]
> A bitmap image has a bit depth of 1 bit. Explain how run-length encoding compresses it, and state the kind of saving that can be achieved.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The image is read as a stream of bits, and RLE creates **frequency/data pairs**
>> - … e.g. `30 11 20 11 20 11 50 11 …` — three 0s (white) then one 1 (black), and so on
>> - Pairs can **carry over onto the next line** — the end of one row and the start of the next count as one run
>> - SME's worked image drops from **195 bits to 38 bits**, a saving of about **80%**
>> - For images with more than two colours, the **RGB value** of each colour is stored with the count
>> - … e.g. `10 0 0 0` = ten black pixels, `5 255 0 0` = five red, `3 0 255 0` = three green
>>
>> *The carry-over across rows and the RGB form are both SME-only; 9618 marks RLE description questions at 2–3.*
