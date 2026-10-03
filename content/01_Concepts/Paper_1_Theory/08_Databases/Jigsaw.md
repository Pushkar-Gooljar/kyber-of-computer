---
title: Jigsaw — 8 Databases (AS Level)
syllabus: 9618 (2026)
topics: 8.1 Database Concepts · 8.2 Database Management Systems · 8.3 DDL and DML
---

# Jigsaw — 8 Databases

Syllabus content for **9618 Topic 8**, rebuilt bullet by bullet, with every tested angle mapped onto it.

**Legend**

> [!success] Already examined in 9618
> Tested in a 9618 paper (2021 onwards). Latest question ID given.

> [!warning] 9608 only (not yet in 9618)
> Tested under the old 9608 syllabus, still inside the 9618 syllabus wording. Fair game — just untested in the current series. Latest 9608 question ID given.

> [!info] Not yet tested — inference
> In syllabus, not yet asked in either series (or only asked in a much narrower form). Justification given.

> [!abstract] From the Save My Exams notes
> Content the SME revision notes teach that no past question above covers.

> [!note] This is the biggest chapter in Paper 1
> Databases carries more 9618 questions than any other AS topic: **64 pages** of Database Concepts alone, plus 39 of DDL/DML and 16 of DBMS. It appears as a **whole question (6–15 marks)** in every single paper since 2021, and the question is almost always built the same way: a scenario, a set of table definitions, then parts that walk from E-R diagram → terminology → normalisation → SQL. Learn the shape of the question, not just the content.

---

# 8.1 Database Concepts

## 8.1.1 Limitations of using a file-based approach

> [!success] Explain the benefits of a relational database instead of a file-based approach [3]
> Reduced **data redundancy** // less repeated data … because each item of data is only stored once · **data consistency** is maintained // data integrity is improved … changes in one table automatically update in another … linked data cannot be entered differently in two tables · **program-data independence** is ensured … changes to the data do not require programs to be re-written // queries are not dependent on the structure of the data · **complex queries** are easier to run · different **views** can be provided … so users only see specific aspects of the database · **multiple concurrent access** is possible … through record locking. `9618_w24_qp_12_sc_6.a`

> [!success] Give one limitation of a file-based approach and explain how a relational database addresses it [3]
> *1 mark for the limitation, 2 for the corresponding explanation — the explanation must match the limitation named.*
> **Data redundancy / duplication** → separate linked tables are used; data items are stored once, so duplication is reduced. **Data inconsistency / poor data integrity** → data changed once in one place updates elsewhere; linked data cannot be entered differently in two tables; referential integrity can be enforced. **The data structure depends on the application** → changes to the structure are managed by the DBMS, queries are not dependent on the structure, and changes do not require programs to be re-written. `9618_w24_qp_11_sc_2.a`

> [!success] Identify three advantages of a relational database compared to a file-based approach [3]
> Reduced data **redundancy** · improved data **integrity / consistency / referential integrity** · allows for **views** / improved privacy · allows for **program-data independence** · **complex queries** can be executed. `9618_w23_qp_11_sc_3.b`

> [!success] Explain why a file-based approach is *not* better than a relational database [3]
> The inverted framing. Flat-file has **more data redundancy** … because the same data is stored many times, whereas a database stores it in different linked tables · there is **program-data dependence** with flat files … because any change to the structure of the data means the programs accessing it must be re-written · flat-file has more **data inconsistency** / worse data integrity … because duplicated data might be stored differently, and when data is updated in one place it is not updated everywhere · it is **not easy to perform complex searches** … because a new program has to be written each time · flat files could have a **lack of privacy** … as user views cannot easily be implemented. `9618_s21_qp_11_sc_7.a`

> [!warning] Describe three drawbacks of a file-based approach [6]
> *1 mark per drawback identified, 1 mark for the related description.* The 9608 version is **twice the tariff** of any 9618 version, so each point needs a full expansion: data duplication … the same data is stored multiple times, data changed in one file is not automatically changed in others · data inconsistency … duplicated data might be stored as different values · program-data dependency … if the data structure changes, all programs accessing it must change too · complex searches are hard … a new program has to be written each time · lack of privacy … access controls are usually to the **system** rather than to the **data**. `9608_s21_qp_12_sc_4.a`

> [!warning] Give three limitations of a file-based approach [3]
> Data redundancy // data is repeated in more than one file · data dependency // changes to data means changes to programs accessing that data · lack of data integrity // entries that should be the same can be different in different places · lack of data privacy // **all users have access to all data if a single flat file**. `9608_s19_qp_11_sc_2.b.i`

> [!warning] State what is meant by the term data redundancy [1]
> **Repeated / duplicated data.** A one-mark definition that 9618 has never asked for, despite "reduced data redundancy" being the first credited point in every single 9618 answer on this bullet. `9608_s19_qp_12_sc_5.a.i`

> [!info] The **cost and scale** limitations
> Every mark scheme in both series lists the same five limitations. SME adds **limited scalability** (unsuitable for large volumes or complex relationships), **no central control** (each application manages its own data) and **difficulty of updating** (changes must be made in several places). None of these appears in a 9618 mark scheme, but they follow directly from the credited points.

> [!abstract] Flat file versus relational, with the worked example
> A **flat file** database stores all data in a single table: simple to understand, but it causes data redundancy, inefficient storage and is harder to maintain. A **relational** database organises data into multiple tables and uses **keys** to connect them, which reduces redundancy, uses storage efficiently and is easier to maintain.
> SME's worked example is the cleanest illustration available: a single STUDENT table holding tutor name and form room repeats that tutor's details on every student row. If a tutor changes name, every instance must be found and changed — miss one and the table is inconsistent. Moving the tutor data to its own table and linking with a **TutorID** foreign key stores each tutor once, so one edit updates the whole database.

---

## 8.1.2 Features of a relational database that address those limitations

> [!success] Describe two ways in which a relational database addresses the limitations of a file-based approach [4]
> *Mark in pairs. Max 2 for each description — so two points with expansions, not four bare points.*
> **Reduces data redundancy** … because linked tables mean each data item is stored only once · **reduces program-data dependency** … because the data is separate from the software, so changes to the data do not require programs to be re-written · **reduces data inconsistency / improves data integrity** … because by only storing data once it only needs to be updated once // changes in one table automatically update in another // linked data cannot be entered differently in two tables · **complex queries are easier to run** · **can provide different views** … so users can only see specific aspects of the database. `9618_s23_qp_13_sc_4.a`

> [!warning] Describe the features of a relational database that address the limitations of a file-based system [4]
> *Max 3 from any one group, to max 4 — so the answer must draw on at least two different groups.* **Multiple tables are linked together** … which eliminates data redundancy … increases data integrity/consistency … reduces compatibility issues … so data need only be updated once … and associated data is automatically updated // referential integrity can be enforced. **Program-data independence** … the structure of the data can change without affecting the program, and vice versa. **Concurrent access** … by record locking … restricting over-writing of changes. **Complex queries** can be more easily written. **Access rights** improve security. **Different views** maintain privacy. `9608_w19_qp_12_sc_4.a.i`

> [!warning] Give three reasons why a programmer should use a relational database [6]
> *1 mark per reason, 1 for a further explanation, max three reasons.* The same content as above, but with two extra points 9618 has never credited: **fields can be more easily added to or removed from tables** … without affecting existing applications that do not use those fields · **unwanted or accidental deletion of linked data is prevented, as the DBMS will flag an error**. `9608_w16_qp_12_sc_9.a`

> [!warning] Explain how a relational database reduces data redundancy [3]
> Because each record / piece of data is **stored once and is referenced by a (primary) key** · because data is stored in individual tables … and the tables are linked by relationships · by the proper use of **primary and foreign keys** · by enforcing **referential integrity** · by going through the **normalisation process**. 9618 credits "reduced redundancy" as a bare point but has never asked *how*. `9608_s19_qp_12_sc_5.a.ii`

> [!info] The **ad hoc query** point
> 9608 credits "ability to create **ad hoc** queries" and "the DBMS will have a query language / QBE form". 9618 says only "complex queries are easier to run". The idea that a query can be written *on demand*, without writing a new program, is the sharper version of the same point and is worth having.

---

## 8.1.3 Terminology of the relational database model

> [!success] Define the given database terms [6]
> *1 mark for the definition, 1 mark for an appropriate example from the given database — the example carries half the marks and is where candidates lose them.*
> **Field** — a column / attribute in a table (e.g. `CustomerID` in the table `CUSTOMER`) · **Entity** — anything that data can be stored about (e.g. a customer or a house) · **Foreign key** — a field in one table that is **linked** to a **primary key** in another table (e.g. `CustomerID` in the table `RENTAL`). `9618_s21_qp_12_sc_1.a`

> [!success] Complete the table by writing a definition for each database term [3]
> **Referential integrity** — all duplicate entries of data between tables are consistent // all foreign keys are matched to an appropriate primary key · **Candidate key** — a field that **could** be a primary key but is not // an attribute or smallest set of attributes in a table where no tuple has the same value · **Tuple** — a row / record in a table // one instance of an entity in a table. `9618_w24_qp_11_sc_2.c`

> [!success] State what is meant by entity, primary key and referential integrity [3]
> **Entity** — an object about which data can be stored · **Primary key** — the **unique** attribute / combination of attributes used to identify the **record / tuple** · **Referential integrity** — makes sure that if data is changed in one place the change is reflected in all related records (cascading update/delete) · makes sure that data that does not exist cannot be referenced · ensures every foreign key has a **corresponding** primary key // a logical dependency of a foreign key on a primary key · ensures the data in the database is consistent / up to date · prevents records being added, deleted or modified incorrectly · makes sure any queries return accurate and complete results. `9618_w23_qp_12_sc_2.a`

> [!success] Complete the table of terms and descriptions [4]
> **Entity** ↔ an object that data is stored about · **Tuple** ↔ a row of data in a table about one instance of an object · **Secondary key** ↔ an additional/alternative key used **as well as** the primary key to locate specific data // a candidate key that has not been chosen as a primary key · **Foreign key** ↔ a field in one table that is linked to a primary key in another table. `9618_s23_qp_13_sc_4.b`

> [!success] Define entity and attribute [2]
> **Entity** — a real-life object that is represented as a **table** · **Attribute** — an item of data about an entity. `9618_w24_qp_13_sc_4.d`

> [!success] State what is meant by a candidate key [1]
> An attribute / field (or set of attributes / fields) that **could** be a primary key. `9618_w22_qp_12_sc_5.c`

> [!success] State what is meant by a tuple, and give an example from the table [2]
> *1 mark for the definition, 1 for the example.* **Definition** — a single row in a table. **Example** — a complete row quoted from the table given in the question. `9618_w22_qp_11_sc_4.c.i`

> [!success] Explain what is meant by referential integrity, and how it applies to this database [3]
> *Max 2 generic + max 2 specific — so a purely generic answer caps at 2 marks.*
> **Generic:** referential integrity ensures that related data is consistent · ensures that every **foreign key has a corresponding primary key** · provides for **cascading update / delete** · ensures that if a primary key is deleted or modified, all linked records in the foreign table are deleted or modified // stops **"orphaned records"** — records that point to an entry in another table that no longer exists.
> **Specific:** e.g. `CompanyID` is a foreign key in `PLACEMENT` and is dependent on the primary key `CompanyID` in `COMPANY` · if a record is deleted from `STUDENT`, all records with that `StudentID` will be deleted from `PLACEMENT`. `9618_w25_qp_11_sc_2.d`

> [!success] Explain the reasons why referential integrity is important [3]
> Makes sure data is **consistent** · makes sure all data is **up to date** · ensures every foreign key has a **corresponding** primary key · prevents records from being added / deleted / modified incorrectly · makes sure that if data is changed in one place the change is reflected in all related records · makes sure any **queries return accurate and complete results**. `9618_s23_qp_12_sc_2.b`

> [!success] Describe the relationship between two tables, referring to the primary and foreign keys [2]
> The relationship between `SHIP` and `CONTAINER` is **one-to-many (1:M)** · the primary key `ShipID` in the `SHIP` table is linked to the foreign key `ShipID` in the `CONTAINER` table. Both halves are required — naming the degree alone scores 1. `9618_w25_qp_12_sc_4.a`

> [!success] Identify the relationship between two named tables [1]
> **1-to-many**, or **many-to-1** depending on the direction asked — "there are many performances of each show". Read which table is named first. `9618_s24_qp_12_sc_4.a`; `9618_s24_qp_13_sc_4.a`

> [!success] Identify each relationship between the tables and explain how each is implemented [6]
> *1 mark each to max 6 — so three relationships, each named and then explained.*
> `CUSTOMER` to `JOB` is **1 to many** … implemented by the primary key in `CUSTOMER` being a foreign key in `JOB` · `EMPLOYEE` to `LOGIN_DATA` is **1 to 1** … implemented by the primary key in `EMPLOYEE` being a foreign key in `LOGIN_DATA` · `JOB` to `JOB_EMPLOYEE` is **1 to many** … implemented by the primary key in `JOB` being a foreign key in `JOB_EMPLOYEE` · `EMPLOYEE` to `JOB_EMPLOYEE` is **1 to many** … implemented the same way. The pattern never changes: **name the degree, then say which primary key becomes which foreign key.** `9618_w24_qp_12_sc_6.b.i`

> [!success] Identify two foreign keys and the table each is found in / references [2]
> *1 mark for each field name and table.* e.g. foreign key `BatchID` → table `BATCH`; foreign key `CustomerID` → table `CUSTOMER`. Note the two formats: 9618 asks either for "the table where each **is found**" (`s23_qp_11_sc_2.b.i`) or "the table each foreign key **references**" (`w24_qp_13_sc_4.a`) — answering the wrong one scores nothing. `9618_w24_qp_13_sc_4.a`; `9618_s23_qp_11_sc_2.b.i`

> [!success] Identify two tables that contain foreign keys, and one foreign key in each [2]
> A variant where the **table** is the answer, not the key: e.g. `ORDER_ITEM` → `OrderID`; `ORDER` → `CustomerID`; `CUSTOMER_CARD_DATA` → `CustomerID`. `9618_s25_qp_11_sc_5.c`

> [!success] Identify one attribute that could be a candidate key [1]
> e.g. `CardNumber` in `CUSTOMER_CARD_DATA`. The answer is the attribute that is unique to each record but has **not** been chosen as the primary key. `9618_s25_qp_11_sc_5.b`

> [!success] Complete the table: suitable primary key, a candidate key, and the degree of relationship [3]
> A three-in-one terminology question: a suitable field for the primary key in `COMPANY` → `CompanyID` · a candidate key in `TELESCOPE` → `SerialNumber` // `TelescopeID` · the degree of relationship between `TELESCOPE` and `PHOTOGRAPH` → **1:M / 1 to many**. `9618_w22_qp_13_sc_2.a`

> [!success] Tick one box in each row to identify whether each field is a primary key or a foreign key [2]
> *1 mark for 2 or 3 correct ticks, 2 marks for all 4* — a block-marked question, so one careless row halves it. `MANAGER.ManagerID` → PK · `SHOP.ManagerID` → FK · `CAR.RegistrationNumber` → PK · `CAR.ShopID` → FK. `9618_w21_qp_11_sc_5.a`

> [!success] Underline the attribute(s) that form the primary key in each table [2]
> *1 mark for the three single primary keys, 1 mark for the composite key* — the **composite key carries its own mark**, so a link table must be underlined on both attributes: `CHARACTER_ITEM(CharacterID, ItemName)`. `9618_s25_qp_12_sc_5.b`

> [!success] Give one example of each relationship from the database described [3]
> **one-to-one** — e.g. customer to payment details // customer to login details · **one-to-many** — e.g. customer to order · **many-to-many** — e.g. order to product // customer to product. `9618_s21_qp_11_sc_7.b.i`

> [!success] Tick the relationship that cannot be directly implemented in a normalised relational database [1]
> **Many-to-many.** `9618_s21_qp_11_sc_7.b.ii`

> [!info] **Indexing**
> The syllabus notes name **indexing** in the list of terminology to be understood and used, alongside entity, table, record, field, tuple, attribute, the four key types, the three relationship degrees and referential integrity. Every other item on that list has been examined repeatedly. **Indexing has never appeared in a 9618 question, or in a 9608 one.** It is the single clearest untested term in the chapter: an index is a data structure of ordered key values with pointers to the records, built to speed up searching and sorting on a non-key field, at the cost of extra storage and slower inserts.

> [!info] **Secondary key** asked on its own
> Secondary key appears once, as one row of the `s23_qp_13_sc_4.b` matching table. It has never been the subject of a "state what is meant by" question, unlike primary key, candidate key, foreign key and tuple — all of which have.

> [!info] **Record** and **table** as terms in their own right
> The syllabus lists both. 9618 has examined *tuple*, *attribute*, *field* and *entity* directly, but "define what is meant by a record" or "define a table" has never been set, presumably as too easy. They are the free marks in a definition table if one appears.

> [!abstract] The full terminology table
> **Entity** — a real-world object or concept that data is stored about · **Table** — a collection of data about an entity, in rows and columns · **Record (tuple)** — a single row representing one instance of an entity · **Field (attribute)** — a single column, storing one piece of data about the entity · **Primary key** — a unique identifier for each record · **Candidate key** — a field, or combination of fields, that could be used as a primary key · **Secondary key** — a field used for searching or sorting, but not necessarily unique · **Foreign key** — a field that links to the primary key in another table · **Relationship** — a logical connection between two tables · **Referential integrity** — ensures foreign keys match a primary key in the related table, preventing broken links · **Indexing** — a technique to speed up searching by creating an ordered list of key fields.

---

## 8.1.4 Entity-relationship (E-R) diagrams

> [!success] Complete the E-R diagram for the database [4]
> *1 mark for each correct relationship.* Tariffs run **1 to 4** depending on how many relationships exist: 1 mark (`w23_qp_13_sc_3.b.i`), 2 marks (`w25_qp_11_sc_2.a`), 3 marks (`w25_qp_13_sc_5.a`, `s25_qp_11_sc_5.a`, `w24_qp_11_sc_2.b.i`, `w23_qp_11_sc_3.a`, `w22_qp_11_sc_4.a`, `w21_qp_12_sc_6.a.ii`), 4 marks (`s25_qp_13_sc_6.a`). `9618_s25_qp_13_sc_6.a`
> **The method, every time:** find the foreign keys. A table containing a foreign key is on the **many** side; the table whose primary key it references is on the **one** side. A table whose primary key is **composite, made of two foreign keys**, is a **link table** — it sits on the many side of *both* relationships.

> [!success] Draw an E-R diagram from the given tables [3]
> Some questions give the boxes; others ask you to draw the whole diagram. Marks are for relationships only, never for the boxes. **Max 2 if any extra relationships are drawn** (`s25_qp_11_sc_5.a`) — so do not add a link the foreign keys do not justify. `9618_w21_qp_12_sc_6.a.ii`

> [!success] Complete the E-R diagram where relationships must be named as well as drawn [3]
> `w23_qp_11_sc_3.a` states the answer in words as well as crow's feet: **1:M between CUSTOMER and SHOP_ORDER** · **1:M between SUPPLIER and ITEM** · **1:M between SHOP_ORDER and ORDER_ITEM and M:1 between ORDER_ITEM and ITEM** — the last two count as **one mark together**, because the link table's two relationships are marked as a pair. `9618_w23_qp_11_sc_3.a`

> [!warning] Draw an E-R diagram to document a design described in prose [varies]
> 9608 has **eighteen** questions under this bullet against 9618's nine, and several give only a written description rather than a set of table definitions — the entities must be identified from the prose first. The drawing itself is identical. `9608_w21_qp_11_sc_9.a`; `9608_s18_qp_13_sc_2.a`

> [!info] Reading an E-R diagram **backwards**
> Every 9618 question gives the tables and asks for the diagram. The reverse — given a completed E-R diagram, write the table definitions, or state which table will contain a foreign key — has never been asked in 9618, though it is the same knowledge and is exactly what SME's examiner tip points at: *"when an entity has a 'many' relationship against it, that means it will have a foreign key in it that links to the primary key of the connected entity."*

> [!info] The **crow's foot notation** itself
> No question asks candidates to explain what the notation means, or to label a relationship as 1:1, 1:M or M:N *on* the diagram. Marks are always for the lines. But a mis-drawn crow's foot silently loses the mark, so the three symbols must be automatic.

> [!abstract] Why the diagram matters, in SME's framing
> An E-R diagram tells you two things about a database at a glance: **the names of all the tables**, and **which tables will have a foreign key**. Entities become tables; the relationships decide how they link. One-to-one relationships exist but are uncommon — customer to login details is the standard example. A many-to-many relationship cannot be implemented directly and must be broken with a **link table**.

---

## 8.1.5 The normalisation process

> [!success] Match each Normal Form to its definition [1]
> *1 mark for all three correct — it is all-or-nothing.* **1NF** ↔ there are no repeating groups of attributes · **2NF** ↔ there are no partial dependencies · **3NF** ↔ all fields are fully dependent on the primary key. `9618_s23_qp_11_sc_2.b.ii`

> [!success] Tick one box in each row to identify the stage at which each task happens [2]
> *1 mark for one tick in the correct place, 2 marks for all three.* Remove any **repeating groups of attributes** → 0NF to 1NF · remove any **partial key dependencies** → 1NF to 2NF · remove any **non-key dependencies** → 2NF to 3NF. `9618_w21_qp_12_sc_6.a.i`

> [!success] Describe the characteristics of a database in Third Normal Form [3]
> No **repeating groups** of attributes // data is atomic · no **partial key dependencies** · no **non-key dependencies** // no **transitive dependencies**. Three marks, three lines — the cleanest three marks in the chapter. `9618_w22_qp_11_sc_4.b`

> [!success] Explain how to modify an unnormalised table to put it into 1NF [4]
> Identify **repeating groups of attributes** … naming them from the table (e.g. `Subject` **and** `SubjectCode`) · ensure each field is **atomic** … e.g. `StudentName` should be split into `FirstName` and `LastName` · identify the **primary key** for the table. Both halves of 1NF are needed — atomicity *and* repeating groups — plus the primary key. `9618_w23_qp_12_sc_2.c`

> [!success] Explain the purpose of a link table in a normalised design [2]
> To remove the **many-to-many relationship** · between the two named tables · to allow each X to have many Y // to allow each Y to be linked to many X · by creating a **linking table** · between the two entities. `9618_s25_qp_12_sc_5.a`

> [!success] Explain why the data in one table cannot be stored in another [3]
> Each order would only be able to have **one item** · or the database would **not be normalised** · it would **not be in 1NF** · due to **repeated groups of attributes** · in the `ORDER` table. `9618_s25_qp_11_sc_5.d`

> [!success] Explain how a database that is not in 3NF can be normalised to 3NF [3]
> Two different valid solutions are credited for the same database, which is worth knowing — the mark scheme does not demand one particular decomposition.
> *Solution 1:* remove the many-to-many relationship between `OWNER` and `TREE` … by removing `TreeID` and `TreePosition` from `OWNER` … and creating a **linking table** between them … containing `OwnerID`, `TreeID` and `TreePosition` … with a **composite primary key** of `OwnerID` and `TreeID`, or a new named primary key.
> *Solution 2:* move `TreePosition` into `TREE` … put `OwnerID` into `TREE` … create a new table for the species … containing `ScientificName`, `MaxHeight`, `FastGrowing` … with `ScientificName` as primary key. `9618_w22_qp_12_sc_5.a`

> [!warning] Complete the statements defining the three normal forms [4]
> A cloze version: for **1NF** there must be no **repeating** groups of attributes · for **2NF** it must be in 1NF and contain no **partial** key dependencies · for **3NF** it must be in 2NF and all attributes must be fully dependent on the **primary key**. 9618 has the matching and tick versions but not the cloze. `9608_w19_qp_12_sc_4.a.ii`

> [!warning] Define the three stages of database normalisation [3]
> *Max 1 mark from each bulleted group.* **1NF** — no repeated groups of attributes · all attributes should be **atomic** · **no duplicate rows**. **2NF** — in 1NF and no partial dependencies. **3NF** — in 2NF and no non-key dependencies / no transitive dependencies. The **"no duplicate rows"** point for 1NF is credited in 9608 and appears in **no** 9618 mark scheme. `9608_s18_qp_12_sc_7.c`

> [!warning] Identify three reasons why a given table is not in 1NF [3]
> Applied to a specific table of data, not the abstract definition: there is **no unique primary key** · a named field is **not atomic** // e.g. customer name needs to be split into first name and last name · named fields have **repeated groups of attributes**. The "no unique primary key" reason is the one candidates miss. `9608_s21_qp_12_sc_4.b`

> [!warning] State why a given table is not in 1NF [1]
> The one-mark version, where a single reason from the table will do: the table has a **repeated group of attributes** · each salesperson has a number of products · `FirstName` and `Shop` would need to be repeated for each record. `9608_s15_qp_12_sc_9.a`

> [!info] **Why** normalise at all
> Every question in both series asks *what* the normal forms are, *whether* a table is in them, or *how* to get there. Neither series has ever asked what normalisation **achieves**: eliminating redundancy so each fact is stored once, preventing update, insert and delete anomalies, and guaranteeing data integrity. It is the "explain the purpose" question that has not yet been written for this bullet.

> [!info] **Boyce-Codd** and beyond
> 3NF is the ceiling at AS. Nothing beyond it is examinable, and offering BCNF gains nothing — but knowing that 3NF is *not* the end of the sequence prevents the mistake of claiming a 3NF table is free of every anomaly.

> [!abstract] The three forms, with SME's worked tables
> **1NF** — atomic values (each column holds a single indivisible value), no repeating groups (no arrays or lists in a column), unique column names, and a primary key. *Example:* a `Customers` table with `name` stored as one field and no key is not in 1NF; splitting into `forename` and `surname` and adding `customer_id` puts it in 1NF.
> **2NF** — in 1NF, and **only relevant to tables with a compound primary key**; every non-key attribute must depend on the **whole** key, not part of it. *Example:* a `Course(Course, Date, CourseTitle, Room, Capacity)` table keyed on (Course, Date) — `CourseTitle` depends only on `Course`, so it moves to its own `Course` table, leaving a `Session` table for the time-specific fields.
> **3NF** — in 2NF, with **no transitive dependencies**: no non-key attribute may depend on another non-key attribute. *Example:* `Film(FilmID, Title, Certificate, Description)` — `Description` depends on `Certificate`, not on `FilmID`, so `Certificate` and `Description` move to their own table and `Certificate` becomes a foreign key.
> The mnemonic SME gives is the one worth carrying into the exam: **every field must depend on the key, the whole key, and nothing but the key.**

---

## 8.1.6 Explaining why a set of tables is, or is not, in 3NF

> [!success] Explain why a given database **is** in 3NF [2]
> There are no **repeating groups of attributes** · there are no **many-to-many relationships** · there are no **partial key dependencies** // no non-key dependencies // no transitive dependencies. Note the middle point: "no many-to-many relationships" is credited here and nowhere else. `9618_w25_qp_11_sc_2.b`

> [!success] Tick whether the database is in 3NF or not, and justify using examples from it [2]
> **No mark for the tick — both marks are in the justification, and the justification must quote the database.** All fields in all tables are dependent fully on the primary key and on no other fields · for example, all fields in the `Customer` table are fully dependent on `CustomerID`. `9618_s21_qp_12_sc_1.b`

> [!warning] Explain why a given database is **not** in 3NF, referring to the tables [2]
> This is the harder direction and 9618 has never set it. The answer must **name the offending attribute and say what it depends on**: there are **partial dependencies** in `SOFTWARE_PURCHASED` // `SoftwareDescription` is dependent only on `SoftwareName` and not on both `SoftwareName` and `CustomerID` · there is a **non-key dependency** in `SOFTWARE_PURCHASED` // `LicenceCost` is dependent on `LicenceType`. `9608_s20_qp_12_sc_6.a`

> [!warning] Explain why a named table is not in 3NF [2]
> The compact version: there is a **non-key dependency** · `Manufacturer` is dependent on `ProductName`, which is not the primary key of the `SalesProducts` table. Two lines, and the second must name both attributes. `9608_s15_qp_12_sc_9.c.ii`

> [!warning] Tick true or false for "this database is in 3NF", and justify [3]
> *1 mark for the correct box, then max 2 for the justification* — so here, unlike the 9618 version, **the tick does carry a mark**. No repeated attributes // data is atomic // no partial dependencies (no dual keys) · no non-key / transitive dependencies. `9608_s18_qp_13_sc_2.c`

> [!warning] Give three reasons why a database is fully normalised [3]
> There are no repeating groups (1NF) · there are no partial dependencies (2NF) · there are no non-key dependencies // no transitive dependencies (3NF). One mark per normal form, each labelled. `9608_s19_qp_13_sc_3.d`

> [!info] Explaining **not** in 3NF is the gap
> 9618 has asked this bullet exactly twice, and **both times the answer was that the database *is* in 3NF**. The syllabus wording is "explain why a given set of database tables **are, or are not**, in 3NF" — half of that has never been examined in the current series, and it is the half that requires real analysis: spotting a partial dependency on part of a composite key, or a transitive dependency between two non-key fields. The 9608 mark schemes above are the model answers.

> [!info] Naming the **dependency type** precisely
> The 9608 answers distinguish *partial* (depends on part of a composite key) from *non-key / transitive* (depends on another non-key field). 9618's two questions never required the distinction, because the answer was "it is in 3NF". If the not-in-3NF version appears, using the wrong term for the right observation will cost the mark.

---

## 8.1.7 Producing a normalised database design

> [!success] Create a 3-table design normalised to 3NF, from a written description [6]
> *1 mark each, in pairs: the table with a suitable primary key, then its contents.*
> User table with the **username as the primary key** … containing at least email address, date of birth / age and rating · Quiz table with QuizID or date or filename as the primary key … containing at least the other fields not used as the PK · a **joining table** with an appropriate name including fields for user identification, quiz identification and score … with an appropriate primary key … and **foreign keys matching the primary keys of the other two tables**.
> Model answer: `USER(Username, Email, DateOfBirth, Rating)` / `QUIZ(QuizID, Date, Filename)` / `USER_QUIZ(Username, QuizID, Score)`. `9618_s24_qp_11_sc_6.a`

> [!success] Write a normalised database design for a given unnormalised design, all tables in 3NF [4]
> *1 mark each.* Only **3 tables** with appropriate identifiers (one for customer, one for booking, one for car) · appropriate primary key in each table, **underlined** · the booking table includes the primary key from car and the primary key from customer as **foreign keys** · **all original fields are in the correct tables**.
> Model answer: `BOOKING(BookingID, CarRegistration, CustomerID, StartDate, EndDate)` / `CAR(CarRegistration, CarModel, CarColour)` / `CUSTOMER(CustomerID, CustomerFirstName, CustomerLastName, EmailAddress, TelephoneNumber)`. Note the instruction "use the field names given" — inventing new names loses the last mark. `9618_s23_qp_13_sc_4.c`

> [!success] Normalise one given table, write the new table definitions, and identify the keys [4]
> *1 mark per bullet.* A new table with an **appropriate name** · containing the fields that were repeating · with a **suitable primary key** · and a **foreign key identified in the original table** that links to the new primary key.
> Model: `BATCH(BatchID, IceCreamID, EndDate)` / `ICE_CREAM(IceCreamID, Type, Flavour, Size, SellingPrice)`. The instruction "do not change or include tables X and Y" is part of the question — touching them loses marks. `9618_w24_qp_13_sc_4.c.ii`

> [!success] Describe the additional tables needed and explain how they will be linked [5]
> *1 mark each to max 5.* The pattern is always: name each new table with a suitable primary key · say what other fields it holds · then, for each link, say **which primary key is stored in which table as a foreign key**.
> `s24_qp_13_sc_4.d`: CUSTOMER table with suitable PK … and fields including name and email · BOOKING table with suitable PK … storing the PK of CUSTOMER as an FK … and the PK of PERFORMANCE as an FK · a **linking table between BOOKING and SEAT** with suitable PK … including BOOKING's PK as an FK … storing the SeatID.
> `s24_qp_12_sc_4.d`: STUDENT table with suitable PK · a linking table between STUDENT and EXAM with suitable PK and name … including both PKs as FKs · a linking table between STUDENT and EXAM_QUESTION … storing the ExamQuestionID and the mark for that question. `9618_s24_qp_13_sc_4.d`

> [!warning] Show how given data is redistributed into revised table designs [3]
> A format 9618 has never used: the question gives an unnormalised table of **actual data** and a revised set of table definitions, and the candidate fills in the new tables with the data. Marks are per table (1 for the small table, 2 for the larger). It tests whether normalisation is understood as a data operation, not just a design one. `9608_s15_qp_12_sc_9.b`

> [!warning] Write the table definitions to give the database in 3NF [2]
> The compact version, marked as: 1 mark for correct attributes in the new tables, 1 mark for correct identification of **both** primary keys. Model: `SalesPerson(FirstName, Shop)` / `SalesProducts(FirstName, ProductName, NoOfProducts)` / `Product(ProductName, Manufacturer)`. `9608_s15_qp_12_sc_9.c.iii`

> [!info] Normalising a table of **raw data** rather than a table definition
> The syllabus says a normalised design may be required "for a description of a database, **a given set of data**, or a given set of tables". 9618 has examined the description version (`s24_qp_11_sc_6.a`) and the tables version (`s23_qp_13_sc_4.c`, `w24_qp_13_sc_4.c.ii`) repeatedly — but **never the set-of-data version**, where the raw rows must be read and the entities inferred from them. 9608 did, twice. It is the one-third of this bullet with no 9618 precedent.

> [!info] Choosing between two valid normalisations
> `w22_qp_12_sc_5.a` shows that two different decompositions can both be fully credited. No question has yet asked candidates to **justify** their choice of design, or to compare two given designs — though "explain why your design is in 3NF" is a natural follow-on, and would combine this bullet with 8.1.6.

> [!abstract] The seven-step method
> 1 — Read the scenario or table carefully and work out what **entities** are involved. 2 — Identify the fields and any repeated or duplicated values; these indicate the need for more than one table. 3 — Apply **1NF**: remove repeating groups, split non-atomic fields. 4 — Apply **2NF**: remove partial dependencies. 5 — Apply **3NF**: remove transitive dependencies. 6 — Assign a **primary key** to every table. 7 — Use **foreign keys** to link the related tables, giving referential integrity.
> SME's worked example, which is exactly the shape of `s24_qp_11_sc_6.a`: a table holding `StudentName, StudentID, CourseID, CourseName, TeacherName` becomes `Student(StudentID, StudentName)`, `Course(CourseID, CourseName, TeacherID)`, `Teacher(TeacherID, TeacherName)` and a link table `StudentCourse(StudentID, CourseID)` for the many-to-many.
> Two examiner habits worth copying: **label each stage** (1NF → 2NF → 3NF) so the marker can follow the work, and **watch for composite keys** in link tables.

---

# 8.2 Database Management Systems (DBMS)

## 8.2.1 Features provided by a DBMS

> [!success] Describe what is meant by a data dictionary, and by a logical schema [4]
> *Max 2 for each.*
> **Data dictionary** — data about the data in the database // **metadata** · identifies the **characteristics** of the data that will be stored · plus an appropriate example: field names, table name, validation rules, data types, primary / foreign keys, relationships.
> **Logical schema** — the **conceptual design** · a platform / database **independent** overview of the database · is used to design the **physical structure** · plus an appropriate example: the design of entities, an E-R diagram, views. `9618_s24_qp_11_sc_6.b`

> [!success] State what is meant by a data dictionary and give one example of an item found in it [2]
> *1 mark for the definition, 1 for the example.* **Definition** — data about the data in the database // data about the structure of the database // metadata. **Examples** — table names, data types, field names. `9618_s23_qp_11_sc_2.a.i`

> [!success] Describe the purpose **and** contents of the data dictionary [3]
> *1 mark for the purpose, then 1 mark per example to max 2.* **Purpose** — stores metadata about the database. **Contents** — field / attribute names, table name, validation rules, data types, primary keys // foreign keys, relationships. `9618_w21_qp_12_sc_6.b`

> [!success] Give three items stored in a data dictionary [3]
> Table name · field name // attribute · data type · type of validation · primary key · foreign key · relationships. `9618_s21_qp_11_sc_7.c`

> [!success] Identify three **other** items stored in a data dictionary [3]
> When the question has already given attribute names, table names, foreign keys and primary keys, what remains is: **relationships · views · data types · validation rules**. `9618_s25_qp_13_sc_6.d.i`

> [!success] Describe what is meant by a logical schema [2]
> The **overview of a database structure** · models the problem / situation … by using methods such as an **E-R diagram** · **independent of any particular DBMS**. `9618_w22_qp_12_sc_5.d.ii`

> [!success] Identify the DBMS feature that describes the relationship between data and its structure [1]
> **Logical schema.** `9618_w22_qp_13_sc_2.b`

> [!success] State what is meant by data integrity and give one example of how it is implemented [2]
> *1 mark for the definition, 1 for the example.* **Definition** — methods of making sure the data is **consistent**. **Examples** — enforcing referential integrity · if data in one table is deleted or edited, all tables are updated // cascading update/delete · validation / verification rules. `9618_s23_qp_11_sc_2.a.ii`

> [!success] Explain how a DBMS supports data integrity [3]
> **Referential integrity is enforced** · … such as **cascade update / delete** // if the data is changed in one place it is updated in every other place · … and ensures each foreign key has a corresponding primary key. Note that all three marks here are about referential integrity — this is a narrower answer than the general "data integrity" question. `9618_w24_qp_13_sc_4.e`

> [!success] Give two ways that a DBMS can support data integrity [2]
> **Validation** · enforce **referential integrity** · **cascade update / delete** · ensuring the database is **normalised**. The normalisation point is the one candidates rarely give. `9618_s25_qp_12_sc_5.c.ii`

> [!success] Describe two ways the DBMS can be used to ensure the security of the data [4]
> *1 mark for identification of the method, 1 for the corresponding description.*
> **Authentication methods / passwords / biometrics / 2-factor authentication** … which prevents unauthorised access to the data · **access rights / privileges** can be set … so that only those with the correct permissions can read or edit the data · **regular backups** can be scheduled … so a second copy is available in case of loss or damage · the data can be **encrypted** … so it cannot be understood by anyone who gains unauthorised access · different **views** can be created … so not everyone can see all the data. `9618_w25_qp_13_sc_5.d`

> [!success] Identify two methods the DBMS can use to protect a named table, and explain each [4]
> The same content, applied to a **named table** — every explanation must refer to that table: **access rights** … appropriate permissions for the table `USER` are needed to read or edit the data · a **password** for the database or the `USER` table … prevents users without it from accessing the data · **encrypting the database** … stops users without the decryption key from decoding the data · **views** … users can be given a view that does not include the data in the table `USER`. `9618_s25_qp_12_sc_5.c.i`

> [!success] Describe methods **other than authentication** that a DBMS can use to improve security [4]
> *Max 2 if no descriptions are given* — so bare points cap the answer at half marks.
> **Backup / recovery procedures** … automatically takes copies of the database and stores them off site regularly … so the data can be recovered if lost · **access rights** … different users are given different permissions to different tables … read/write, read only, full access · **views** … different users see different parts of the database … only what they need to see · **record and table locking** … prevents simultaneous access to data … so updates are not lost and data is not overwritten · **encryption** … the data is turned into ciphertext … so it cannot be understood **without a decryption key**. `9618_w23_qp_12_sc_2.b`

> [!success] Describe how access rights can be used to protect the data from unauthorised access [3]
> Access rights give managers / the owner access to different elements · by having different **accounts / logins** · which have different access rights, e.g. read only // no access // read/write · specific **views** can be assigned to each user · e.g. managers can only see the data for their own shop(s). `9618_w21_qp_11_sc_5.b`

> [!warning] Name and describe two security features provided by a DBMS [4]
> *1 mark for naming, 1 for the description.* Access rights // user accounts — restrict actions (e.g. read / read-write) of specific users · **views** — restrict which parts of the database specific users can see · password // biometrics // PIN code — prevents unauthorised access · automatic backup — creates regular copies in case of loss · encryption — data is incomprehensible to unauthorised users. `9608_s19_qp_12_sc_5.b.ii`

> [!warning] Name and describe two security measures protecting data held in a DBMS [4]
> A far wider list than any 9618 mark scheme, because the question is about the whole system rather than DBMS features alone: **physical measures** (locked doors, keypads, biometric scans) · **backup of data** · **disk-mirroring** — all activity is duplicated to a second disk in real time, so if the first fails a complete copy is available · **access rights** · **encryption** · **firewall** · **authentication** · **anti-malware program** · **concurrent access controls // record locking** — closes a record to a second user until the first update is complete, to prevent simultaneous updates being lost. **Disk-mirroring appears in no 9618 mark scheme.** `9608_w17_qp_12_sc_3.b`

> [!warning] Describe two ways the Database Administrator could use DBMS software to ensure security [4]
> *Max 2 marks per method, max 2 methods.* The same five methods as 9618, plus one 9618 never credits: **usage monitoring / logging of activity** … creation of an **audit / activity log** … records the use of the data, all operations performed by all users, all access to the data … e.g. track who changed a student's grade. `9608_s16_qp_12_sc_8.a.ii`

> [!warning] Describe three factors to consider when planning a backup procedure, and justify each [6]
> *1 mark for the procedure point, 1 for the justification, max three procedures.* **How often** should the data be backed up — e.g. at the end of each day … because a student's progress may be edited each day · **what medium** — e.g. an external hard disk … it has large enough capacity · **where** should backups be stored — **off-site** … so if the building is damaged only the original data is lost · **what** is backed up — e.g. only updated files … because there are many files and not all change daily · **when** should it happen — overnight … the system is not likely to be in use · **who** is responsible · make sure the procedure is **written down and understood by staff**. The 9618 syllabus names "backup procedures" explicitly under DBMS data security, and **9618 has never asked about the procedure itself — only that backups happen.** `9608_s16_qp_13_sc_5.b`

> [!warning] Match the DBMS features to their descriptions [3]
> **Data dictionary** ↔ a file or table containing all the details of the database design · **Data security** ↔ methods of protecting the data, including passwords and different access rights for different users · **Data integrity** ↔ data design features to ensure the **validity** of data in the database. (The fourth description — "a model of what the database will look like, although it may not be stored in this way" — is the **logical schema**, the distractor.) `9608_s16_qp_13_sc_5.a`

> [!warning] Name and describe two levels of the schema of a database [4]
> *1 mark for each name, 1 for each matching description, max 2 per level.* **External** — the individual's view(s) of the database · **Conceptual** — describes the data as seen by the applications making use of the DBMS; describes the 'views' users might have · **Physical / Internal** — describes how the data will be stored on the physical media · **Logical** — describes how the relationships will be implemented in the logical structure of the database. The 9618 syllabus names only the **logical schema**; the three-level architecture behind it is 9608 content but explains what "logical" is being contrasted with. `9608_s19_qp_11_sc_2.b.ii`

> [!warning] State what DBMS stands for [1]
> **Database Management System.** A free mark that 9618 has never offered. `9608_s16_qp_12_sc_8.a.i`

> [!info] **Data modelling** as a named feature
> The 9618 syllabus lists five DBMS features: data management including maintaining a data dictionary, **data modelling**, logical schema, data integrity, and data security including backup procedures and access rights. Four of the five are examined repeatedly. **Data modelling has never been the subject of a question in either series** — the closest is the logical schema answer that credits "by using methods such as an E-R diagram". It is the DBMS feature most likely to be asked next.

> [!info] **Backup procedures** in 9618
> Named explicitly in the syllabus notes under data security. 9618 credits "regular backups can be scheduled … so a second copy is available" as one point inside a security question, but has never asked about the backup **procedure** — frequency, medium, location, scope. 9608 set that as a 6-mark question (above).

> [!info] Why a DBMS rather than writing the software yourself
> Every question asks what features a DBMS has. The prior question — why an organisation buys a DBMS instead of building its own file handling — is untested: the features are already built, tested and standardised; multi-user access, security and integrity are handled centrally; and the developer writes queries rather than file-handling code.

> [!abstract] The DBMS, feature by feature, against the file-based problem it solves
> **Data redundancy** → a DBMS centralises data, so it is stored once and referenced when needed. **Data inconsistency** → the DBMS updates a single source of truth. **Data management** → a **data dictionary** defines all data elements across the system (field and table names, data types). **Data modelling** → tools such as E-R diagrams define entities and relationships. **Logical schema** → describes the structure independently of how it is stored. **Data integrity** → constraints such as primary and foreign keys enforce it. **Data security** → user accounts, access rights and permissions for individuals and groups. **Backup procedures** → automated backup and recovery tools reduce the risk of data loss.
> This table is the answer to any "how does a DBMS address the issues of a file-based approach" question, and it maps one-to-one onto the syllabus's own list.

---

## 8.2.2 Software tools found within a DBMS

> [!success] Complete the table of DBMS features and tools [4]
> *1 mark for each correct feature or description.*
> **Data dictionary** ↔ data about the data in the database // data about the structure of the database // metadata for a database · **Query processor** ↔ software that allows the user to enter **criteria**, then finds and returns the appropriate result // software that processes and executes queries **written in SQL** · **Logical schema** ↔ a model of a database that is not specific to one DBMS · **Developer interface** ↔ a software tool that allows the user to create items such as tables, forms and reports. `9618_s23_qp_12_sc_2.a`

> [!success] Describe the purpose of a developer interface [2]
> To allow the user to **create / modify / delete tables** // maintain the database · to set up or modify **relationships** · to create a **form** for data input · to add tools to a form, e.g. drop-down boxes, buttons · to design a **report** to show output in an organised manner · to add a **menu** enabling a choice of different actions · to inspect the database contents and metadata … by creating and/or running different **SQL queries**. `9618_w25_qp_12_sc_4.d`

> [!success] Explain how a database designer can make use of the developer interface [3]
> The same list, framed as usage: to create / modify / delete database objects · to create a form for data input · to add tools to a form · for example, drop-down boxes or buttons · to design a report to show the output in an organised manner · to add a menu to enable users to choose different actions / run different queries. `9618_s25_qp_13_sc_6.d.ii`

> [!success] Describe the purpose of a query processor [2]
> Allows the user to **enter criteria** · **searches for the data** that meets the entered criteria · **organises the results** to be displayed to the user. Three points, two marks — and all three are needed for a reliable answer. `9618_w22_qp_13_sc_2.f`

> [!warning] Identify three tasks that can be performed using the DBMS developer interface [3]
> Create a table · set up **relationships** between tables · create / design a **form** · create / design a **report** · **create / design a query (NOT run a query)**. The bracket is the examiner's own: *designing* a query is the developer interface, *running* it is the query processor. That distinction has never been tested in 9618 and is exactly the kind of trap a new question would set. `9608_s20_qp_13_sc_6.b`

> [!warning] Describe, using examples, how the developer interface and the query processor are used [5]
> *Max 2 per tool plus 1 mark for a suitable example for each.* **Developer interface** — to create user-friendly features, e.g. forms to enter new bookings · to create outputs, e.g. a report of bookings on a given date · to create interactive features, e.g. buttons and menus. **Query processor** — to create SQL/QBE queries · to search for data that meets **set criteria**, e.g. all bookings for next week · to **perform calculations on extracted data**, e.g. the number of empty rooms tomorrow. The calculation point is credited in no 9618 mark scheme. `9608_w19_qp_13_sc_3.b`

> [!warning] Fill in the names of the missing software tools [2]
> A **query processor** allows a developer to extract data from a database · a **developer interface** enables a developer to create user-friendly forms and reports. `9608_s19_qp_12_sc_5.b.iii`

> [!info] The **internal components** of the query processor
> 9618 asks only what the query processor does for the user. SME breaks it into three parts — a **DDL interpreter** (interprets CREATE, ALTER, DROP and updates the data dictionary), a **DML compiler** (compiles SELECT, INSERT, UPDATE into low-level instructions and optimises the query) and a **query evaluation engine** (executes the compiled instructions). This is not in any mark scheme in either series, but it is the natural next level of a bullet that already carries four questions.

> [!info] **Query-by-example (QBE)** against SQL
> 9608 credits "SQL/QBE queries" and "the DBMS will have a query language / QBE form". 9618 never mentions QBE. SME frames the distinction usefully: the developer interface allows queries to be written in **SQL**, which is more flexible than **query-by-example** tools, which are visual and simplified — so SQL allows more complex and precise queries. Untested in 9618, and it links 8.2 directly to 8.3.

> [!abstract] The two tools, in one line each
> **Developer interface** — where the database is *built*: tables, relationships, forms for input, reports for output, menus and buttons, and the place SQL is written. **Query processor** — where the database is *interrogated*: it takes the criteria, searches for matching data, performs any calculations on it, and organises the results for display.

---

# 8.3 Data Definition Language (DDL) and Data Manipulation Language (DML)

> [!note] Where the marks actually are
> Of the 39 pages in the 9618 DDL/DML Legend, **14 are DDL and 22 are DML**. DML is the larger half and the more heavily examined: `SELECT … FROM … WHERE` with a join and an aggregate function appears in **every series**. The DDL half is narrower and much more predictable — `CREATE DATABASE`, `CREATE TABLE` with data types and a primary key, and `ALTER TABLE … ADD`.

## 8.3.1 The DBMS carries out creation and modification of structure using DDL

> [!info] The bullet has **no question of its own**
> The 9618 Legend's page for this bullet is **empty** — the heading is there and no question sits under it. The same is true in 9608 apart from one shared cloze. The understanding is assumed and tested *through* the SQL questions in 8.3.4: DDL is the sub-language that **builds and changes the structure** — databases, tables, fields, data types, keys and relationships — as opposed to the data inside it.

> [!abstract] DDL and DML, side by side
> **DDL** is used to build and manage the **structure** of a relational database: it defines how data is stored, by creating and modifying tables, fields, indexes and relationships. **DML** is used to manage the **data stored within** those structures: adding, updating, deleting and retrieving it. Both use SQL syntax. The one-line summary: **DDL structures the database; DML maintains its contents.**

---

## 8.3.2 The DBMS carries out queries and maintenance of data using DML

> [!info] This bullet also has **no question of its own**
> Empty in the 9618 Legend, as above. It is examined only through the scripts in 8.3.5. The distinction that would be tested, if it were asked directly, is which commands belong to which: `CREATE`, `ALTER`, `DROP` and the key definitions are **DDL**; `SELECT`, `INSERT INTO`, `UPDATE` and `DELETE FROM` are **DML**.

> [!info] Sorting commands into DDL and DML
> A "tick to show whether each statement is DDL or DML" table would test both of the two bullets above at once, in the format 9618 already uses for normalisation stages and for hardware/software interrupts. It has never been set in either series, and it is the obvious way to examine two bullets that currently carry no questions at all.

---

## 8.3.3 SQL as the industry standard for both DDL and DML

> [!success] Identify and correct the errors in a given SQL script [4]
> *1 mark each.* The 9618 model of this question is worth learning as a checklist, because the four errors are the four things candidates get wrong in their own scripts:
> **`SUM` should be `COUNT`** — SUM totals a numeric column, COUNT counts rows · **the WHERE statement needs the table names before each field name** — `WHERE STUDENT.StudentID = LESSON.StudentID`, because the field exists in both tables · **the `OR` should be `AND`** — the conditions must all hold, not any of them · **a string literal is missing its speech marks** — `STUDENT.RiderLevel = "Beginner"`. `9618_s23_qp_12_sc_2.c.iii`

> [!info] Naming SQL, and saying what it is for
> The syllabus bullet is "show understanding that the industry standard for both DDL and DML is Structured Query Language (SQL)", with the note "understand a given SQL statement". The only 9618 question under it is the error-spotting one above. A question asking what SQL stands for, or why an industry standard matters (the same language works across different DBMSs, so skills and scripts transfer), has never been set.

> [!abstract] Reading a given statement
> The "understand a given SQL statement" half of the bullet is best practised backwards: given a script, say in words what it returns. Work through it clause by clause — **SELECT** what columns, **FROM** which tables, joined **how**, filtered by **which conditions**, **grouped** by what, **ordered** how. If the script has a `GROUP BY`, the answer is "one row per group"; if it has an aggregate with no `GROUP BY`, the answer is a single value.

---

## 8.3.4 Writing SQL (DDL) statements

> [!success] Write an SQL script to define a database [1]
> `CREATE DATABASE SHOP;` — one mark, and the whole question. The semicolon and the name from the scenario are all that is needed. `9618_w23_qp_11_sc_3.c.i`; `9618_s21_qp_11_sc_7.b.iii`

> [!success] Write an SQL script to define a table, from sample data [4]
> *1 mark per bullet.* `CREATE TABLE` with **opening and closing brackets** and commas separating the attributes · appropriate data types for the **text** fields · appropriate data types for the **numeric / Boolean / date** fields · **primary key correctly defined**.
> ```sql
> CREATE TABLE STAFF(
>   StaffID INTEGER,
>   StaffFirstName VARCHAR(50),
>   StaffLastName VARCHAR(50),
>   Department CHAR,
>   RemoteWorker BOOLEAN,
>   PRIMARY KEY (StaffID)
> );
> ```
> `PRIMARY KEY (field)` on its own line and `field INTEGER NOT NULL PRIMARY KEY` inline are **both accepted**. `9618_w25_qp_13_sc_5.b`

> [!success] Write an SQL script to define a table, **including constraints** [5]
> The five-mark version adds a mark for constraints and one for the key: `CREATE TABLE` with brackets, all statements within them · the text fields as **varchar or equivalent** · **… with suitable constraint(s)** · the numeric and date fields as decimal / currency / date · **primary key identified**.
> ```sql
> CREATE TABLE BATCH(
>   BatchID VARCHAR(6) NOT NULL,
>   Type VARCHAR(20) NOT NULL,
>   Flavour VARCHAR(20) NOT NULL,
>   Size FLOAT,
>   SellingPrice CURRENCY,
>   EndDate DATE,
>   PRIMARY KEY(BatchID)
> );
> ```
> "Include constraints where appropriate" means **`NOT NULL`** — it is a named mark point, and omitting it costs a mark on every 5-mark version. `9618_w24_qp_13_sc_4.c.i`

> [!success] Write an SQL script to define a table with a **composite primary key** [5]
> Same structure, but the last mark is a **dual primary key**: `PRIMARY KEY (PartID, RepairNumber)`. A link table always takes this form, and writing two separate `PRIMARY KEY` lines is wrong. `9618_w24_qp_11_sc_2.b.ii`

> [!success] Write an SQL script to define a table including a **foreign key** [4]
> *1 mark each:* creating the table with brackets · all four attributes with appropriate data types · setting the primary key · setting the foreign key **referencing the correct table**.
> ```sql
> CREATE TABLE PERFORMANCE(
>   PerformanceID VARCHAR NOT NULL,
>   ShowID VARCHAR,
>   ShowDate DATE,
>   StartTime TIME,
>   PRIMARY KEY(PerformanceID),
>   FOREIGN KEY(ShowID) REFERENCES SHOW(ShowID)
> );
> ```
> `9618_s24_qp_13_sc_4.b`

> [!success] Write an SQL script to define a table, choosing from a restricted list of data types [4]
> When the question lists the supported types (character, varchar, Boolean, integer, real, date, time), the data-type marks are awarded for choosing **from that list** and sizing them sensibly: `BirdID CHAR(4) NOT NULL`, `Name VARCHAR(9)`, `Size VARCHAR(6)`, `PRIMARY KEY (BirdID)`. Sizing a `VARCHAR` to fit the longest value shown in the sample data is the giveaway that the data has been read. `9618_s23_qp_11_sc_2.b.iii`

> [!success] Complete a given DDL statement [4]
> *1 mark per correctly completed line.* A cloze `CREATE TABLE` where the missing pieces are always the same four kinds of thing: the words **`TABLE`** and the table name · a **`VARCHAR(n)`** for a text field · a **`REAL` / `CURRENCY`** for a money field · **`PRIMARY KEY`** before the bracketed field. `9618_s21_qp_12_sc_1.c.i`

> [!success] Write an SQL script to add one field to an existing table [2]
> *1 mark for the `ALTER TABLE` statement, 1 for the field with a suitable name and suitable type.*
> `ALTER TABLE CONTAINER ADD InspectionDate DATE;` `9618_w25_qp_12_sc_4.b`
> The type must match what is being stored — a date for a date, `TEXT`/`VARCHAR(11)` for a resolution such as "1920 × 1068" (`w22_qp_13_sc_2.d`).

> [!success] Write an SQL script to add **two** fields to an existing table [3]
> `ALTER TABLE CAMERA_DATA ADD NumberStored INTEGER, LastUsed DATE;` — marked as three points: the ALTER TABLE line, the first field with its type, and the second field with its type. `9618_w22_qp_11_sc_4.d`

> [!success] Write DDL statements to include a field to store a date [3]
> `ALTER TABLE PURCHASE ADD OrderDate DATE;` — the three marks are the ALTER TABLE, the field name, and a suitable data type. `9618_w21_qp_12_sc_6.c.ii`

> [!success] Write an SQL script to link a foreign key to an existing table [2]
> *1 mark for altering the correct table, 1 for adding the foreign key referencing the correct table.*
> `ALTER TABLE EXAM_QUESTION ADD FOREIGN KEY (ExamID) REFERENCES EXAM(ExamID);` `9618_s24_qp_12_sc_4.c`; `9618_s24_qp_11_sc_6.c.i`
> Note which table is altered: the **table containing the foreign key**, not the one being referenced.

> [!info] `DROP`, and removing a field
> Every 9618 `ALTER TABLE` question **adds**. `ALTER TABLE … DROP` and `DROP TABLE` have never appeared in a 9618 question, and are not in the syllabus's named sub-set (`CREATE DATABASE`, `CREATE TABLE`, `ALTER TABLE`, `PRIMARY KEY`, `FOREIGN KEY`) — so this is correctly untested rather than a gap. Do not offer a `DROP` where an `ALTER` is wanted.

> [!info] Changing an existing field's type
> The syllabus says "change a table definition (ALTER TABLE)". Nine 9618 questions use it to **add**; none uses it to modify an existing field's definition. `ALTER TABLE … MODIFY` is not in the named sub-set either, so the safest reading is that `ADD` is the version examined.

> [!info] `NOT NULL` as a topic in its own right
> "Include constraints on the data that can be entered into each field where appropriate" is a named mark point in the two 5-mark CREATE TABLE questions, yet no question asks **what a constraint is** or **why NOT NULL matters** (it prevents a record being stored with that field empty — essential for a primary key, and a form of validation the DBMS enforces). It is the link between 8.3 and the data-integrity feature in 8.2.

> [!abstract] The DDL command set, with the data types
> `CREATE DATABASE <name>` — creates a new database. `CREATE TABLE <name> ( … )` — creates a table with fields and data types. `ALTER TABLE <name> ADD <field> <type>` — changes an existing table. `PRIMARY KEY (field)` — sets the unique identifier. `FOREIGN KEY (field) REFERENCES Table(Field)` — sets up the relationship.
> The **seven data types named in the syllabus**, and nothing else: **CHARACTER** fixed-length text · **VARCHAR(n)** variable-length text to a maximum of n · **BOOLEAN** true or false · **INTEGER** whole numbers · **REAL** decimal numbers · **DATE** a calendar date · **TIME** a time of day.
> SME's full worked example — a `Students` table, a `Courses` table and an `Enrolments` link table with a composite primary key and two foreign keys — is the exact shape of the 5-mark 9618 questions, and worth being able to write from memory.

---

## 8.3.5 Writing SQL (DML) scripts

> [!success] Write a script with a join, a condition and an ORDER BY [5]
> *1 mark per bullet:* `SELECT` and the correct attributes · `FROM` and the correct tables · **tables joined correctly** · correct condition · correct `ORDER BY` clause.
> ```sql
> SELECT PRODUCT.ProductID, ProductName, ComplaintDetails
> FROM PRODUCT INNER JOIN COMPLAINT
> ON PRODUCT.ProductID = COMPLAINT.ProductID
> WHERE Rating <= 5
> ORDER BY Rating DESC;
> ```
> The `FROM A, B WHERE A.key = B.key` form is **equally credited** — the mark is for joining, not for the keyword. Note `DESC` for descending. `9618_w25_qp_13_sc_5.c`

> [!success] Write a script using COUNT across two joined tables [4]
> *1 mark each:* `SELECT COUNT` statement · using the correct tables · joining the tables · the condition for the name.
> ```sql
> SELECT COUNT(ContainerID)
> FROM CONTAINER, SHIP
> WHERE CONTAINER.ShipID = SHIP.ShipID
> AND ShipName = "Caledonia";
> ```
> `9618_w25_qp_12_sc_4.c`; `9618_s25_qp_12_sc_5.d.i`; `9618_w23_qp_11_sc_3.c.ii`

> [!success] Write a script using COUNT with AS and several conditions [4]
> *1 mark each:* `SELECT COUNT` of any appropriate field · **`AS` and an appropriate name** · `FROM` and correct table and `WHERE` and one correct condition · **two `AND` clauses** with the other two conditions.
> ```sql
> SELECT COUNT(CompanyID) AS TotalPlacements
> FROM PLACEMENT
> WHERE CompanyID = "NEAM"
> AND StudentID = "LDEA01"
> AND Complete = TRUE;
> ```
> Whenever the question says "the total should be given an appropriate name" or "with an appropriate title", the `AS` carries its own mark. `9618_w25_qp_11_sc_2.c.ii`

> [!success] Write a script using SUM with a date range [3]
> *1 mark each:* `SELECT SUM(field)` · `FROM` table and one correct condition · the remaining conditions.
> ```sql
> SELECT SUM(Quantity)
> FROM SALE
> WHERE CustomerID = "0034E"
> AND Date >= #01/01/2023# AND Date <= #31/12/2023#;
> ```
> Dates are wrapped in **`#`**, strings in speech marks. "In the year 2023" needs **two** conditions, not one. `9618_w24_qp_13_sc_4.b`; `9618_w24_qp_12_sc_6.b.ii`; `9618_w24_qp_11_sc_2.b.iii`

> [!success] Write a script using COUNT with GROUP BY [3]
> ```sql
> SELECT PlayerID, COUNT(EventID)
> FROM EVENT
> GROUP BY PlayerID;
> ```
> *Marked as:* selecting the field from the table · counting the other field · **grouping by the first field**. "The number of X **for each** Y" always means `GROUP BY Y`. `9618_s24_qp_11_sc_6.c.ii`

> [!success] Write a script using COUNT, a join and GROUP BY, with a title [4]
> *1 mark each:* selecting `COUNT` of an attribute with a suitable name · `FROM` clause · **joining tables** · **grouping by the title and selecting the title**.
> ```sql
> SELECT SHOW.Title, COUNT(PERFORMANCE.PerformanceID) AS NumberOfShowings
> FROM PERFORMANCE INNER JOIN SHOW
> ON PERFORMANCE.ShowID = SHOW.ShowID
> GROUP BY SHOW.Title;
> ```
> `9618_s24_qp_13_sc_4.c`

> [!success] Write a script using COUNT, a join, a condition and GROUP BY [4]
> The four-clause maximum version of the standard question:
> ```sql
> SELECT CustomerName, COUNT(OrderID) AS NotCollected
> FROM ORDER, CUSTOMER
> WHERE ORDER.CustomerID = CUSTOMER.CustomerID
> AND Collected = FALSE
> GROUP BY CUSTOMER.CustomerID;
> ```
> Note `Collected = FALSE` — a Boolean is compared to `TRUE`/`FALSE`, not to a string. `9618_s25_qp_13_sc_6.c`

> [!success] Write a script using SUM, a join, a condition and GROUP BY [4]
> ```sql
> SELECT CUSTOMER.CustomerID, CUSTOMER.Name, SUM(ORDER.TotalCost) AS TotalOwed
> FROM CUSTOMER INNER JOIN ORDER
> ON CUSTOMER.CustomerID = ORDER.CustomerID
> WHERE ORDER.Paid = FALSE
> GROUP BY CUSTOMER.CustomerID;
> ```
> *Marks:* selecting the three things with an appropriate identifier for the sum · the `FROM` with a suitable join (`ON` **or** `WHERE`) · the `Paid = FALSE` condition **with the correct key word** · the `GROUP BY`. `9618_s25_qp_11_sc_5.e`

> [!success] Write a script using SUM across two joined tables [4]
> ```sql
> SELECT SUM(Quantity)
> FROM ORDER_ITEM, SHOP_ORDER
> WHERE ORDER_ITEM.OrderNo = SHOP_ORDER.OrderNo
> AND SHOP_ORDER.CustomerID = 'HJ231';
> ```
> *1 mark per line, max 4* — the `INNER JOIN … ON` form is equally credited. `9618_w23_qp_11_sc_3.c.ii`

> [!success] Write a script using COUNT with a date condition and AS [4]
> ```sql
> SELECT COUNT(CourseID) AS NumOfCourses
> FROM COURSE_SCHEDULE
> WHERE DateStarted > "09/09/23";
> ```
> Four separate marks: the `SELECT COUNT`, the `AS`, the `FROM`, and the `WHERE`. A single-table query can still be worth four marks if it has four clauses. `9618_w23_qp_13_sc_3.b.ii`

> [!success] Write a script using OR for two alternative values [4]
> ```sql
> SELECT Name
> FROM HORSE
> WHERE HorseLevel = "Intermediate"
> OR HorseLevel = "Beginner";
> ```
> *1 mark each for the SELECT, the FROM, and each of the two conditions.* "X **or** Y" needs the field name repeated on both sides of the `OR` — `WHERE HorseLevel = "A" OR "B"` is wrong. `9618_s23_qp_12_sc_2.c.ii`

> [!success] Write a script using LIKE with a wildcard [4]
> ```sql
> SELECT COUNT(TelescopeID)
> FROM TELESCOPE
> WHERE CompanyID LIKE 'HW%';
> ```
> "begins with" / "starting with" → **`LIKE`** with a trailing wildcard. Both `'HW%'` and `'HW*'` are credited. `9618_w22_qp_13_sc_2.c`; `9618_w22_qp_11_sc_4.c.ii`

> [!success] Complete a partly written SQL script [5]
> The cloze version, marked **1 mark per correctly completed space** — so the tariff is the number of gaps, and they always fall on the same landmarks: the aggregate function, the second table name in the `FROM`, the qualified field name in the `WHERE`, the join condition, and the `GROUP BY`.
> ```sql
> SELECT BIRD_TYPE.Size, COUNT(BIRD_TYPE.BirdID) AS NumberOfBirds
> FROM BIRD_TYPE, BIRD_SEEN
> WHERE BIRD_SEEN.PersonID = "J_123"
> AND BIRD_TYPE.BirdID = BIRD_SEEN.BirdID
> GROUP BY BIRD_TYPE.Size;
> ```
> `9618_s23_qp_11_sc_2.b.iv`

> [!success] Write a script to insert a new record [4]
> *1 mark each:* `INSERT INTO <table>` · `VALUES` with opening and closing brackets · inserting the **string** fields correctly, **including quotation marks**, into the correct fields · inserting the **numeric** fields correctly.
> ```sql
> INSERT INTO PRODUCT (ProductID, ProductName, QuantityInBox, Cost, SupplierID)
> VALUES ("002323", "Blue ball point 2 mm", 50, 5.00, "SFX223");
> ```
> Naming the fields is optional — `INSERT INTO PRODUCT VALUES (...)` is equally credited, but then the **order must match the table definition exactly**. `9618_s25_qp_13_sc_6.b`; `9618_w22_qp_12_sc_5.b`; `9618_w21_qp_11_sc_5.c.ii`

> [!success] Write a script to update existing data [3]
> *1 mark each:* `UPDATE <table>` · `SET` the fields · the `WHERE` condition.
> ```sql
> UPDATE CHARACTER
> SET Level = 3, Money = 10000.00
> WHERE CharacterID = "0002";
> ```
> Two fields are set in **one** `SET` clause, separated by a comma. `9618_s25_qp_12_sc_5.d.ii`

> [!success] Write a script to delete records [2]
> *1 mark each:* `DELETE FROM` and the correct table · the correct condition.
> ```sql
> DELETE FROM PLACEMENT
> WHERE Complete = TRUE;
> ```
> `9618_w25_qp_11_sc_2.c.i`

> [!success] Complete a DML statement using COUNT and GROUP BY [3]
> ```sql
> SELECT COUNT(RegistrationNumber)
> FROM CAR
> GROUP BY ShopID;
> ```
> `9618_w21_qp_11_sc_5.c.i`; `9618_w21_qp_12_sc_6.c.i`

> [!info] **AVG** — named in the syllabus, never examined
> The syllabus names six things a DML query may use: `SELECT … FROM`, `WHERE`, `ORDER BY`, `GROUP BY`, `INNER JOIN`, **`SUM`**, **`COUNT`**, **`AVG`**. `SUM` and `COUNT` appear in almost every paper. **`AVG` has never appeared in a 9618 question, or in a 9608 one.** It is the single clearest untested item in 8.3 — `SELECT AVG(Cost) FROM PRODUCT;` — and it behaves exactly like SUM, including needing an `AS` when the question asks for a title.

> [!info] `ORDER BY` in only one question
> `ORDER BY` is named in the syllabus and appears in exactly **one** 9618 question (`w25_qp_13_sc_5.c`, the most recent series), where it was worth a mark of its own. `ASC` versus `DESC`, and ordering by more than one field, have never been tested. Given it has just appeared for the first time, a second appearance is likely.

> [!info] `INNER JOIN` versus the comma-and-WHERE form
> Every mark scheme accepts both, and most print both as example answers. No question has ever asked candidates to explain what an inner join **does** (returns only the rows where the key matches in both tables). The comma form is safer under pressure, because it puts the join condition in the same place as the other conditions — but the `INNER JOIN … ON` form makes the join explicit and is harder to forget.

> [!info] Queries spanning **more than two** tables
> The syllabus caps this at "(at most two) database tables", and every 9618 question obeys it. The SME example joining three tables is beyond the AS requirement — useful for understanding, not for the exam.

> [!abstract] The DML command set
> **Retrieving:** `SELECT … FROM` chooses the columns and tables · `WHERE` filters on a condition · `ORDER BY … ASC/DESC` sorts the results · `GROUP BY` groups rows sharing a value, so an aggregate returns one row per group · `INNER JOIN … ON` combines rows from two tables on a matching key · `SUM()` totals a numeric column · `COUNT()` counts rows · `AVG()` averages a numeric column.
> **Maintaining:** `INSERT INTO … VALUES (…)` adds a record · `UPDATE … SET … WHERE` modifies existing data · `DELETE FROM … WHERE` removes records.
> **Three habits that protect marks:** qualify every field name with its table (`ORDER.CustomerID`) as soon as two tables are involved; put strings in quotation marks and dates in `#…#`; and give every aggregate an `AS` name whenever the question mentions a title, a name or a heading.
