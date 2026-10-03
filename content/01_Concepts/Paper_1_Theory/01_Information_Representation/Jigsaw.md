---
title: Jigsaw — 1 Information Representation (AS Level)
syllabus: 9618 (2026)
topics: 1.1 Data Representation · 1.2 Multimedia · 1.3 Compression
---

# Jigsaw — 1 Information Representation

Syllabus content for **9618 Topic 1**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording. Fair game — just untested in the current series. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers.

---

> [!note] The most examined topic in the paper
> Topic 1 carries **128 pages** of 9618 Legend — more than Databases. It is also the most *predictable*: the same half-dozen calculations and conversions recur every series, almost always as **Question 1**. The marks here are won by **speed and accuracy**, not by recall, which makes it the one topic where drilling beats reading.

> [!note] Two habits that protect marks throughout
> **Always show working.** Nearly every calculation question splits its marks as *1 for working, 1 for the answer* — so a correct answer with no working caps at 1, and a wrong answer with correct working still scores 1.
> **Read the unit demanded.** Questions ask for the answer in kibibytes, mebibytes, megabytes or gigabytes, and the divisor changes with it. Getting the arithmetic right and the unit wrong scores the working mark only.

---

# 1.1 Data Representation

## 1.1.1 Binary magnitudes, and binary versus decimal prefixes

> [!success] State one difference between two named units [1]
> Two acceptable forms, and the second is far quicker to write:
> **By value** — a kibibyte = 1024 bytes // 2¹⁰ bytes **and** a kilobyte = 1000 bytes · a tebibyte = 1024 gibibytes / 1 048 576 kibibytes / 2⁴⁰ bytes **whereas** a gigabyte = 1000 megabytes / 1 000 000 kilobytes / 10⁹ bytes.
> **By prefix type** — "**kibi is a binary prefix and kilo is a denary prefix**". One line, full mark. `9618_w24_qp_11_sc_1.a`; `9618_w23_qp_12_sc_3.a`; `9618_s23_qp_11_sc_3.d.i`

> [!success] Complete the description of prefixes [4]
> A kibibyte has a **binary** prefix. Three kibibytes is the same as **3072** bytes. A megabyte has a **decimal / denary** prefix. Two terabytes is the same as **2000** gigabytes. *1 mark each* — note the question mixes a prefix-type answer with an arithmetic answer in the same four marks. `9618_s24_qp_13_sc_1.a`

> [!success] Tick the largest file size [1]
> Given 3300 kibibytes, 0.3 megabytes, 3 mebibytes, 3300 kilobytes → the answer is **3300 kibibytes** (3300 × 1024 = 3 379 200 bytes, against 3 145 728 for 3 mebibytes and 3 300 000 for 3300 kilobytes). The trap is that mebibytes *sound* bigger. `9618_s24_qp_12_sc_7.a`

> [!success] Match each binary value to its equivalent unit [5]
> 8 bits → **1 byte** · 8000 bits → **1 kilobyte** · 1000 kilobytes → **1 megabyte** · 1024 mebibytes → **1 gibibyte** · 8192 bits → **1 kibibyte**. *1 mark per line.* Two of the seven options (1 gigabyte, 1 mebibyte) are **distractors with no match**. `9618_w21_qp_11_sc_1.a`

> [!info] The **pebi / peta** row, and the units above tera
> The syllabus names only kibi/kilo, mebi/mega, gibi/giga and tebi/tera. SME teaches **pebibyte (2⁵⁰) and petabyte (10¹⁵)** as the next row. No question in either series has gone above tera — but the four named pairs have all appeared, so the pattern is complete and a fifth row would be a natural extension.

> [!info] **Why** the two systems exist
> Every question tests the *difference*; none asks the *reason*. The explanation — computers address memory in powers of 2, so RAM is quoted in binary prefixes, while storage manufacturers quote capacity in denary prefixes because the numbers look larger — has never been asked, in either series.

> [!abstract] The two tables, side by side
> **Denary (base 10):** kilobyte 10³ = 1000 bytes · megabyte 10⁶ · gigabyte 10⁹ · terabyte 10¹² · petabyte 10¹⁵.
> **Binary (base 2):** kibibyte 2¹⁰ = 1024 · mebibyte 2²⁰ = 1 048 576 · gibibyte 2³⁰ = 1 073 741 824 · tebibyte 2⁴⁰ · pebibyte 2⁵⁰.
> SME's rule of thumb for which to use: **be precise about memory** (16 GiB RAM really is 16 × 2³⁰ bytes), but a **rough estimate is acceptable for storage** (a 16 GB memory stick holds 16 × 10⁹ bytes).

---

## 1.1.2 Different number systems

> [!success] Tick the minimum number of bits needed to store each example [3]
> *3 marks for 6 correct ticks, 2 for 4–5, 1 for 2–3.* The hexadecimal value F139 → **16** (four hex digits × 4 bits) · 16 000 000 unique amplitude values → **24** (2²⁴ = 16.7 m) · an IPv4 address → **32** · 256 unique colours → **8** · an IPv6 address → **128** · the denary value 65 000 → **16**. A genuinely synoptic question — it needs IP addressing from Topic 2 and colour depth from 1.2. `9618_w25_qp_13_sc_2.a`

> [!success] State the number of unique binary values representable in n bits [1]
> 16 bits → **2¹⁶ // 65 536**. The general rule: *n* bits give **2ⁿ** distinct values. `9618_s23_qp_12_sc_4.a`

> [!success] Match descriptions to denary values [3]
> The smallest integer in 8-bit two's complement → **−128** · the largest integer in 8-bit two's complement → **127** · the largest **unsigned** integer in 8 bits → **255**. *1 mark per line.* The distractors (−127, −255, −256, 256, 128) are all near-misses, so the three must be known exactly. `9618_s23_qp_13_sc_7.a`

> [!success] Write the smallest and largest two's complement integers in 8 bits [2]
> *1 mark each.* Smallest **1000 0000** (= −128) · largest **0111 1111** (= +127). Note the question asks for the **binary patterns**, not the denary values — the matching question above asks for the denary. Read which is wanted. `9618_s25_qp_12_sc_2.b.ii`; `9618_s23_qp_11_sc_3.d.iv`

> [!success] State two benefits of using Binary Coded Decimal [2]
> *1 mark per benefit, max 2.* It is **straightforward to convert to and from denary** … so it is less complex to encode and decode for programmers · it is **easier for digital equipment** that displays output information · it can represent **monetary values exactly**. `9618_w22_qp_13_sc_9.b`

> [!success] State why a value cannot be interpreted as BCD [1]
> Because **the denary value in each group of 4 bits is greater than 9** // the value in each nibble is greater than 9. Any nibble from `1010` to `1111` is invalid BCD. `9618_w21_qp_12_sc_4.d`

> [!info] **One's complement** barely exists in 9618
> The syllabus names "**one's and two's complement** representation". Two's complement appears in almost every paper. **One's complement has been asked exactly once** — `9618_s23_qp_12_sc_4.b`, giving the 8-bit one's complement of −120 (working: +120 = `0111 1000`, answer: `1000 0111`). Its defining weakness — that it has **two representations for zero**, `0000 0000` and `1111 1111` — has never been examined in either series, though SME teaches it.

> [!info] Describing what a number base **is**
> Every question uses the bases; none asks what a base means. The definition — a number base is the count of distinct digits the system uses, and each column is a **power of the base** — plus the fact that **one hexadecimal digit maps exactly to one 4-bit nibble**, is assumed throughout and asked nowhere.

> [!info] Why **two's** complement rather than one's or sign-and-magnitude
> Untested in either series. The reason is that two's complement needs **no separate subtraction circuit** — the same adder handles any combination of signs — and it has **only one representation of zero**. SME makes this point explicitly; no mark scheme does.

> [!abstract] The four representations, defined
> **Binary** — base 2, digits 0 and 1, column weights 1, 2, 4, 8, 16 … **Denary** — base 10, digits 0–9. **Hexadecimal** — base 16, digits 0–9 then A–F (A = 10 … F = 15); each hex digit is exactly one nibble. **BCD** — each denary **digit** is separately coded as its own 4-bit pattern, so 2500 becomes `0010 0101 0000 0000`. BCD may be stored as one nibble per digit, or two digits packed into a byte.
> **One's complement:** invert every bit. **Two's complement:** invert every bit, then add 1 — or, faster, *keep every bit up to and including the rightmost 1, then flip the rest*. In two's complement the leftmost column becomes **negative** (−128 in 8 bits), which is why the range is −128 to +127.

---

## 1.1.3 Converting between number bases and representations

> [!note] The highest-frequency bullet in the entire paper
> **Fifty-one** separate 9618 questions sit under this one bullet, almost all worth 1–2 marks. Nothing here is conceptually hard; the marks are lost to arithmetic slips and to misreading which representation is wanted. Practise all nine conversions below until they are mechanical.

> [!success] Convert binary to hexadecimal [1]
> `101100111010` → **B3A** · `110001100111` → **C67** · `1110001100111011` → **E33B**. Split into nibbles **from the right**, convert each. `9618_w25_qp_13_sc_2.d`; `9618_w25_qp_11_sc_1.a.i`; `9618_w24_qp_11_sc_1.b.i`

> [!success] Convert hexadecimal to denary [1–2]
> `1FAB` → **8107** · `C0F` → **3087** (2 marks, with working). Multiply each digit by its power of 16. `9618_w24_qp_13_sc_8.a`; `9618_s24_qp_12_sc_7.c`

> [!success] Convert denary to hexadecimal [1]
> 241 → **F1**. Divide by 16: quotient is the first digit, remainder the second. `9618_s24_qp_13_sc_1.b`

> [!success] Convert denary to binary **and** hexadecimal in one question [2]
> 558 → binary **0010 0010 1110**, hexadecimal **22E**. *1 mark each.* Doing the binary first and grouping into nibbles gives the hex free. `9618_s25_qp_12_sc_2.a`

> [!success] Convert denary to a 12-bit two's complement binary number [1]
> −108 → **1111 1001 0100** · −196 → **1111 0011 1100**. Convert the magnitude, pad to 12 bits, then invert and add 1. `9618_w25_qp_13_sc_2.b`; `9618_w23_qp_12_sc_3.b.i`

> [!success] Convert two's complement binary to denary [1–2]
> `11100010` → **−30** · `10010110` → **−106** · `100110010111` → **−1641** · `111110111100` → **−68** (2 marks, with working). `9618_s25_qp_12_sc_2.b.i`; `9618_w24_qp_11_sc_1.b.ii`; `9618_w25_qp_11_sc_1.a.iii`

> [!success] Explain **how** to convert two's complement to denary, and give the value [3]
> *1 mark per method bullet (max 2) + 1 for the correct conversion.* **Method 1:** flip each bit then add 1 … then convert the new binary number into denary (and negate). **Method 2:** treat the **most significant 1 bit as its corresponding negative denary value** … then add the other positive corresponding denary values. For `10011111` the answer is **−97**. Both methods are credited — but the question asks for an *explanation*, so the method must be written out, not just the answer. `9618_w24_qp_13_sc_8.b`

> [!success] Convert denary to BCD [1]
> 108 → **0001 0000 1000** · 964 → **1001 0110 0100**. One nibble per digit, including leading zeros. `9618_w25_qp_11_sc_1.a.ii`; `9618_s23_qp_11_sc_3.d.ii`

> [!success] Convert BCD to denary [1]
> `100001100101` → **865** · `010101110011` → **573**. Split into nibbles and read each as a single digit. `9618_w23_qp_12_sc_3.b.ii`; `9618_w24_qp_11_sc_1.b.iii`

> [!success] Convert an unsigned binary integer into BCD, showing working [2]
> `10010101` → denary **149** → BCD **0001 0100 1001**. *1 mark for the denary step, 1 for the BCD* — so the intermediate denary value is itself a mark. `9618_w22_qp_12_sc_2.a.iii`

> [!success] Convert a 12-bit two's complement value in the ACC [1]
> `11001101` → **−51**. Appears inside Chapter 4 assembly questions as well as Chapter 1. `9618_w21_qp_12_sc_4.b`

> [!success] Complete a character table across denary, binary and hexadecimal [3]
> `!` 33 → **0010 0001** / 21 · `L` → **76** / `0100 1100` / 4C · `ü` 252 / `1111 1100` → **FC**. *1 mark per completed space.* Three conversions in three marks, each in a different direction. `9618_s25_qp_13_sc_1.c.ii`

> [!info] **Hexadecimal to binary** asked on its own
> 9618 asks binary→hex repeatedly, and hex→denary repeatedly — but a bare **"convert this hexadecimal number into binary"** has never been set, despite being the easiest of the nine (each digit becomes one nibble). It appears only *inside* the character tables.

> [!info] Converting **negative** numbers into hexadecimal
> All hex conversions in 9618 use positive values. Converting a two's complement negative into hex (e.g. −68 → `1111 1011 1100` → **FBC**) has not been asked, though both halves have been separately.

> [!abstract] The conversion methods, in brief
> **Binary → denary:** add the column weights where there is a 1. **Denary → binary:** work left from the highest column that fits, subtracting as you go. **Binary ↔ hex:** group into nibbles of 4. **Denary → hex:** divide by 16, quotient then remainder. **Hex → denary:** first digit × 16, plus second digit. **Denary → BCD:** code each digit separately into 4 bits. **Two's complement:** invert and add 1 — or keep bits up to the rightmost 1, flip the rest.

---

## 1.1.4 Binary addition and subtraction

> [!success] Perform binary addition, showing working [2]
> *1 mark for the working (the carries), 1 for the answer.* `1010 1010 + 0011 0111` = **1110 0001**, carries `1 1 1 1 1`. Write the carry row — it **is** the working mark. `9618_w21_qp_11_sc_1.b.i`

> [!success] Add a denary number to a binary number, in binary [3]
> *1 mark per bullet:* converting the denary value to binary … the method for the addition … the final answer. For `0010 0011 + 15`: 15 = `0000 1111`, giving **0011 0010**. The conversion step is a separate mark from the addition. `9618_s21_qp_11_sc_1.c.ii`

> [!success] Subtract a denary number from a two's complement binary number [3]
> *1 mark per bullet:* converting the number being subtracted to **two's complement** … adding the values … the final answer. For `0010 0011 − 10`: −10 = `1111 0110`, and `0010 0011 + 1111 0110` = **0001 1001**. `9618_s21_qp_11_sc_1.c.iii`; `9618_w24_qp_11_sc_1.c`

> [!success] Subtract one denary number from another using binary subtraction [3]
> *1 mark each:* converting **both** numbers to binary · the subtraction method (convert to the negative and add, **or** direct subtraction) · the correct answer. For 100 − 10: `0110 0100` and `0000 1010`, answer **0101 1010**. **Both methods are equally credited** — direct borrowing is accepted, not only two's complement. `9618_s24_qp_12_sc_7.b`

> [!success] State how an overflow can occur when adding two binary integers [1]
> **The result is a larger number than can be stored in the given number of bits** // the result is greater than 255 (for 8 unsigned bits). `9618_w21_qp_11_sc_1.b.ii`

> [!info] Overflow is **named in the syllabus and asked once**
> The notes say "show understanding of **how overflow can occur**". There is exactly one 9618 question on it, worth **1 mark**, in the very first series (w21). Nothing has tested: overflow **flipping the sign bit** in a signed addition, how a programmer would detect it, or why the carry-out of a two's complement subtraction is discarded rather than being an error. All three are in SME, none in a mark scheme.

> [!info] Subtraction asked **without** a method being implied
> Every 9618 subtraction question either gives a two's complement value or says "using binary subtraction". A question that simply says *subtract* and leaves the method open — then asks the candidate to **justify why two's complement addition is used instead of borrowing** — is the untested conceptual version of this bullet.

> [!abstract] Why the extra bit is discarded
> SME's worked example makes the point no mark scheme states: when 48 + (−12) is done in 8-bit two's complement the sum produces a **ninth bit**, which is simply ignored, leaving `0010 0100` = 36 — the correct answer. In two's complement arithmetic that carry-out is a **by-product of the method**, not an overflow. Genuine overflow is when the result itself will not fit in the available bits.

---

## 1.1.5 Practical applications of BCD and hexadecimal

> [!success] Give one application where BCD is used, and justify it [2]
> *1 mark for the application, 1 for a **corresponding** justification.*
> **Financial / banking calculations** … because financial transactions use only **two decimal places and must be exact**, there are no accumulating or rounding errors, and it is difficult to represent decimal values exactly in normal binary.
> **Electronic displays** (calculators, digital clocks) … because visual displays only need to show **individual digits**, and conversion between denary and BCD is straightforward.
> **Storing the date and time in the BIOS** … because conversion with denary is easier.
> **Barcode systems** … because conversion between denary and BCD can be completed accurately. `9618_s25_qp_12_sc_2.c`; `9618_w23_qp_12_sc_3.c`

> [!warning] Describe a use of BCD representation [2]
> The 9608 framing is broader and adds one credited point 9618 never uses: **"when denary numbers need to be electronically coded"** · e.g. to operate displays on a calculator where each digit is represented separately · **decimal fractions can be accurately represented**. `9608_s15_qp_13_sc_1.b.ii`; `9608_w19_qp_11_sc_5.c.ii`; `9608_w17_qp_13_sc_1.b.iii`

> [!info] **Hexadecimal applications have never been asked — in either series**
> The bullet is titled *"practical applications where Binary Coded Decimal (BCD) **and Hexadecimal** are used"*. **Every question in both series asks only about BCD.** The hexadecimal half has no question against it anywhere.
> The available content: hex is a **shorthand for binary** that is far easier for humans to read and less error-prone to transcribe, because one hex digit replaces four bits. Real uses: **MAC addresses**, **IPv6 addresses**, **HTML/CSS colour codes** (`#FF0000`), **memory addresses and memory dumps**, **assembly language operands and error codes**, and the **ASCII/Unicode code point tables**. Several of these are already examined elsewhere in the syllabus (MAC and IPv6 in Topic 2, memory addresses in Topic 4), which makes a synoptic "why is hexadecimal used here" question very easy to set. **This is the clearest single gap in Topic 1.**

> [!info] The **drawbacks** of BCD
> Both series ask only for benefits. The costs — BCD **wastes storage**, since 4 bits represent only 10 of 16 possible patterns, and **arithmetic is more complex** than in pure binary — have never been asked, though they are the obvious counterweight to the benefits question that *is* set.

> [!abstract] The use-case table
> **Electronic calculators** — keeps numbers in decimal format for easier display and accuracy. **Digital clocks and watches** — time is naturally decimal (12:45), so display logic is simpler. **Banking and financial systems** — avoids rounding errors in decimal calculations, especially with money. **Older digital and embedded systems** — simpler to implement with hardware that drives one digit at a time.

---

## 1.1.6 Character sets

> [!success] Explain how text is represented by a character set [2]
> *1 mark per bullet, max 2.* Each character has a **unique** code · each character in the text is **replaced sequentially / in order** by its code · the codes are **stored in the order they appear** in the word. `9618_w25_qp_13_sc_1.b`; `9618_s24_qp_13_sc_1.d.ii`; `9618_s21_qp_12_sc_6.b`

> [!success] Give two differences between ASCII and Unicode [2]
> *1 mark per bullet, max 2.* **ASCII uses 7 / 8 bits; Unicode can use many more — up to 32** · Unicode can represent a **wider range of characters, including different languages**. `9618_w25_qp_13_sc_1.c`

> [!success] Give one similarity **and** two differences between ASCII and Unicode [3]
> *1 mark for the similarity, 2 for differences.*
> **Similarity (max 1):** both **can** use 8 bits · both represent each character using a **unique** code · Unicode contains all the characters ASCII contains // **ASCII is a subset of Unicode**.
> **Differences (max 2):** Unicode goes up to 32 bits per character whereas ASCII is 7 or 8 · Unicode represents a wider range of **characters** · different **languages** are represented in Unicode, ASCII is only for one. `9618_w22_qp_11_sc_1.c`

> [!success] Give two advantages of Unicode instead of ASCII [2]
> A **wider range of characters** can be represented · so characters from **more languages** can be represented · and symbols such as **emojis** can be used. `9618_s25_qp_11_sc_3.b.i`

> [!success] Give two characteristics of the Unicode character set [2]
> **8 / 16 / 32 bits per character** · represents **2⁸ / 2¹⁶** etc. characters · represents **every language** and other characters such as emojis. `9618_s25_qp_13_sc_1.c.i`

> [!success] Identify and describe one character set [2]
> *1 mark for identification, 1 for a **matching** description.* **ASCII** — 7/8 bits per character // represents 128/256 characters // represents all characters from the Latin alphabet. **UNICODE** — 8/16/32 bits per character // represents 256/65 536+ characters // represents all characters in all languages. `9618_w24_qp_13_sc_6.a`

> [!success] State the number of bits each character set allocates [1]
> *1 mark for **all three** correct.* ASCII → **7** · extended ASCII → **8** · Unicode → **16/32**. All-or-nothing. `9618_s24_qp_13_sc_1.d.i`

> [!success] State the number of characters ASCII and extended ASCII can represent [2]
> ASCII = **128 // 2⁷** · Extended ASCII = **256 // 2⁸**. `9618_s21_qp_12_sc_6.a`

> [!success] State the number of bits used to store one Unicode character [1]
> **8 // 16 // 32 // 64** — any of these is credited, which is unusually generous. `9618_w25_qp_12_sc_7.b`

> [!success] Convert a character's code between representations [1]
> The Unicode character `ɮ` = `0010 0111 0110 1110` → denary **10 094** · the Unicode character `∑` = hex 2140 → denary **8512** · ASCII `h` = denary 104 → BCD **0001 0000 0100**, hexadecimal **68** · Unicode `1` = denary 49 → hex **31** · Unicode `5` → denary **53**. The character-set questions are really conversion questions in disguise. `9618_s25_qp_11_sc_3.b.ii`; `9618_w25_qp_12_sc_7.c.i`

> [!success] Use a code table to decode received binary values [1]
> Given a word/value lookup table, `0011 1000` → 56 → **Science**, `0011 1100` → 60 → **is**, `0011 1110` → 62 → **Amazing!**. *1 mark for all three in the correct order.* `9618_w25_qp_12_sc_6.b`

> [!warning] Give two disadvantages of using ASCII [2]
> Only **128 / 256** characters can be represented · it uses values **0 to 127** (or 255 extended) / one byte · **many characters used in other languages cannot be represented** · in extended ASCII the characters from **128 to 255 may be coded differently on different systems**. That last point — extended ASCII is **not** consistently standardised — appears in no 9618 mark scheme. `9608_w16_qp_13_sc_8.c.i`

> [!warning] Describe how Unicode is designed to overcome the disadvantages of ASCII [2]
> Uses **16, 24 or 32 bits** / two, three or four bytes · Unicode is designed to be a **superset of ASCII** · designed so that most characters in other languages can be represented. The word **superset** is the sharp version of 9618's "ASCII is a subset of Unicode". `9608_w16_qp_13_sc_8.c.ii`

> [!warning] Define the term character set [1]
> **The symbols that the computer recognises / uses** // a list of characters recognised by the computer hardware and software. 9618 has never asked for the definition itself, only for how one works. `9608_s18_qp_12_sc_4.b.i`

> [!warning] Explain the differences between ASCII and Unicode [2]
> Adds one point 9618 does not credit: **Unicode is standardised while ASCII is not**. Otherwise the same content as the 9618 difference questions. `9608_s18_qp_12_sc_4.b.ii`

> [!warning] Calculate a character code by arithmetic on another [2]
> *1 mark for working, 1 for the answer.* If ASCII `A` = 41₁₆, then `Z` = A + 25₁₀ = 41₁₆ + 19₁₆ = **5A₁₆**. This exploits the fact that character sets are **ordered logically** — a property 9618 relies on implicitly but has never made the subject of a question. `9608_s18_qp_12_sc_4.b.iii`; `9608_s19_qp_12_sc_3.d.iii`

> [!info] The **logical ordering** property
> SME makes the point that a character set is ordered so that the code for `B` is one more than the code for `A`, and that in ASCII the **sixth bit alone distinguishes upper from lower case** (`a` = `0110 0001`, `A` = `0100 0001`), which makes case conversion a single bit operation. 9608 exploits the ordering in a calculation question; **9618 has never tested either property**, even though it is the reason character sets are designed the way they are.

> [!abstract] ASCII versus Unicode, feature by feature
> **Bits:** ASCII 7 · extended ASCII 8 · Unicode minimum 16. **Characters:** 128 · 256 · 65 536+. **Covers:** standard English keyboard · plus mathematical operators and symbols such as © · all major world languages and emoji. **Benefit:** ASCII uses far less storage. **Drawback:** ASCII cannot represent other languages or special characters; Unicode uses considerably more storage.
> The first **128 Unicode code points are identical to ASCII**, which is what makes Unicode backward compatible.

---

# 1.2 Multimedia

## 1.2.1 How data for a bitmapped image is encoded

> [!success] Describe how the data for a bitmapped image is encoded [3]
> *1 mark each.* The image is **made of pixels and each pixel has one colour** · each colour has a **unique binary code** · the **code for the colour of each pixel is stored in sequence**. Note the parallel with character sets and with sound — Cambridge marks all three the same way: *unit → unique code → stored in sequence*. `9618_s24_qp_12_sc_2.d.i`

> [!success] Define the bitmap terms [3]
> **Pixel** — the smallest part of the image // one square or dot of one colour // the smallest addressable element in an image · **Colour / bit depth** — the number of bits per pixel // the number of bits used to represent each colour // determines the number of colours that can be represented · **File header** — stores data about the image file / **metadata**. `9618_s23_qp_11_sc_1.a`; `9618_w24_qp_12_sc_7.a.i`; `9618_s21_qp_11_sc_1.a.i`

> [!success] Complete the statements about bitmap images [2]
> The **bit depth** of a bitmap image is the number of bits used to store each pixel. Metadata about the image is stored in the **header** of the file. `9618_w22_qp_13_sc_2.e`

> [!success] Complete the table of bitmap statements [3]
> The smallest element that makes up an image → **pixel** · the largest number of different colours representable with a bit depth of 8 bits → **256 // 2⁸** · the term for the dots per inch (dpi) when an image is displayed → **screen resolution**. `9618_s25_qp_11_sc_3.a`

> [!success] State the largest number of colours representable by n bits [1]
> 8 bits → **256 // 2⁸**. The formula is **2ⁿ**, exactly as for unique binary values in 1.1.2. `9618_w24_qp_13_sc_6.b.i`

> [!success] Identify two other items in a bitmap file header [2]
> Given that colour depth and image resolution are already there: **confirmation that it is a bitmap / the file type** · the **compression type** used · the **location / offset of the data** within the file · the **dimensions**, e.g. 100 × 100 pixels. `9618_s23_qp_11_sc_1.b.i`

> [!success] Explain why the actual file size is larger than the calculated estimate [2]
> The file will contain **metadata** · the file will have a **header**. This is why every file-size question says "calculate an **estimate**". `9618_w25_qp_11_sc_7.d.ii`

> [!info] **Image resolution versus screen resolution**
> Both terms are named in the syllabus. **Image resolution** is examined constantly (every file-size calculation uses it). **Screen resolution** appears exactly once, as the one-word answer "screen resolution" to a dpi description (`s25_qp_11_sc_3.a`) — and once as a distractor in `w22_qp_12_sc_8.a`, where changing the screen resolution correctly has **no effect on the file size**. The distinction itself — that image resolution is a property of the *file* while screen resolution is a property of the *display* — has never been the subject of a question.

> [!abstract] Pixel density, and why it matters
> SME adds the layer above screen resolution: **pixels per inch (PPI)** is the pixel density, which depends on the resolution **and the physical size** of the display. A 65″ 4K television works out at about **68 PPI**, while a modern smartphone exceeds **300 PPI** — which is why a phone can be viewed from a few inches without visible pixelation and a television cannot. Not in any mark scheme, but it explains the dpi row that *is* examined.

---

## 1.2.2 Calculating bitmap file size

> [!note] The formula, and the only thing that changes
> **File size = image resolution (width × height) × colour depth**, giving a size **in bits**.
> Then divide: **÷ 8** for bytes · **÷ 1000** per denary step (kB, MB, GB) · **÷ 1024** per binary step (KiB, MiB, GiB).
> *1 mark for working, 1 mark for the answer*, every time. Nine 9618 questions, identical structure.

> [!success] Calculate the file size in megabytes [2]
> 1000 × 2000 × 16 bits ÷ (8 × 1000 × 1000) = **4 MB** · 2 000 000 pixels × 16 ÷ (8 × 1000 × 1000) = **4 MB** · 1500 × 3000 × 8 **bytes** ÷ 1000 ÷ 1000 = **36 MB**. Watch the third one: the bit depth is given **in bytes**, so there is no ÷ 8. `9618_w25_qp_12_sc_6.d`; `9618_s25_qp_13_sc_1.a.i`; `9618_s23_qp_11_sc_1.b.ii`

> [!success] Calculate the file size where the bit depth is given in bytes [2]
> 4000 × 3000 × **4 bytes** = 48 000 000 bytes = **48 MB**. The working mark is just `4000 * 3000 * 4` — no division by 8, because the depth is already in bytes. The single most common slip in this bullet. `9618_s24_qp_13_sc_2.a`

> [!success] Calculate the file size in kibibytes [2]
> 2048 × 1024 × 16 ÷ (8 × 1024) = **4096 kibibytes** · 512 × 2048 × 8 ÷ (8 × 1024) = **1024 kibibytes // 2¹⁰ kibibytes**. Note "a maximum of 256 colours" means a bit depth of **8**. `9618_w23_qp_13_sc_2.b`; `9618_w25_qp_11_sc_7.d.i`

> [!success] Calculate the file size in mebibytes [2–3]
> 2048 × 1024 × 10 ÷ (8 × 1024 × 1024) = **2.5 mebibytes** · 1024 × 512 × 8 bits ÷ 8 ÷ 1024 ÷ 1024 = **0.50 mebibytes** (3 marks: *1 per working bullet, 1 for the answer*). `9618_w23_qp_12_sc_6.c`; `9618_s21_qp_11_sc_1.a.ii`

> [!success] Calculate the file size of one second of video [2]
> A video is a sequence of bitmap frames, so the frame rate is simply another multiplier: 4000 × 3000 × **30 frames** × 16 ÷ (8 × 1000 × 1000 × 1000) = **0.72 gigabytes**. `9618_w25_qp_13_sc_7.b`

> [!info] Working **backwards** from a file size
> Every question gives the resolution and depth and asks for the size. The inverse — given a file size and resolution, find the **bit depth**; or given a size and a storage limit, find **how many images fit** — has never been asked in 9618, though it uses exactly the same formula and is a standard way to raise the difficulty.

> [!info] The file size of a **vector** graphic
> Calculations are only ever asked for bitmaps. The syllabus has no vector-size bullet, so this is correctly untested — but it is worth knowing *why*: a vector file stores a **drawing list of commands**, so its size depends on the **number of objects**, not on the image dimensions.

> [!abstract] The worked SME example, including a sound file
> **Image:** 250 000 pixels × 24 bits = 6 000 000 bits = 750 000 bytes = **732 KiB** or **750 kB**.
> **Sound** uses the same discipline: **sampling rate × sampling resolution × duration in seconds**. For `w22_qp_13_sc_1.b`: 50 kHz × (20 × 60 s) × 16 bits = 960 000 000 bits = 120 000 000 bytes = **120 megabytes**. That sound calculation is filed under *Data Representation* in the Legend, not Multimedia — but it is the same formula with time in place of area.

---

## 1.2.3 Effects of changing elements of a bitmap image

> [!success] Explain the effect of decreasing the bit depth, on the image and on the file [4]
> *1 mark each, two for the image and two for the file.*
> **Image:** there will be **fewer shades of colour available** … so the image does not match the original, as **detail is lost**.
> **Image file:** **fewer bits are used to store each pixel** … so less data is stored, therefore the **file size is reduced**. `9618_s25_qp_13_sc_1.a.ii`

> [!success] State what is meant by bit depth, and explain how changing it affects the image [3]
> *1 mark definition + 1 per explanation bullet.* **Definition:** the number of bits used to represent each colour. **Explanation:** an increase means a **greater range of colours** (a decrease, a smaller range) · an increase makes the image **closer to the original / more realistic** (a decrease, less like the original). `9618_w23_qp_11_sc_1.b`

> [!success] Explain why changing the image resolution affects quality and file size [2]
> *1 mark for each explanation.* **Quality:** decreasing the resolution means **detail is lost because there are fewer pixels** // increasing means more detail because there are more pixels. **File size:** decreasing the resolution decreases the file size **because there are fewer pixels therefore less data** // increasing increases it. Each half must carry its **because** — the bare statement scores nothing. `9618_w24_qp_12_sc_7.a.ii`

> [!success] Describe the impact of increasing the image resolution on quality [2]
> **More pixels can be stored / are available** · the image is **sharper / less pixelated**. `9618_w23_qp_13_sc_2.a`

> [!success] State one drawback of increasing the bits per pixel [1]
> **Increased file size.** `9618_w24_qp_13_sc_6.b.ii`

> [!success] Identify two elements that can be changed to reduce file size [2]
> **Colour / bit depth** · **image resolution**. Only these two — a third answer earns nothing. `9618_s24_qp_13_sc_2.c`

> [!success] Tick the effect of each action on the file size [2]
> *1 mark for one or two correct rows, 2 marks for all three.* Change the colour depth to 16 bits per pixel (from 24) → **decreases** the file size · change the **screen** resolution to 1366 × 768 → **no change** · change the colour of the rectangle from black to red → **no change**. The two "no change" rows are the question: screen resolution is a property of the **display**, and changing which colour is used does not change how many bits store it. `9618_w22_qp_12_sc_8.a`

> [!info] The **trade-off** framed as a decision
> Every question asks what happens when a value changes. None asks the candidate to **recommend** a resolution or depth for a stated purpose and justify it — the format used constantly in Chapter 3 for storage devices. Given that 1.2.5 already asks for a justified choice between bitmap and vector, the same framing applied to resolution and depth is readily available.

---

## 1.2.4 How data for a vector graphic is encoded

> [!success] Define the vector graphic terms [2–3]
> **Drawing list** — **all the drawing objects in an image** // a list that stores the **commands / descriptions / mathematical equations** required to draw each object · **Drawing object** — a component created using a **formula** · **Property** — an **attribute of a drawing object** // data about a shape // defines **one aspect of the appearance** of a drawing object. `9618_w24_qp_12_sc_7.b`; `9618_w23_qp_11_sc_1.a`; `9618_s23_qp_11_sc_1.a`

> [!success] Describe the contents of a vector graphic drawing list [2]
> *1 mark each to max 2.* A **list of the objects** in the drawing · a list that stores the **command / description / equation required to draw each object** · the **properties of each object**, e.g. the fill colour, line weight or colour. `9618_s24_qp_12_sc_2.d.ii`

> [!success] Describe each vector term **and** give an example from a given logo [4]
> *1 mark for each description, 1 for each valid example.* **Property** — data about the shapes // defines one aspect of the appearance … *e.g.* black line, white fill, solid line, font of the letter, colour of the triangle. **Drawing list** — the list of shapes involved in an image … *e.g.* triangle, capital letter R, rectangle, line. The example must be read **off the image given**. `9618_w21_qp_12_sc_5.a`

> [!success] Match each vector term to its description [2]
> *2 marks for all 3 correct, 1 mark for 1 correct.* **Drawing list** → data required to create all components in the graphic · **Drawing object** → a component created using a formula · **Property** → defines one characteristic of a component. `9618_w23_qp_11_sc_1.a`

> [!info] The **relative position** of objects
> SME lists three things a drawing list holds: the **commands** to create each object, the **attributes/properties** of each object, and the **relative position** of each object. 9618 mark schemes credit the first two repeatedly; **position is never mentioned** — yet it is what makes a drawing list reproducible, and it is the reason a vector image has no fixed dimensions.

> [!info] Why a vector graphic **scales without loss**
> Credited as a bare point in the comparison questions ("when vector is enlarged it is recalculated and does not pixelate"), but the mechanism — the file stores **equations, not pixels**, so on enlargement the shape is **recalculated at the new size** rather than stretched — has never been the subject of its own question.

> [!abstract] What a vector file actually stores
> A vector graphic is created from **mathematical equations and points**; only the mathematics is stored. To draw a circle, the data stored is the **centre point (x, y) and the radius** — nothing else. The drawing list sits in the **file header**. Because **no dimensions are defined**, scaling up causes no loss of quality. Typical examples are **logos and clipart**; typical file types are `.svg`, `.ai`, `.eps`.

---

## 1.2.5 Justifying the use of a bitmap image or a vector graphic

> [!success] Describe two differences between a vector graphic and a bitmap image [4]
> *1 mark per bullet to **max 2 for each difference** — so two differences, each with an expansion.*
> **Composition:** bitmap is made of **pixels** // colours stored for individual pixels · vector stores a **set of instructions** about how to draw the shape.
> **Scaling:** when a bitmap is enlarged the **pixels get bigger and it pixelates** · when a vector is enlarged it is **recalculated and does not pixelate**.
> **File size:** bitmap files are usually bigger, because data about **each pixel** must be stored · vector files are smaller, because they contain **just the instructions**.
> **Compression:** bitmaps **compress well**, with significant reduction · vector graphics **do not compress well, because there is little redundant data**. `9618_w21_qp_12_sc_5.b.i`

> [!success] State two benefits of creating a vector graphic instead of a bitmap image [2]
> *1 mark each, max 2.* Can be **enlarged without pixelation / loss of quality** · **individual components** of the image can be edited · generally a **smaller file size**. `9618_w22_qp_12_sc_8.b`

> [!warning] Describe two drawbacks of using a bitmap for a logo instead of a vector [4]
> *1 mark per drawback, 1 for its expansion, max 2 each.* A bitmap file is likely to take up **more storage space** … because the colour of **each pixel** needs to be stored · a bitmap **cannot be enlarged** // is difficult to use in different types of document … **without the image pixelating** · a bitmap would be **more difficult to edit** … because **each pixel would need to be edited separately**. That last drawback — editability — appears in **no 9618 mark scheme**. `9608_s21_qp_11_sc_2.c`

> [!warning] Describe two reasons why a vector graphic is a sensible choice for a logo [4]
> *1 mark per bullet, max 2 per reason.* **Smaller file size** … so it can be transferred / downloaded quicker · **enlarges without pixelation** … because it needs to be used on different **screens / devices / resolutions**. `9608_w18_qp_12_sc_1.c`; `9608_s18_qp_11_sc_2.d`

> [!warning] State two reasons why a logo is saved as a vector graphic [2]
> Adds a storage angle 9618 does not use: needs to be **large for signs** without pixelating · smaller file size means **faster transfer rates** · smaller file size **reduces storage requirements when stored many times** on multiple documents. `9608_s20_qp_12_sc_1.b.ii`

> [!info] 9618 has asked this bullet **once**, for 2 marks
> There is exactly **one** 9618 question under *"justify the use of a bitmap image or a vector graphic for a given task"* — `w22_qp_12_sc_8.b`, worth 2 marks. **9608 has five**, several at 4 marks with the point-plus-expansion structure. Given that every other Multimedia bullet is examined repeatedly in 9618, this one is overdue, and the 9608 answers above are the model.

> [!info] Justifying a **bitmap** over a vector
> Every question in both series runs the argument one way: why vector beats bitmap for a **logo**. The reverse — why a bitmap is right for a **photograph** (continuous tone, millions of colours, no describable shapes to store as equations, produced directly by a camera sensor) — has never been asked, despite being half of what the bullet says.

> [!abstract] The decision questions SME suggests
> Three questions settle the choice every time: **Does the image need to be resized?** · **Does it need to be drawn to scale?** · **Does it need to look real?** The first two point to vector, the third to bitmap.

---

## 1.2.6 How sound is represented and encoded

> [!success] Describe how sound is represented in a computer [3]
> *1 mark each.* The **amplitude is recorded a set number of times a second** · each instance of an amplitude is given a **corresponding binary number** · the binary number of each amplitude is **saved in sequence**. The same three-part shape as the bitmap and character-set answers. `9618_s23_qp_13_sc_3.c.i`

> [!success] Explain how an analogue sound wave is converted into digital data [2]
> *1 mark per bullet, max 2.* The **value / magnitude / size of the analogue sound wave is measured a set number of times each second** / at set intervals · each sample / reading / measurement is **given a binary number and stored in sequence**. `9618_w24_qp_13_sc_6.c.i`

> [!success] Complete the table of sound terms [3]
> The number of times the amplitude is measured per time interval → **sampling rate** · the number of bits used to store each amplitude measurement → **sampling resolution** · the type of sound wave before it is recorded by a computer → **analogue**. `9618_s25_qp_13_sc_1.b`

> [!success] Match the sound terms to their descriptions [2]
> *1 mark for 1 correct line, 2 marks for all 3.* **Sampling** → taking measurements at regular intervals and storing the values · **Sampling rate** → the number of samples taken per second · **Sampling resolution** → the number of bits used to store each sample. `9618_w23_qp_13_sc_1.b`

> [!success] State what is meant by sampling rate [1]
> The number of samples taken **per unit time / per second**. `9618_w22_qp_11_sc_1.d.i`

> [!success] State what is meant by analogue data [1]
> Data values that are **continuously changing** // variable // can take **any** value. `9618_w23_qp_13_sc_1.a`

> [!warning] Complete the table by defining sampling, sampling rate and sampling resolution [3]
> *1 mark per definition.* **Sampling** — measuring the **amplitude of the wave at regular / set time intervals** · **Sampling resolution** — the number of bits used to represent **each sample** · **Sampling rate** — the number of samples taken **per unit of time**. 9618 asks for these as a *matching* exercise; 9608 asks for them to be **written out**. `9608_w21_qp_11_sc_2.a`; `9608_s20_qp_12_sc_2.a`

> [!warning] State what is meant by a given sampling rate and resolution [2]
> Applied to actual figures: a sampling rate of **88.2 kHz** means the sound wave is sampled **88 200 times per second** · a sampling resolution of **32 bits** means each sample is stored as a **32-bit binary number**. Reading the units off a specification is never asked in 9618. `9608_s19_qp_13_sc_5.c`

> [!warning] Describe how images **and** sound are encoded into digital form [4]
> *Max 3 for image, max 3 for sound.* **Images:** stored as bitmaps · each image is made of pixels · each pixel is a single colour · each colour has a unique binary number · **store the sequence of binary numbers for each image / frame**. **Sound:** measure the height / amplitude of the sound wave · a **set number of times per second** at regular intervals · each amplitude has a unique binary number · **store the sequence of binary numbers for each sample**. A single question covering both encodings, which 9618 has never set. `9608_w19_qp_12_sc_6.d.i`

> [!warning] Describe two features of sound editing software [4]
> *1 mark for naming the feature, 1 for describing it, max 2 per feature.* **Cut / delete** — remove part of the sound file · **Copy and paste** — replicate part of the sound · **Amplify** — increase the volume of a section · **Fading** — change the volume of a section so it gets louder or quieter · **Change pitch** — increase or decrease the frequency of a section · **Change sampling resolution** — to change the accuracy of the sound or the file size. Sound *editing* appears nowhere in the 9618 syllabus notes — treat this as background, not as a likely question. `9608_w18_qp_11_sc_1.c`; `9608_s18_qp_12_sc_5.d`

> [!info] The **ADC** named as a component
> 9618 asks repeatedly how analogue becomes digital but never names the device. SME calls the process **analogue-to-digital conversion (A2D)**; Chapter 3 examines the ADC as hardware. The link between the two — that the sampling described here *is* what the ADC in a microphone does — is never made in a question.

> [!info] Playing sound **back**
> Every question describes recording. The reverse path — the stored binary values are read in sequence, converted back to voltages by a **DAC**, and drive a speaker cone — is never asked, though SME describes it and the speaker is in the Chapter 3 syllabus.

---

## 1.2.7 Impact of changing the sampling rate and resolution

> [!success] Explain why increasing the sampling rate and resolution improves precision [4]
> *1 mark each; **max 2 for rate and max 2 for resolution**.*
> **Sampling rate:** there are **smaller 'gaps' in the sound wave** // sound is recorded more often · the **digital waveform is closer to the analogue waveform** · the **quantisation errors are smaller**.
> **Sampling resolution:** there are **more bits per sample** // a wider range of amplitudes can be stored · each binary amplitude is **closer to the analogue amplitude** · the digital waveform is closer to the analogue waveform · quantisation errors are smaller.
> Four points about the rate alone score 2. `9618_s23_qp_13_sc_3.c.ii`

> [!success] Explain the impact of changing the sampling resolution on accuracy [3]
> *1 mark per bullet, max 3.* **Increase:** the number of bits per sample is increased … more values are available to represent each sample // more amplitudes can be represented … each binary amplitude is closer to the analogue amplitude … **quantisation errors are reduced** … the digital soundwave is closer to the original analogue soundwave. **Decrease:** the mirror of each. `9618_w23_qp_12_sc_6.b`

> [!success] Explain the effect of increasing the sampling rate on accuracy [2]
> **Improves** the accuracy of the sound file · because the digital **waveform more closely resembles the analogue waveform** · **quantisation errors are reduced** · it increases the amount of detail stored. `9618_w22_qp_12_sc_6.b.i`

> [!success] Explain the effect of increasing the sampling resolution on the sound file [2]
> Increases the **number of bits per sample** // a larger range of values · which means the **file size increases** · makes the sound file more accurate // digital waveform closer to the original · **smaller quantisation errors**. `9618_w22_qp_11_sc_1.d.ii`

> [!success] Explain the effect of decreasing the sampling resolution on the file size [2]
> **Decreases** the file size of the sound file · because **fewer bits are used to store each sample**. `9618_w22_qp_12_sc_6.b.ii`

> [!success] Describe the reasons why a higher sample rate sounds closer to the original [2]
> **Smaller time gaps between the samples** · makes the **digital** sound wave more accurate · **smaller quantisation errors**. `9618_w21_qp_11_sc_7.a.i`

> [!success] Describe the reasons why the file size increases with a higher sample rate [2]
> **More samples / data are taken or recorded** · so **more bits are stored altogether**. `9618_w21_qp_11_sc_7.a.ii`

> [!success] Draw lines from each change to its impacts [3]
> *1 mark for each correctly connected change box, max 3.* Increase the **duration** → the file size gets bigger · **no change** to the accuracy. Increase the **sampling rate** → the file size gets bigger · the accuracy **improves**. Decrease the **sampling resolution** → the file size gets **smaller** · the accuracy **worsens**. Note each change box needs **two** lines. `9618_w25_qp_13_sc_1.a`

> [!success] Tick the effect of each action on accuracy [2]
> *1 mark for 1–2 correct, 2 marks for all 3.* Sampling rate 40 kHz → 60 kHz → accuracy **increases** · duration 20 → 40 minutes → accuracy **does not change** · sampling resolution 24 → 16 bits → accuracy **decreases**. The duration row is the trap: **longer recordings are bigger, not more accurate**. `9618_w22_qp_13_sc_1.a`

> [!success] Describe how a change in sampling rate affects a device's performance [3]
> *1 mark each, max 3.* Doubling the rate from 44.1 kHz to 88.2 kHz means **data transmission will take longer** … because there is **more data to transmit** · the **secondary storage device will fill faster** … so fewer videos can be stored long-term // videos are overwritten more often. An applied, consequences-based version of the bullet — the only one in 9618. `9618_s24_qp_11_sc_2.d`

> [!warning] Define sampling rate and explain its influence on accuracy [2]
> *1 mark for the definition, 1 for the explanation.* **Definition:** the number of samples taken per unit time // the number of times the amplitude is measured per unit time. **Explanation:** increasing the sampling rate will **increase the accuracy / precision of the digitised sound** // will result in **smaller quantisation errors**. 9618 asks the definition and the effect in separate questions; 9608 combines them. `9608_s17_qp_13_sc_3.a`; `9608_s17_qp_11_sc_3.a`

> [!warning] Define sampling resolution and explain its effect on accuracy [3]
> *Max 2 for the definition, max 2 for the explanation.* **Definition:** the number of **distinct values available** to encode each sample · specified by the number of **bits** used to encode one sample · sometimes referred to as **bit depth**. **Explanation:** a larger resolution means **more values available** to store each sample · improves accuracy // **decreases the distortion** of the sound · means a **smaller quantisation error**.
> Two pieces of vocabulary here are 9608-only: **"distinct values available"** and **"distortion"**. `9608_s17_qp_12_sc_3.a`

> [!info] **Quantisation error** named but never defined
> The phrase appears in six separate 9618 mark schemes as a credited point. **No question in either series asks what a quantisation error is** — that each sample must be rounded to the nearest value the resolution can represent, and the difference between the true amplitude and the stored one is the error. It is the single most-credited term in 1.2.7 and the least explained.

> [!info] **Nyquist** and choosing a rate
> Why a CD samples at **44.1 kHz** specifically — roughly twice the upper limit of human hearing — is not in the 9618 syllabus and has never been asked. Worth knowing as context for why "higher is always better" is not how rates are chosen in practice, but do not offer it as a mark-scheme point.

> [!abstract] The impact table, in one place
> **Sampling rate ↑** → more detail, better sound quality · more data, **larger file size**. **Sampling resolution ↑** → bigger range of amplitudes, better quality · more data per sample, **larger file size**. **Duration ↑** → **larger file size, no change to accuracy**.
> A typical audio CD: sampling rate **44.1 kHz**, sampling resolution **16 bits**, recorded in stereo.

---

# 1.3 Compression

## 1.3.1 The need for, and examples of, compression

> [!success] Explain why a video is compressed before real-time bit streaming [4]
> *1 mark each to max 4.* Video is **data-intensive** · the file size needs reducing in order to **reduce the amount of bandwidth used** · and **reduce buffering** · this means people are **not behind in the conversation** · and people with **lower bandwidth can still take part**. The highest-tariff compression question in the chapter, and the one most tied to Topic 2. `9618_s25_qp_11_sc_2.b.i`

> [!success] Explain the benefits of a compressed email attachment [3]
> *1 mark per bullet, max 3.* **Less storage space** is used … so more work can be stored · **transmission time is reduced** … so the recipient does not have to wait as long for it to arrive · **bandwidth usage is reduced** … so other transmissions are not adversely affected · **less data allowance** is used on the email system. Note the structure: each benefit has its own **consequence**, and the consequence is a separate mark. `9618_w24_qp_11_sc_4.b.i`

> [!success] Explain why a bitmap image is compressed before being attached to an email [2]
> **Reduced bandwidth usage** when transmitting · **reduced transmission time** from email client to email server · **reduced storage space on the email** · **email accounts often have a maximum size for an attachment**. That last point is specific to email and is easily missed. `9618_w23_qp_11_sc_1.c`

> [!success] Explain why compressing files benefits the customers who download them [3]
> *1 mark each.* Customers can **download in less time** · and it takes **less of the customer's bandwidth** · the files take up **less space on the customer's storage medium** · therefore customers can **store more images** · and have **more space for other files**. The answer must be framed from the **customer's** side, not the server's. `9618_s23_qp_11_sc_1.c.i`

> [!success] Explain the reasons for compressing files on a web server [2]
> To reduce the **time it takes to download** the files from the server // to **upload** them to the server in the first place · to reduce the **storage space used on the web server** // on the user's device. `9618_w23_qp_13_sc_5.b.i`

> [!success] Explain the reasons for compressing a sound file before emailing it [2]
> **Reduces the file size** · **faster to transmit / download** · the **original file is too large** for email storage or as an attachment. `9618_w21_qp_11_sc_7.b.i`

> [!success] Give two reasons why a video does **not** need to be compressed [2]
> The inverted question. *1 mark each to max 2.* A **dedicated connection** to the headset // not sharing bandwidth · an **already fast connection** that can transmit the data without slowing · the video **may already be a small file size** and does not need further reduction · the video is **not saved**, so storage is not an issue. `9618_s24_qp_12_sc_2.d.iii`

> [!info] The **cost** of compressing
> Every question asks for benefits. The trade-offs — compression and decompression take **processing time**, lossy compression **permanently destroys data**, and an already-compressed file **cannot usefully be compressed again** — are never asked. The "why not compress" question above (`s24_qp_12_sc_2.d.iii`) is the closest, and it is argued from bandwidth rather than from the cost of compressing.

> [!abstract] Named compression formats
> Not required by the syllabus, but useful as examples: **MP3** compresses audio by up to 90% using **perceptual music shaping** — removing frequencies outside human hearing and quieter sounds **masked** by louder ones; it is lossy. **MP4** stores audio, video, photos and animations and is the standard for streaming. **JPEG** is the standard lossy bitmap format, and it **creates a new file**, so the original can no longer be recovered. **SVG** vector files are XML text, which is why they compress at all.

---

## 1.3.2 Lossy and lossless compression, and justifying a method

> [!success] State whether a described method is lossy or lossless, and justify [1]
> A sound file compressed by **reducing the sampling rate** → **lossy** · because there will be **fewer samples per second, so data is permanently lost** // so the original sound **cannot be re-created**. The justification carries the mark; the label alone does not. `9618_w25_qp_12_sc_6.a`

> [!success] Identify the appropriate method for real-time bit streaming, and justify [3]
> **No mark for the choice** — but **lossy** is the expected answer. *1 mark each to max 3:* reduces file size **more than lossless** · so **significantly less bandwidth / data** is needed · so **buffering is reduced even more than with lossless** · data can be removed **which cannot be seen** · reducing quality **without impacting the experience** · for example, the resolution of the video can be reduced // the sample rate of the audio can be reduced. `9618_s25_qp_11_sc_2.b.ii`

> [!success] Tick the most appropriate compression type for a scenario, and justify [3]
> *1 mark per bullet, max 3.* **Both choices are credited if justified**, which is the key feature of this question.
> **Lossy:** loss of quality will not be noticed · needs to be viewed in **real time**, so less bandwidth is needed if the file is smaller · smaller files reduce **buffering**, so the video plays more smoothly · viewers may watch on different devices, so may not need high resolution.
> **Lossless:** the original recording may not have been made in high resolution · could be streaming to **high bandwidth** devices · the reduction in file size is **sufficient** for the receiving device · **viewers do not want any loss of quality**. `9618_w23_qp_12_sc_6.a`

> [!success] Explain why lossy compression is suitable for a bitmap image [2]
> *1 mark per bullet, max 2.* The change **may not be noticeable** // data removed is usually **not noticed by the human eye** · for example, changes in shade or detail · it produces a **larger decrease in file size** compared to lossless. `9618_w24_qp_13_sc_6.b.iii`

> [!success] Give three benefits of lossy instead of lossless for a photograph [3]
> *1 mark each to max 3 — and every point must be comparative.* The file takes **less storage space on the web server than if lossless was used** · is **faster to upload/download** than if lossless was used · uses **less bandwidth** to transmit than if lossless was used · **consumes less data allowance** than if lossless was used. `9618_s24_qp_13_sc_2.b.i`

> [!success] Explain why lossless is more appropriate than lossy for a text file [2]
> *1 mark per bullet.* **All the data is required** // **no data can be lost** · otherwise the text file will be **corrupted / not make sense**. `9618_w22_qp_12_sc_8.c.ii`

> [!info] Defining lossy and lossless
> Both terms are used in every question; **neither has ever been asked for as a definition** in 9618. The definitions — **lossy** permanently discards data and is **irreversible**; **lossless** encodes the data so the file can be **restored exactly** to its original state — are assumed throughout.

> [!info] Choosing lossless for a **sound** file
> The justification questions cover: lossy for video, lossy for photographs, lossless for text. The fourth combination — **lossless for audio**, where the recording is a master to be edited further or quality is non-negotiable — is never set, despite sound being examined heavily everywhere else in the topic.

> [!abstract] The two methods, defined
> **Lossy** — data is **removed** to reduce the file size; irreversible; greatly reduces size at the expense of quality; suitable where some quality loss is acceptable, i.e. **images, video and sound**. In photographs it groups similar colours together, reducing the number of colours without visibly compromising the image.
> **Lossless** — data is **encoded** rather than discarded; **reversible**, so the file returns to its original state; reduces size less dramatically; usable on all data but essential where loss is unacceptable, i.e. **documents and program files**. It works by analysing the contents for **patterns and repetition**. DOCX and PDF apply it automatically.

---

## 1.3.3 How a text file, bitmap image, vector graphic and sound file can be compressed

> [!success] Identify one lossless method of compressing an image [1]
> **Run-Length Encoding (RLE).** `9618_w24_qp_12_sc_7.a.iii`

> [!success] Identify a lossless method and describe how it reduces the file size [3]
> *1 mark for naming the method, 1 per description bullet to max 2.* **Run-length encoding** · replaces **sequences of the same colour** pixel · with the **colour code and the number of identical pixels**. `9618_s21_qp_11_sc_1.b`

> [!success] Explain how a bitmap image is compressed using RLE [2]
> *1 mark per bullet, max 2.* **Sequences of consecutive identical colours / pixels** · are stored as the **colour value and the number of times it occurs consecutively**. The two credited words are **consecutive** and **repeating**. `9618_w25_qp_11_sc_7.d.iii`; `9618_s24_qp_13_sc_2.b.ii`

> [!success] Describe one lossless method of compressing a **text** file [3]
> *1 mark per bullet, max 3.* **Run-Length Encoding / RLE** · **repeated sequences of the same characters** are replaced by · **a single copy of the character** · **and a count of the number of characters**. The four-bullet structure is worth copying exactly. `9618_w24_qp_11_sc_4.b.ii`; `9618_w22_qp_11_sc_7.c`

> [!success] Complete an RLE compression table [2]
> *1 mark for each correctly completed part.* Uncompressed `EA F1 F1 F2 F2 F2 EA` → compressed `1EA 2F1 3F2 1EA`. Working backwards: `2AB 2FF 11D 167` → **`AB AB FF FF 1D 67`**. Forwards: `32 32 80 81 81` → **`232 180 281`**. The question runs in **both directions**, so the expansion must be as fluent as the compression. `9618_w22_qp_12_sc_8.c.i`

> [!success] Explain why RLE may **not** reduce the file size, with an example [3]
> *1 mark each to max 2 for the explanation, 1 mark for an image-related example.* RLE stores a **colour and the number of times it occurs consecutively** · an image may **not have many sequences of the same colour** · it would need to store each colour **and then the count / number 1**, which **adds data**. **Example:** Red-Green-Blue would become **Red 1 Green 1 Blue 1**. The sharpest question in the sub-topic, and the only one that tests the limits of the method. `9618_s23_qp_11_sc_1.c.ii`

> [!success] Describe two lossy methods of compressing an image [4]
> *1 mark per bullet to **max 2 for each method**.* **Reduce bit depth** … reduces the number of bits per colour/pixel, which means each pixel has fewer bits · **reduce the colour palette** // reduce the number of colours … fewer colours mean fewer bits needed to store each colour · **reduce image resolution** … fewer pixels per unit measurement means less binary to store. `9618_w21_qp_12_sc_5.b.ii`

> [!success] Describe one method of compressing a sound file using lossy compression [2]
> *1 mark for the point, 1 for a **matching** expansion.* **Decrease the sample rate** … fewer samples / readings stored per second // fewer bits per second stored · **decrease the sample resolution** … fewer bits per sample // each sample has fewer bits · **sound outside the set / human hearing range is removed** … fewer measurements are stored // decreases the number of possible binary values so fewer bits are stored. `9618_w24_qp_13_sc_6.c.ii`

> [!success] Describe how lossless compression can compress a sound file [2]
> *1 mark per bullet, max 2.* **Reduce the amplitude to only the range used** … limited amplitudes mean fewer bits per sample · **run-length encoding** … where consecutive sounds are the same, record the **binary value of the sound and the number of times it repeats** · **record the changes instead of the actual sounds**. That last method — storing deltas — is credited here and nowhere else. `9618_w21_qp_11_sc_7.b.ii`

> [!info] Compressing a **vector graphic** — named in the syllabus, never asked
> The bullet reads *"show understanding of how a text file, bitmap image, **vector graphic** and sound file can be compressed"*. Text, bitmap and sound each have multiple 9618 questions. **Vector graphics have none, in either series.** The only trace is one line inside a comparison mark scheme: *"vector graphic images do not compress well because of little redundant data"*.
> The available content: an SVG is an **XML text file**, so it can be compressed with the same **lossless text methods** (producing `.svgz`); and a vector image can be simplified by **reducing the number of objects or control points**, which is lossy. **This is the clearest gap in 1.3**, and it is a one-mark name away from being examinable.

> [!info] RLE expressed in **binary**
> 9618 asks for RLE in hexadecimal pairs (`w22_qp_12_sc_8.c.i`) and in prose. The binary form — the count in a fixed-size field followed by the character's code, so `4A` becomes `0000100 1000001` — is taught by SME and has never appeared in a question, in either series.

> [!abstract] RLE worked three ways
> **Text:** `AAAABBBCCDAA` → `4A3B2C1D2A`. In binary, the count is stored in a fixed-size field (7 or 8 bits) and the character as its 7-bit ASCII value, so `4A` = `0000100 1000001`.
> **1-bit image:** frequency/data pairs, e.g. `30 11 20 11 20 11 50 11 …` — three white then one black, and so on. **Pairs can carry across the end of a row onto the start of the next.** SME's worked image drops from **195 bits to 38 bits, a saving of about 80%**.
> **Colour image:** the **RGB value** of each colour is stored with the count, e.g. `10 0 0 0` = ten black pixels, `5 255 0 0` = five red, `3 0 255 0` = three green.
