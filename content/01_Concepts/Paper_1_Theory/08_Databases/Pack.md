---
title: Pack — 8 Databases (AS Level)
syllabus: 9618 (2026)
topics: 8.1 Database Concepts · 8.2 Database Management Systems · 8.3 DDL and DML
pairs with: Jigsaw
---

# Pack — 8 Databases

Question-and-answer mirror of **Jigsaw**. Every concept in Jigsaw appears here as a `!question` with a collapsible `!success` answer.

**How marks are set**

- **9618 |** — the **highest** mark tariff that concept has ever carried in a 9618 paper. Answer points = that tariff **+ 2** spare, newest mark scheme first, older ones filling the gaps.
- **9608 |** — same rule, using 9608 tariffs. Still inside the 9618 syllabus wording, but untested in the current series.
- **Inferred |** — not tested in either series. Tariff estimated from how 9618 marks comparable questions.
- **SME |** — from the Save My Exams notes. Tariff estimated the same way.

One bullet = one mark, unless the bullet begins `…` (an expansion of the point above it).

> [!note] The shape of the question matters as much as the content
> Databases is a **whole question** in every paper since 2021, and it is built the same way each time: a scenario → a set of table definitions → E-R diagram → terminology → normalisation → SQL. Work the parts in that order when you practise, because the later parts depend on reading the table definitions correctly in the first.

---

# 8.1 Database Concepts

## 8.1.1 Limitations of using a file-based approach

> [!question] 9618 | Explain the benefits of using a relational database instead of a file-based approach [3]
> A company stores its data using a file-based approach. Explain the benefits of using a relational database instead.
>
>> [!success]- Answer — 11 points for 3 marks
>> - There is reduced **data redundancy** // less repeated data
>> - … because each item of data is only stored once
>> - **Data consistency** is maintained // data integrity is improved
>> - … changes in one table will automatically update in another
>> - … linked data cannot be entered differently in two tables
>> - **Program-data independence** is ensured
>> - … changes to the data do not require programs to be re-written // queries are not dependent on the structure of the data
>> - **Complex queries** are easier to run
>> - Different **views** can be provided
>> - … so users can only see specific aspects of the database
>> - **Multiple concurrent access** is possible, through **record locking**
>>
>> *Latest: `9618_w24_qp_12_sc_6.a`*

> [!question] 9618 | Give one limitation of a file-based approach and explain how a relational database addresses it [3]
> Give **one** limitation of using a file-based approach to store the data **and** explain how a relational database addresses this limitation.
>
>> [!success]- Answer — 1 mark for the limitation, 2 for the matching explanation
>> - **Data redundancy // data duplication** — separate linked tables are used
>> - … data items are stored once, so duplication / redundancy is reduced
>> - **Data inconsistency // poor data integrity** — data changed once in one place will automatically update elsewhere
>> - … linked data cannot be entered differently in two tables // referential integrity can be enforced
>> - **The data structure used depends on the application** — changes to the data structure are managed by the DBMS
>> - … queries are not dependent on the structure of the data, and changes do not require programs to be re-written
>> - The explanation **must match the limitation named** — a mismatched pair scores 1
>>
>> *Latest: `9618_w24_qp_11_sc_2.a`*

> [!question] 9618 | Identify three advantages of a relational database compared to a file-based approach [3]
> Identify **three** advantages of a relational database compared to a file-based approach.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Reduced data **redundancy**
>> - Improved data **integrity / consistency / referential integrity**
>> - Allows for **views** // improved **privacy**
>> - Allows for **program-data independence**
>> - **Complex queries** can be executed
>>
>> *Latest: `9618_w23_qp_11_sc_3.b`*

> [!question] 9618 | Explain why a file-based approach is not better than a relational database [3]
> Someone claims that a file-based approach is usually better than a relational database. Explain why they are incorrect.
>
>> [!success]- Answer — 10 points for 3 marks
>> - Flat-file has more **data redundancy**
>> - … because the same data is stored many times // data is stored in different tables which are linked
>> - There is **program-data dependence** with flat files
>> - … because any change to the structure of the data means the programs that access it have to be re-written
>> - Flat-file has more **data inconsistency** // worse data integrity
>> - … because duplicated data might be stored differently // because when data is updated in one place it is not updated everywhere
>> - It is not easy to perform **complex searches / queries**
>> - … because a new program has to be written each time
>> - Flat files could have a **lack of privacy**
>> - … as user views cannot easily be implemented
>>
>> *Latest: `9618_s21_qp_11_sc_7.a`. The inverted framing — the answer is the same content, but each point must be phrased as a **fault of the flat file**, not a benefit of the database.*

> [!question] 9608 | Describe three drawbacks of a file-based approach compared to a relational database [6]
> Describe **three** drawbacks of a file-based approach compared to a relational database.
>
>> [!success]- Answer — 1 mark per drawback, 1 for its description, 6 marks
>> - There is **data duplication** // redundant data
>> - … because the same data is stored multiple times // data changed in one file is not automatically changed in others
>> - There could be **data inconsistency** // reduced data integrity
>> - … because duplicated data might be stored as different values
>> - There is **program-data dependency**
>> - … if the data **structure** changes, all the programs accessing that data must be changed too
>> - It is not easy to perform **complex searches / queries**
>> - … a new program has to be written each time
>> - **Lack of privacy**
>> - … as access controls are usually to the **system** rather than to the **data** // user views cannot easily be implemented
>>
>> *Latest: `9608_s21_qp_12_sc_4.a`. Twice the tariff of any 9618 version, so every point needs its expansion — the access-controls-to-the-system point is 9608-only.*

> [!question] 9608 | Give three limitations of a file-based approach [3]
> Give **three** limitations of using a file-based approach to store data.
>
>> [!success]- Answer — 4 points for 3 marks
>> - **Data redundancy** // data is repeated in more than one file
>> - **Data dependency** // changes to data means changes to the programs accessing that data
>> - **Lack of data integrity** // entries that should be the same can be different in different places
>> - **Lack of data privacy** // all users have access to all data if it is a single flat file
>>
>> *Latest: `9608_s19_qp_11_sc_2.b.i`*

> [!question] 9608 | State what is meant by the term data redundancy [1]
> State what is meant by the term **data redundancy**.
>
>> [!success]- Answer — 1 mark
>> - **Repeated / duplicated data**
>> - … the same item of data stored in more than one place
>>
>> *Latest: `9608_s19_qp_12_sc_5.a.i`. A one-mark definition 9618 has never asked for, despite "reduced data redundancy" being the first credited point in every 9618 answer on this bullet.*

> [!question] Inferred | Explain the scale and control limitations of a file-based approach [3]
> Other than data redundancy and inconsistency, explain three limitations of a file-based approach.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **Limited scalability** — not suitable for large volumes of data or complex relationships between data
>> - **No central control** — each application manages its own data, so there is no coordination
>> - **Difficult to update** — changes must be made in several places, increasing time taken and risk of error
>> - **Hard to manage relationships** — related data across files cannot easily be linked (e.g. customers and their orders)
>> - **Poor security** — limited control over who can access or modify each file
>>
>> *Inference: every mark scheme in both series lists the same five limitations. SME adds these, and they follow directly from the credited points — a "state three **other** limitations" question is the standard 9618 way of forcing the less obvious half of a list.*

> [!question] SME | Explain, with an example, why a flat file causes inconsistency [4]
> A school stores each student's tutor name and form room in a single STUDENT table. Explain why this causes problems and how a relational database solves them.
>
>> [!success]- Answer — 6 points for 4 marks
>> - The tutor and form room information **repeats on every student row**, which is inefficient use of storage
>> - If a tutor changed their name, **every instance** of that name would have to be found and changed
>> - … missing any one of them leaves the table with **inconsistent data**
>> - A new **TUTOR table** could be created to store the tutor information
>> - … and the tutor fields removed from the student table
>> - A **foreign key** in the student table (`TutorID`) links each student to their tutor
>> - … so each tutor's details are stored **only once** and one edit updates the whole database
>>
>> *SME's worked example. 9618 marks "explain how a relational database addresses this limitation" at 2–3; the worked version with the fix carries 4.*

---

## 8.1.2 Features of a relational database that address those limitations

> [!question] 9618 | Describe two ways a relational database addresses the limitations of a file-based approach [4]
> Describe **two** ways in which a relational database addresses the limitations of a file-based approach.
>
>> [!success]- Answer — mark in pairs, max 2 for each description, 4 marks
>> - **Reduces data redundancy**
>> - … because linked tables mean each data item is stored only once
>> - **Reduces program-data dependency**
>> - … because the data is separate from the software, so changes to the data do not require programs to be re-written
>> - **Reduces data inconsistency // improves data integrity**
>> - … because by only storing data once it only needs to be updated once // changes in one table will automatically update in another // linked data cannot be entered differently in two tables
>> - **Complex queries are easier to run**
>> - Can provide different **views** … so users can only see specific aspects of the database
>>
>> *Latest: `9618_s23_qp_13_sc_4.a`. "Mark in pairs, max 2 each" means **two points with expansions**, not four bare points — four separate features cap at 2.*

> [!question] 9608 | Describe the features of a relational database that address the limitations of a file-based system [4]
> Describe the features of a relational database that address the limitations of a file-based system.
>
>> [!success]- Answer — max 3 from any one group, to max 4
>> - **Multiple tables are linked together**
>> - … which eliminates / reduces data redundancy and duplication
>> - … and increases data integrity / consistency, reducing compatibility issues
>> - … so data need only be updated once, and associated data is automatically updated // referential integrity can be enforced
>> - **Program-data independence** — the structure of the data can change without affecting the program, and vice versa
>> - **Concurrent access** to data — by record locking, restricting over-writing of changes
>> - **Complex queries** can be more easily written, to find specific data
>> - Different users can be given different **access rights**, improving security, and different **views**, maintaining privacy
>>
>> *Latest: `9608_w19_qp_12_sc_4.a.i`. The capping rule forces the answer to draw on **at least two different groups** — four points about linked tables would only score 3.*

> [!question] 9608 | Give three reasons why a programmer should use a relational database [6]
> Give **three** reasons why a programmer should use a relational database rather than a file-based approach.
>
>> [!success]- Answer — 1 mark per reason, 1 for a further explanation, max three reasons
>> - Reduced data redundancy … data is stored in separate linked tables and only needs to be updated once
>> - Improved data consistency / integrity … associated data is automatically updated, eliminating unproductive maintenance
>> - Complex queries can be more easily written … to search for specific data
>> - **Fields can be more easily added to or removed from tables** … without affecting existing applications that do not use those fields
>> - **Unwanted or accidental deletion of linked data is prevented** … as the DBMS will flag an error
>> - Program-data dependence is overcome … changes to the data design do not require changes to programs
>> - Security is improved … each application only has access to the fields it needs
>> - Allows concurrent access … record locking prevents two users updating the same record at once
>>
>> *Latest: `9608_w16_qp_12_sc_9.a`. The two bolded points appear in **no** 9618 mark scheme.*

> [!question] 9608 | Explain how a relational database reduces data redundancy [3]
> Explain **how** a relational database helps to reduce data redundancy.
>
>> [!success]- Answer — 6 points for 3 marks
>> - Because each record / piece of data is **stored once and is referenced by a (primary) key**
>> - Because data is stored in **individual tables**
>> - … and the tables are **linked by relationships**
>> - By the proper use of **primary and foreign keys**
>> - By enforcing **referential integrity**
>> - By going through the **normalisation** process
>>
>> *Latest: `9608_s19_qp_12_sc_5.a.ii`. 9618 credits "reduced redundancy" as a bare point in five different questions but has never asked **how**.*

> [!question] Inferred | Explain what is meant by an ad hoc query and why it is a benefit [2]
> Explain what is meant by an ad hoc query, and why the ability to write one is a benefit of a relational database.
>
>> [!success]- Answer — 4 points for 2 marks
>> - An **ad hoc query** is one written **on demand**, to answer a question that was not anticipated when the database was designed
>> - The DBMS provides a **query language (SQL) or a QBE form** for writing it
>> - … so no new program has to be written, unlike with a file-based approach
>> - … so the data can be interrogated in any way the user needs, immediately
>>
>> *Inference: 9608 credits "ability to create **ad hoc** queries"; 9618 says only "complex queries are easier to run". The sharper version has never been asked directly in either series.*

---

## 8.1.3 Terminology of the relational database model

> [!question] 9618 | Define the given database terms, with an example from the database [6]
> Give the definition of the terms **field**, **entity** and **foreign key**, using an example from the given database for each.
>
>> [!success]- Answer — 1 mark for the definition, 1 for an appropriate example, 6 marks
>> - **Field** — a column / attribute in a table
>> - … e.g. `CustomerID` in the table `CUSTOMER`
>> - **Entity** — anything that data can be stored about
>> - … e.g. a customer, or a house
>> - **Foreign key** — a field in one table that is **linked** to a **primary key** in another table
>> - … e.g. `CustomerID` / `HouseID` in the table `RENTAL`
>> - The example **must come from the database given** — a generic example scores nothing
>>
>> *Latest: `9618_s21_qp_12_sc_1.a`. Half the marks are in the examples, and that is where candidates lose them.*

> [!question] 9618 | Write a definition for referential integrity, candidate key and tuple [3]
> Complete the table by writing a definition for each of the database terms: referential integrity, candidate key, tuple.
>
>> [!success]- Answer — 1 mark for each correct definition
>> - **Referential integrity** — all duplicate entries of data between tables are consistent // all foreign keys are matched to an appropriate primary key
>> - **Candidate key** — a field that **could** be a primary key but is not // an attribute, or smallest set of attributes, in a table where no tuple has the same value
>> - **Tuple** — a row / record in a table // one instance of an entity in a table
>>
>> *Latest: `9618_w24_qp_11_sc_2.c`*

> [!question] 9618 | State what is meant by entity, primary key and referential integrity [3]
> State what is meant by the following terms in a relational database model: entity, primary key, referential integrity.
>
>> [!success]- Answer — 1 mark for each term, max 3
>> - **Entity** — an object about which data can be stored
>> - **Primary key** — the **unique** attribute / combination of attributes used to identify the **record / tuple**
>> - **Referential integrity** — makes sure that if data is changed in one place the change is reflected in all related records (cascading update / delete)
>> - … makes sure that data that does not exist cannot be referenced
>> - … ensures that every foreign key has a **corresponding** primary key // a logical dependency of a foreign key on a primary key
>> - … ensures that the data in the database is consistent / up to date
>> - … prevents records from being added, deleted or modified incorrectly
>>
>> *Latest: `9618_w23_qp_12_sc_2.a`*

> [!question] 9618 | Complete the table of database terms and descriptions [4]
> Complete the table by writing the missing term or description for each database feature.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - **Entity** ↔ an object that data is stored about
>> - **Tuple** ↔ a row of data in a table about one instance of an object
>> - **Secondary key** ↔ an additional / alternative key used **as well as** the primary key to locate specific data // a candidate key that has not been chosen as a primary key
>> - **Foreign key** ↔ a field in one table that is linked to a primary key in another table
>>
>> *Latest: `9618_s23_qp_13_sc_4.b`. The table alternates: some rows give the term and want the description, others the reverse — read which column is blank.*

> [!question] 9618 | Define entity and attribute [2]
> Complete the table by defining each database term: entity, attribute.
>
>> [!success]- Answer — 1 mark for each definition
>> - **Entity** — a real-life object that is represented as a **table**
>> - **Attribute** — an item of data about an entity
>> - … i.e. a column / field of the table
>>
>> *Latest: `9618_w24_qp_13_sc_4.d`*

> [!question] 9618 | State what is meant by a candidate key [1]
> State what is meant by a **candidate key** in a relational database.
>
>> [!success]- Answer — 1 mark
>> - An attribute / field, or set of attributes / fields, that **could** be a primary key
>> - … i.e. it uniquely identifies a record, but has not been chosen as the primary key
>>
>> *Latest: `9618_w22_qp_12_sc_5.c`. The word "could" is the mark.*

> [!question] 9618 | State what is meant by a tuple, and give an example from the table [2]
> State what is meant by a **tuple**. Give an example of a tuple from the table shown.
>
>> [!success]- Answer — 1 mark for the definition, 1 for the example
>> - **Definition:** a single row in a table
>> - … one instance of the entity the table represents
>> - **Example:** a complete row quoted from the table given, with all its field values
>> - Quoting a single field value, or a column, scores nothing
>>
>> *Latest: `9618_w22_qp_11_sc_4.c.i`*

> [!question] 9618 | Explain what is meant by referential integrity and how it applies to this database [3]
> Explain what is meant by referential integrity, and how it applies to the database given.
>
>> [!success]- Answer — max 2 generic + max 2 specific, 3 marks
>> - **Generic:** referential integrity ensures that related data is **consistent**
>> - … ensures that every **foreign key has a corresponding primary key**
>> - … provides for **cascading update / delete**
>> - … ensures that if a primary key is deleted or modified, all linked records in the foreign table are deleted or modified // stops **"orphaned records"** — records that point to an entry in another table that no longer exists
>> - **Specific:** e.g. `CompanyID` is a foreign key in `PLACEMENT` and is dependent on the primary key `CompanyID` in `COMPANY`
>> - … e.g. if a record is deleted from `STUDENT`, all records with that `StudentID` will be deleted from `PLACEMENT`
>> - … e.g. if a `CompanyID` is modified in `COMPANY`, all records with that `CompanyID` in `PLACEMENT` will also be modified
>>
>> *Latest: `9618_w25_qp_11_sc_2.d`. A purely generic answer **caps at 2** — the named tables and keys are compulsory for the third mark.*

> [!question] 9618 | Explain the reasons why referential integrity is important in a database [3]
> Explain the reasons why referential integrity is important in a database.
>
>> [!success]- Answer — 6 points for 3 marks
>> - Makes sure data is **consistent**
>> - Makes sure all data is **up to date**
>> - Ensures that every foreign key has a **corresponding** primary key
>> - Prevents records from being **added / deleted / modified incorrectly**
>> - Makes sure that if data is changed in one place the change is reflected in all related records
>> - Makes sure any **queries return accurate and complete results**
>>
>> *Latest: `9618_s23_qp_12_sc_2.b`*

> [!question] 9618 | Describe the relationship between two tables, referring to the primary and foreign keys [2]
> Describe the relationship between the two tables. Refer to the primary and foreign keys in your answer.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - The relationship between `SHIP` and `CONTAINER` is **one-to-many (1:M)**
>> - The primary key `ShipID` in the `SHIP` table is linked to the foreign key `ShipID` in the `CONTAINER` table
>> - Both halves are required — naming the degree alone scores 1
>> - The **foreign key sits in the table on the "many" side**, always
>>
>> *Latest: `9618_w25_qp_12_sc_4.a`*

> [!question] 9618 | Identify the relationship between two named tables [1]
> Identify the relationship between the tables PERFORMANCE and SHOW.
>
>> [!success]- Answer — 1 mark
>> - **Many to 1** // there are many performances of each show
>> - Read the **order the tables are named in** — `PERFORMANCE` to `SHOW` is M:1, but `SHOW` to `PERFORMANCE` is 1:M
>> - `EXAM` to `EXAM_QUESTION` is **1-to-many** (`s24_qp_12_sc_4.a`)
>>
>> *Latest: `9618_s24_qp_13_sc_4.a`*

> [!question] 9618 | Identify each relationship between the tables and explain how each is implemented [6]
> Identify each relationship between the database tables **and** explain how each relationship can be implemented in the normalised database.
>
>> [!success]- Answer — 1 mark each to max 6
>> - `CUSTOMER` to `JOB` is **1 to many**
>> - … implemented by the primary key in `CUSTOMER` being a foreign key in `JOB`
>> - `EMPLOYEE` to `LOGIN_DATA` is **1 to 1**
>> - … implemented by the primary key in `EMPLOYEE` being a foreign key in `LOGIN_DATA`
>> - `JOB` to `JOB_EMPLOYEE` is **1 to many**
>> - … implemented by the primary key in `JOB` being a foreign key in `JOB_EMPLOYEE`
>> - `EMPLOYEE` to `JOB_EMPLOYEE` is **1 to many** … implemented the same way
>> - The pattern never changes: **name the degree, then say which primary key becomes which foreign key**
>>
>> *Latest: `9618_w24_qp_12_sc_6.b.i`. The largest terminology question in the chapter — three relationships named and explained.*

> [!question] 9618 | Identify two foreign keys and the table each is found in [2]
> Complete the table by identifying **two** foreign keys and the database table where each is found.
>
>> [!success]- Answer — 1 mark for each field name and table
>> - e.g. `BirdID` → `BIRD_SEEN`; `PersonID` → `BIRD_SEEN`
>> - Both foreign keys may be in the **same table** — that is the usual case for a link table
>> - The other format asks for the table each foreign key **references**: e.g. `BatchID` → `BATCH`, `CustomerID` → `CUSTOMER`
>> - Answering the wrong one of those two scores nothing — read the question wording
>>
>> *Latest: `9618_w24_qp_13_sc_4.a`; `9618_s23_qp_11_sc_2.b.i`*

> [!question] 9618 | Identify two tables that contain foreign keys, and one foreign key in each [2]
> Identify **two** tables in the database that contain one or more foreign keys. Give **one** attribute that is a foreign key in each table.
>
>> [!success]- Answer — 1 mark per row, max 2
>> - `ORDER_ITEM` → `OrderID`
>> - `ORDER` → `CustomerID`
>> - `CUSTOMER_CARD_DATA` → `CustomerID`
>> - Here the **table** is the answer being looked for, not the key — the reverse of the question above
>>
>> *Latest: `9618_s25_qp_11_sc_5.c`*

> [!question] 9618 | Identify one attribute that could be a candidate key [1]
> Identify **one** attribute in the table that could be a candidate key.
>
>> [!success]- Answer — 1 mark
>> - e.g. `CardNumber` in `CUSTOMER_CARD_DATA`
>> - The answer is the attribute that is **unique to each record** but has **not** been chosen as the primary key
>> - The primary key itself is not the answer — it is already the primary key
>>
>> *Latest: `9618_s25_qp_11_sc_5.b`*

> [!question] 9618 | Complete the table: a primary key, a candidate key and a degree of relationship [3]
> Complete the table by writing the correct answer for each item.
>
>> [!success]- Answer — 1 mark for each correct answer
>> - A suitable field for the primary key in `COMPANY` → **`CompanyID`**
>> - A candidate key in `TELESCOPE` → **`SerialNumber`** // `TelescopeID`
>> - The degree of relationship between `TELESCOPE` and `PHOTOGRAPH` → **1:M / 1 to many**
>> - "Degree of relationship" means 1:1, 1:M or M:N — not the name of a key
>>
>> *Latest: `9618_w22_qp_13_sc_2.a`*

> [!question] 9618 | Tick to identify whether each field is a primary key or a foreign key [2]
> Tick one box in each row to identify whether each field is a primary key or a foreign key.
>
>> [!success]- Answer — 1 mark for 2 or 3 correct ticks, 2 marks for all 4
>> - `MANAGER.ManagerID` → **primary key**
>> - `SHOP.ManagerID` → **foreign key**
>> - `CAR.RegistrationNumber` → **primary key**
>> - `CAR.ShopID` → **foreign key**
>> - Block marked — one careless row **halves** the question
>> - The rule: the field is a PK in the table it **identifies**, and an FK in any table that **references** it
>>
>> *Latest: `9618_w21_qp_11_sc_5.a`*

> [!question] 9618 | Underline the attributes that form the primary key in each table [2]
> Underline the attribute, or attributes, that form the primary key in each of the tables.
>
>> [!success]- Answer — 1 mark for the single primary keys, 1 mark for the composite key
>> - `USER(`**`Username`**`, Password, DateOfBirth)`
>> - `CHARACTER(CharacterName, `**`CharacterID`**`, Username, Level, Money)`
>> - `ITEM(`**`ItemName`**`, MinimumLevel, Cost)`
>> - `CHARACTER_ITEM(`**`CharacterID`**`, `**`ItemName`**`)` — the **composite key**
>> - The composite key carries **its own mark** — a link table must be underlined on **both** attributes
>> - Note that the primary key is not always the first attribute listed
>>
>> *Latest: `9618_s25_qp_12_sc_5.b`*

> [!question] 9618 | Give one example of each relationship from the database [3]
> Give **one** example of each of the following relationships from the database described: one-to-one, one-to-many, many-to-many.
>
>> [!success]- Answer — 1 mark for each correct example
>> - **One-to-one** — e.g. customer to payment details // customer to login details
>> - **One-to-many** — e.g. customer to order
>> - **Many-to-many** — e.g. order to product // customer to product
>> - Each example must name **two entities from the scenario given**
>>
>> *Latest: `9618_s21_qp_11_sc_7.b.i`*

> [!question] 9618 | Tick the relationship that cannot be directly implemented [1]
> Tick one box to identify the relationship that cannot be directly implemented in a normalised relational database.
>
>> [!success]- Answer — 1 mark
>> - **Many-to-many**
>> - … it must be broken into two one-to-many relationships using a **link table**
>>
>> *Latest: `9618_s21_qp_11_sc_7.b.ii`*

> [!question] Inferred | Explain what is meant by indexing in a database [3]
> Explain what is meant by **indexing** in a relational database, and give one benefit and one drawback.
>
>> [!success]- Answer — 5 points for 3 marks
>> - An **index** is an ordered list of the values of a chosen field, each with a **pointer** to the record it belongs to
>> - It is created on a field that is frequently **searched or sorted** on
>> - **Benefit:** searching is much faster, because the DBMS looks up the ordered index instead of scanning every record
>> - **Drawback:** the index takes up **extra storage**
>> - **Drawback:** inserting, updating and deleting records is **slower**, because the index must be maintained as well
>>
>> *Inference: **indexing is named in the syllabus terminology list and has never appeared in a question in either series** — while every other term on that list has been examined repeatedly. It is the clearest untested term in the chapter.*

> [!question] Inferred | State what is meant by a secondary key [2]
> State what is meant by a **secondary key** and explain why one would be used.
>
>> [!success]- Answer — 4 points for 2 marks
>> - An **additional / alternative key** used as well as the primary key to locate specific data
>> - … // a candidate key that has **not** been chosen as the primary key
>> - It is used to **search or sort** on a field other than the primary key
>> - … e.g. searching a customer table by surname rather than by CustomerID
>> - It is **not necessarily unique**
>>
>> *Inference: secondary key appears once, as one row of the `s23_qp_13_sc_4.b` matching table. It has never been the subject of a "state what is meant by" question, unlike primary key, candidate key, foreign key and tuple.*

> [!question] Inferred | Define the terms record and table [2]
> Define what is meant by a **record** and by a **table** in a relational database.
>
>> [!success]- Answer — 1 mark each
>> - **Record** — a single row in a table, holding all the data about one instance of the entity // a **tuple**
>> - **Table** — a collection of data about one entity, organised in rows and columns
>> - … each row is a record, each column is a field
>>
>> *Inference: both are named in the syllabus. 9618 has examined *tuple*, *attribute*, *field* and *entity* directly, but never *record* or *table* — presumably as too easy. They are the free marks in any definition table.*

> [!question] SME | State the full database terminology set [6]
> Define each of the following: entity, tuple, attribute, primary key, foreign key, referential integrity.
>
>> [!success]- Answer — 1 mark each, 6 marks
>> - **Entity** — a real-world object or concept that data is stored about (e.g. Student, Book)
>> - **Tuple (record)** — a single row in a table, representing one instance of an entity
>> - **Attribute (field)** — a single column in a table, storing one piece of data about the entity
>> - **Primary key** — a unique identifier for each record in a table
>> - **Foreign key** — a field that links to the primary key in another table, creating a relationship
>> - **Referential integrity** — ensures foreign keys match a primary key in the related table, preventing broken links
>> - **Candidate key** — a field, or combination of fields, that could be used as a primary key
>> - **Secondary key** — a field used for searching or sorting, not necessarily unique
>>
>> *9618's own 6-mark definition question (`s21_qp_12_sc_1.a`) sets the tariff for a full set of terms.*

---

## 8.1.4 Entity-relationship (E-R) diagrams

> [!question] 9618 | Complete the E-R diagram for the database [4]
> Complete the entity-relationship (E-R) diagram for the database, using the table definitions given.
>
>> [!success]- Answer — 1 mark for each correct relationship
>> - **Find the foreign keys first** — they decide every line on the diagram
>> - A table **containing** a foreign key sits on the **many** side of that relationship
>> - The table whose **primary key** it references sits on the **one** side
>> - A table whose primary key is **composite, made of two foreign keys**, is a **link table**
>> - … so it sits on the **many** side of *both* its relationships
>> - Draw the crow's foot at the **many** end — a reversed crow's foot loses the mark silently
>> - Tariffs run 1 to 4, depending on how many relationships exist in the tables given
>>
>> *Latest: `9618_s25_qp_13_sc_6.a` (4 marks). Also 3 marks in `w25_qp_13_sc_5.a`, `s25_qp_11_sc_5.a`, `w24_qp_11_sc_2.b.i`, `w23_qp_11_sc_3.a`, `w22_qp_11_sc_4.a`, `w21_qp_12_sc_6.a.ii`; 2 in `w25_qp_11_sc_2.a`; 1 in `w23_qp_13_sc_3.b.i`.*

> [!question] 9618 | Draw an E-R diagram from the given tables [3]
> Draw an entity-relationship (E-R) diagram for the database described.
>
>> [!success]- Answer — 1 mark per correct relationship, **max 2 if any extra**
>> - Marks are for **relationships only** — never for drawing or labelling the boxes
>> - Draw a line **only** where a foreign key justifies it
>> - **Max 2 if any extra relationships are drawn** (`s25_qp_11_sc_5.a`) — a guessed extra link costs a mark
>> - Worked example (`w21_qp_12_sc_6.a.ii`): `PLANT` 1:M `PURCHASE_ITEM`, `CUSTOMER` 1:M `PURCHASE`, `PURCHASE` 1:M `PURCHASE_ITEM`
>> - `PURCHASE_ITEM(PurchaseID, PlantName, Quantity)` has a composite key of two foreign keys — the link table
>>
>> *Latest: `9618_w21_qp_12_sc_6.a.ii`*

> [!question] 9618 | Complete the E-R diagram where relationships must be named as well as drawn [3]
> Complete the entity-relationship (E-R) diagram for the relational database.
>
>> [!success]- Answer — 1 mark for each correct relationship or **pair** of relationships
>> - **1:M** between `CUSTOMER` and `SHOP_ORDER`
>> - **1:M** between `SUPPLIER` and `ITEM`
>> - **1:M** between `SHOP_ORDER` and `ORDER_ITEM` **and** **M:1** between `ORDER_ITEM` and `ITEM`
>> - … those last two count as **one mark together**, because the link table's two relationships are marked as a pair
>> - So getting one side of a link table right and the other wrong scores **nothing** for that pair
>>
>> *Latest: `9618_w23_qp_11_sc_3.a`*

> [!question] 9608 | Draw an E-R diagram for a database described in prose [3]
> A company's database is described in words. Draw an entity-relationship (E-R) diagram to document the design.
>
>> [!success]- Answer — 1 mark per correct relationship
>> - **Identify the entities from the prose first** — the nouns that data is stored about
>> - Decide each relationship by asking it **both ways**: "can one X have many Y?" and "can one Y have many X?"
>> - Both answers yes → **many-to-many**, which needs a **link table** drawn as a third box
>> - One yes, one no → **one-to-many**, crow's foot at the "many" end
>> - Both no → **one-to-one**
>>
>> *Latest: `9608_w21_qp_11_sc_9.a`; `9608_s18_qp_13_sc_2.a`. 9608 has **eighteen** questions on this bullet against 9618's nine, and several give only a written description rather than table definitions.*

> [!question] Inferred | Read an E-R diagram backwards to produce table definitions [4]
> A completed E-R diagram is shown. Write the table definitions it represents, identifying the primary and foreign keys.
>
>> [!success]- Answer — 6 points for 4 marks
>> - One table per **entity box**, each with a suitable **primary key** underlined
>> - Where an entity has a **crow's foot against it**, that table contains a **foreign key**
>> - … linking to the **primary key of the connected entity**
>> - A box with crow's feet on **both** sides is a **link table**
>> - … with a **composite primary key** made of the two foreign keys
>> - A one-to-one relationship puts the foreign key in **either** table, but only one of them
>>
>> *Inference: every 9618 question gives the tables and asks for the diagram. The reverse has never been asked, though it is the same knowledge — and it is exactly what SME's examiner tip points at.*

> [!question] Inferred | Explain the crow's foot notation [2]
> Explain what the crow's foot notation on an E-R diagram shows.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **plain line end** means "one" — one record of that entity takes part in the relationship
>> - A **crow's foot (branching) end** means "many" — many records of that entity take part
>> - So a line plain at one end and branched at the other is **one-to-many**
>> - Branched at **both** ends is many-to-many, which cannot be implemented directly
>>
>> *Inference: no question asks what the notation means, or to label a relationship 1:1 / 1:M / M:N **on** the diagram — marks are always for the lines. But a mis-drawn crow's foot loses the mark silently, so the symbols must be automatic.*

> [!question] SME | Explain what an E-R diagram tells you about a database [3]
> Explain what information an entity-relationship diagram gives about a database design.
>
>> [!success]- Answer — 5 points for 3 marks
>> - It shows the **names of all the tables** in the database, as the entity boxes
>> - It shows the **relationships** between them, drawn in crow's foot notation
>> - It shows **which tables will contain a foreign key** — any entity with a "many" relationship against it
>> - … that foreign key links to the **primary key** of the connected entity
>> - It shows where a **link table** is needed, to break a many-to-many relationship
>>
>> *SME's framing. 9618 marks E-R work at up to 4, and a 3-mark "explain what it shows" is the untested prose version.*

---

## 8.1.5 The normalisation process

> [!question] 9618 | Match each Normal Form to its definition [1]
> Draw one line from each Normal Form to the most appropriate definition.
>
>> [!success]- Answer — 1 mark for **all three** correct
>> - **1NF** ↔ there are no repeating groups of attributes
>> - **2NF** ↔ there are no partial dependencies
>> - **3NF** ↔ all fields are fully dependent on the primary key
>> - It is **all-or-nothing** — two right and one wrong scores zero
>> - The lines cross: 1NF is not the first definition listed
>>
>> *Latest: `9618_s23_qp_11_sc_2.b.ii`*

> [!question] 9618 | Tick the stage at which each normalisation task happens [2]
> Tick one box in each row to identify the appropriate stage for each task: 0NF to 1NF, 1NF to 2NF, 2NF to 3NF.
>
>> [!success]- Answer — 1 mark for 1 tick correct, 2 marks for all 3
>> - Remove any **repeating groups of attributes** → **0NF to 1NF**
>> - Remove any **partial key dependencies** → **1NF to 2NF**
>> - Remove any **non-key dependencies** → **2NF to 3NF**
>> - Block marked in a generous way here — one correct tick still scores
>>
>> *Latest: `9618_w21_qp_12_sc_6.a.i`*

> [!question] 9618 | Describe the characteristics of a database in Third Normal Form [3]
> The database is normalised and is in Third Normal Form (3NF). Describe the characteristics of a database in 3NF.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - No **repeating groups of attributes** // data is **atomic**
>> - No **partial key dependencies**
>> - No **non-key dependencies** // no **transitive dependencies**
>> - Three marks, three lines — the cleanest three marks in the chapter
>> - A 3NF database is in 2NF, which is in 1NF, so all three apply at once
>>
>> *Latest: `9618_w22_qp_11_sc_4.b`*

> [!question] 9618 | Explain how to modify an unnormalised table to put it into 1NF [4]
> The database table shown is not normalised. Explain how to modify the table to put it into First Normal Form (1NF).
>
>> [!success]- Answer — 1 mark per bullet, max 4
>> - Identify **repeating groups of attributes**
>> - … naming them from the table given, e.g. `Subject` **and** `SubjectCode`
>> - Ensure each field is **atomic**
>> - … e.g. `StudentName` should be split into `FirstName` and `LastName`
>> - Identify the **primary key** for the table
>> - Both halves of 1NF are needed — repeating groups **and** atomicity — plus the key
>>
>> *Latest: `9618_w23_qp_12_sc_2.c`. The fields must be **named from the table**, not described generically.*

> [!question] 9618 | Explain the purpose of a link table in a normalised database [2]
> Explain the purpose of the table CHARACTER_ITEM in the database.
>
>> [!success]- Answer — 1 mark each to max 2
>> - To remove the **many-to-many relationship**
>> - … between the `CHARACTER` and `ITEM` tables
>> - To allow each character to have **many items** // to allow each item to be purchased for **many characters**
>> - … by creating a **linking table**
>> - … between the characters and the items purchased for each one
>>
>> *Latest: `9618_s25_qp_12_sc_5.a`*

> [!question] 9618 | Explain why the data in one table cannot be stored in another [3]
> Explain the reasons why the data in the table ORDER_ITEM cannot be stored in the table ORDER.
>
>> [!success]- Answer — 1 mark each to max 3
>> - Each order would only be able to have **one item**
>> - … or the database would **not be normalised**
>> - … it would **not be in 1NF**
>> - … due to **repeated groups of attributes**
>> - … in the `ORDER` table
>>
>> *Latest: `9618_s25_qp_11_sc_5.d`. Note how finely the marks are split — "it would not be in 1NF" and "due to repeated groups" are **separate** marks.*

> [!question] 9618 | Explain how a database that is not in 3NF can be normalised to 3NF [3]
> The database is **not** in Third Normal Form (3NF). Explain how the database can be normalised to 3NF.
>
>> [!success]- Answer — 1 mark per bullet, max 3; **two different solutions are credited**
>> - *Solution 1:* remove the **many-to-many relationship** between `OWNER` and `TREE`
>> - … by removing `TreeID` and `TreePosition` from the `OWNER` table
>> - … and creating a **linking table** between `OWNER` and `TREE`
>> - … containing `OwnerID`, `TreeID` and `TreePosition`
>> - … with a **composite primary key** of `OwnerID` and `TreeID`, or a new named primary key
>> - *Solution 2:* move `TreePosition` into `TREE`, put `OwnerID` into `TREE`, and create a new table for the species
>> - … containing `ScientificName`, `MaxHeight`, `FastGrowing`, keyed on `ScientificName`
>>
>> *Latest: `9618_w22_qp_12_sc_5.a`. The mark scheme does **not** demand one particular decomposition — any consistent normalisation that removes the fault is credited.*

> [!question] 9608 | Complete the statements defining the three normal forms [4]
> Complete the statements describing the three stages of database normalisation by filling in the missing words.
>
>> [!success]- Answer — 1 mark for each word in the correct position
>> - For a database to be in **1NF** there must be no **repeating** groups of attributes
>> - For a database to be in **2NF**, it must be in 1NF and contain no **partial** key dependencies
>> - For a database to be in **3NF**, it must be in 2NF and all attributes must be fully dependent on the **primary key**
>> - Note "primary key" is **two words for one mark** — both are needed
>>
>> *Latest: `9608_w19_qp_12_sc_4.a.ii`. 9618 has the matching and tick versions of this content but not the cloze.*

> [!question] 9608 | Define the three stages of database normalisation [3]
> The database has been normalised to Third Normal Form (3NF). Define the three stages of database normalisation.
>
>> [!success]- Answer — max 1 mark from each bulleted group
>> - **1NF** — no repeated groups of attributes
>> - … all attributes should be **atomic**
>> - … **no duplicate rows**
>> - **2NF** — in 1NF, and no partial dependencies
>> - **3NF** — in 2NF, and no non-key dependencies // no transitive dependencies
>> - Only **one mark per normal form**, so three points about 1NF still score 1
>>
>> *Latest: `9608_s18_qp_12_sc_7.c`. The **"no duplicate rows"** point for 1NF appears in **no** 9618 mark scheme.*

> [!question] 9608 | Identify three reasons why a given table is not in 1NF [3]
> Identify **three** reasons why the data in the table shown is not in First Normal Form (1NF).
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - There is **no unique primary key**
>> - **Customer name is not atomic** // customer name needs to be split into first name and last name
>> - Named fields have **repeated groups of attributes** — e.g. customer name, date of birth, destination, guide name, trip date
>> - Each reason must be **tied to a named field** in the table given
>> - The **"no primary key"** reason is the one candidates most often miss
>>
>> *Latest: `9608_s21_qp_12_sc_4.b`*

> [!question] 9608 | State why a given table is not in 1NF [1]
> State why the table shown is **not** in First Normal Form (1NF).
>
>> [!success]- Answer — any **one** for 1 mark
>> - The table has a **repeated group of attributes**
>> - Each salesperson has a number of products in one row
>> - `FirstName` and `Shop` would need to be repeated for each record
>>
>> *Latest: `9608_s15_qp_12_sc_9.a`. The one-mark version — a single reason from the table given will do.*

> [!question] Inferred | Explain the purpose of normalisation [3]
> Explain why a database designer normalises a database.
>
>> [!success]- Answer — 5 points for 3 marks
>> - To **eliminate redundancy** — each fact is stored **once**, in one place
>> - … so storage is used efficiently and updating is faster
>> - To prevent **update anomalies** — a value changed in one place cannot disagree with a copy elsewhere
>> - To prevent **insert and delete anomalies** — data about one entity cannot be lost by deleting a record about another
>> - To guarantee **data integrity** and support accurate relationships between tables
>>
>> *Inference: every question in both series asks **what** the normal forms are, **whether** a table is in them, or **how** to get there. Neither series has ever asked what normalisation **achieves**.*

> [!question] SME | Describe each of the three normal forms with an example [6]
> Describe First, Second and Third Normal Form, giving an example of a table that fails each one.
>
>> [!success]- Answer — 8 points for 6 marks
>> - **1NF** — atomic values, no repeating groups, unique column names, and a primary key
>> - … *fails:* a `Customers` table with `name` in one field and no key; fixed by splitting into `forename`/`surname` and adding `customer_id`
>> - **2NF** — in 1NF, and applies only to tables with a **compound primary key**; every non-key attribute depends on the **whole** key
>> - … *fails:* `Course(Course, Date, CourseTitle, Room, Capacity)` keyed on (Course, Date) — `CourseTitle` depends only on `Course`
>> - … fixed by moving `CourseTitle` to its own `Course` table, leaving a `Session` table for the time-specific fields
>> - **3NF** — in 2NF, with **no transitive dependencies**: no non-key attribute depends on another non-key attribute
>> - … *fails:* `Film(FilmID, Title, Certificate, Description)` — `Description` depends on `Certificate`, not on `FilmID`
>> - … fixed by moving `Certificate` and `Description` to their own table, with `Certificate` as a foreign key
>>
>> *The mnemonic worth carrying in: **every field must depend on the key, the whole key, and nothing but the key.***

---

## 8.1.6 Explaining why a set of tables is, or is not, in 3NF

> [!question] 9618 | Explain why a given database is in 3NF [2]
> Explain why the database WORKEXPERIENCE is in Third Normal Form (3NF).
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - There are **no repeating groups of attributes**
>> - There are **no many-to-many relationships**
>> - There are **no partial key dependencies** // no non-key dependencies // no transitive dependencies
>> - The middle point — "no many-to-many relationships" — is credited **here and nowhere else** in the chapter
>>
>> *Latest: `9618_w25_qp_11_sc_2.b`*

> [!question] 9618 | Tick whether the database is in 3NF, and justify using examples from it [2]
> Tick one box to identify whether the database is in Third Normal Form (3NF) or not. Justify your choice using one or more examples from the database.
>
>> [!success]- Answer — **no mark for the tick**; both marks are in the justification
>> - All fields in all tables are **fully dependent on the primary key** and on no other fields
>> - … for example, all fields in the `Customer` table are fully dependent on `CustomerID`
>> - The justification **must quote the database** — a generic statement scores 1 at most
>> - Ticking the right box and writing nothing scores **zero**
>>
>> *Latest: `9618_s21_qp_12_sc_1.b`. The same "no mark for the choice" pattern as the monitoring-vs-control question in Chapter 3.*

> [!question] 9608 | Explain why a given database is not in 3NF, referring to the tables [2]
> Explain why the database is **not** in Third Normal Form (3NF). Refer to the tables in your answer. Do **not** attempt to normalise the tables.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - There are **partial dependencies** in the `SOFTWARE_PURCHASED` table
>> - … `SoftwareDescription` is dependent only on `SoftwareName` and **not on both** `SoftwareName` and `CustomerID`
>> - There is a **non-key dependency** in the `SOFTWARE_PURCHASED` table
>> - … `LicenceCost` is dependent on `LicenceType`
>> - The answer must **name the offending attribute and say what it depends on** — "it has dependencies" scores nothing
>> - "Do not attempt to normalise" is part of the question — offering a fix wastes time and earns nothing
>>
>> *Latest: `9608_s20_qp_12_sc_6.a`. **This is the direction 9618 has never set**, and the model answer for it.*

> [!question] 9608 | Explain why a named table is not in 3NF [2]
> Explain why the SalesProducts table is **not** in Third Normal Form (3NF).
>
>> [!success]- Answer — 2 marks
>> - There is a **non-key dependency**
>> - `Manufacturer` is dependent on `ProductName`, which is **not the primary key** of the `SalesProducts` table
>> - Two lines, and the second must name **both** attributes and say which is not the key
>>
>> *Latest: `9608_s15_qp_12_sc_9.c.ii`*

> [!question] 9608 | Tick true or false for "this database is in 3NF", and justify [3]
> The designer states that the database is in Third Normal Form (3NF). Tick one box to indicate whether this is true or false, then justify your choice.
>
>> [!success]- Answer — 1 mark for the correct box, then max 2 for the justification
>> - **Here the tick does carry a mark**, unlike the 9618 version
>> - No repeated attributes // data is **atomic** // no **partial** dependencies (no dual keys)
>> - No **non-key / transitive** dependencies
>> - Check the two formats carefully: `9618_s21_qp_12_sc_1.b` gives no mark for the tick; this one does
>>
>> *Latest: `9608_s18_qp_13_sc_2.c`*

> [!question] 9608 | Give three reasons why a database is fully normalised [3]
> Give **three** reasons why the EMPLOYEES database is fully normalised.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - There are **no repeating groups** (1NF)
>> - There are **no partial dependencies** (2NF)
>> - There are **no non-key dependencies** // no **transitive dependencies** (3NF)
>> - One mark per normal form, each **labelled with the form it satisfies**
>>
>> *Latest: `9608_s19_qp_13_sc_3.d`*

> [!question] Inferred | Identify which normal form a given table fails, and why [3]
> The table shown is not fully normalised. State the highest normal form it satisfies and explain why it fails the next one.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Check **1NF** first: are all values atomic, are there repeating groups, is there a primary key?
>> - Check **2NF** next — but only if the primary key is **composite**; a single-field key means 2NF is automatic
>> - … it fails 2NF if a non-key attribute depends on **part** of the composite key — a **partial dependency**
>> - Check **3NF** last: does any non-key attribute depend on **another non-key attribute** — a **transitive dependency**
>> - Name the attribute and what it depends on, in both cases — that is where the marks are
>>
>> *Inference: 9618 has asked this bullet twice and **both times the answer was that the database is in 3NF**. The syllabus wording is "are, **or are not**" — half the bullet has no 9618 precedent, and it is the half requiring real analysis.*

> [!question] Inferred | Distinguish a partial dependency from a transitive dependency [2]
> Explain the difference between a partial key dependency and a transitive dependency.
>
>> [!success]- Answer — 4 points for 2 marks
>> - A **partial dependency** is where a non-key attribute depends on only **part of a composite primary key**
>> - … so it can only exist in a table with a **composite** key, and it breaks **2NF**
>> - A **transitive (non-key) dependency** is where a non-key attribute depends on **another non-key attribute**
>> - … rather than directly on the primary key, and it breaks **3NF**
>>
>> *Inference: the 9608 mark schemes distinguish these precisely; 9618's two questions never required it, because the answer was "it is in 3NF". Using the wrong term for the right observation would cost the mark.*

---

## 8.1.7 Producing a normalised database design

> [!question] 9618 | Create a 3-table design normalised to 3NF from a written description [6]
> Create a 3-table design for this database, normalised to Third Normal Form (3NF). Give your design in the format `TableName(PrimaryKey, Field1, Field2, …)`.
>
>> [!success]- Answer — 1 mark each, in pairs, 6 marks
>> - **User table** with the username as the **primary key**
>> - … containing at least email address, date of birth / age and rating
>> - **Quiz table** with QuizID, date or file name as the primary key
>> - … containing at least the other field(s) not used as the primary key
>> - A **joining table** with an appropriate name, including fields for user identification, quiz identification and score
>> - … with an appropriate **primary key**
>> - … and **foreign keys matching the primary keys of the other two tables**
>> - Model answer: `USER(Username, Email, DateOfBirth, Rating)` / `QUIZ(QuizID, Date, Filename)` / `USER_QUIZ(Username, QuizID, Score)`
>>
>> *Latest: `9618_s24_qp_11_sc_6.a`. Marked **in pairs** — the table with its key, then its contents — so a table named without its fields scores 1.*

> [!question] 9618 | Write a normalised database design for a given unnormalised design [4]
> Write a normalised database design for this database. All tables must be in 3NF. Use the field names given and underline the primary key fields.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - Only **3 tables** with appropriate identifiers — one for customer, one for booking, one for car
>> - Appropriate **primary key in each table, underlined**
>> - The booking table includes the primary key from car and the primary key from customer as **foreign keys**
>> - **All original fields are in the correct tables** — none lost, none duplicated
>> - Model: `BOOKING(BookingID, CarRegistration, CustomerID, StartDate, EndDate)` / `CAR(CarRegistration, CarModel, CarColour)` / `CUSTOMER(CustomerID, CustomerFirstName, CustomerLastName, EmailAddress, TelephoneNumber)`
>> - "Use the field names given" is an instruction — **inventing new names loses the last mark**
>>
>> *Latest: `9618_s23_qp_13_sc_4.c`*

> [!question] 9618 | Normalise one given table, write the new definitions and identify the keys [4]
> The table BATCH is not normalised. Normalise it, write the table definitions for your new tables, and identify any primary and foreign keys. Do **not** change or include the other tables.
>
>> [!success]- Answer — 1 mark per bullet, max 4
>> - A new table with an **appropriate name**
>> - … containing the fields that were repeating — e.g. type, flavour, size, selling price
>> - … with a **suitable primary key**
>> - … and a **foreign key identified in the original table** that links to the new primary key
>> - Model: `BATCH(BatchID, IceCreamID, EndDate)` / `ICE_CREAM(IceCreamID, Type, Flavour, Size, SellingPrice)`
>> - "Do not change or include tables X and Y" is part of the question — touching them loses marks
>>
>> *Latest: `9618_w24_qp_13_sc_4.c.ii`*

> [!question] 9618 | Describe the additional tables needed and explain how they will be linked [5]
> Describe the additional tables that will need to be included in the database **and** explain how these tables will be linked.
>
>> [!success]- Answer — 1 mark each to max 5
>> - The pattern is always the same: **name each new table with a suitable primary key**, say what other fields it holds, then for each link say **which primary key is stored in which table as a foreign key**
>> - `s24_qp_13_sc_4.d`: CUSTOMER table with suitable PK … and other suitable fields including name and email
>> - … BOOKING table with suitable PK … that stores the PK of CUSTOMER as an FK to join with CUSTOMER
>> - … and stores the PK of PERFORMANCE as an FK to join with PERFORMANCE
>> - … a **linking table** between BOOKING and SEAT with suitable PK and appropriate name … that includes BOOKING's PK as an FK … and stores the SeatID
>> - `s24_qp_12_sc_4.d`: STUDENT table with suitable PK · a linking table between STUDENT and EXAM with suitable PK and name, including both PKs as FKs · a linking table between STUDENT and EXAM_QUESTION, storing the ExamQuestionID and the mark for that question
>>
>> *Latest: `9618_s24_qp_13_sc_4.d`. Both halves of the command word are marked — **describe** the tables and **explain** the links.*

> [!question] 9608 | Show how given data is redistributed into revised table designs [3]
> Using the data given in the first-attempt table, show how these data are now stored in the revised table designs.
>
>> [!success]- Answer — 1 mark for the small table, 2 for the larger
>> - Copy each **distinct** value of the key field into the first table, once only — no repeats
>> - … e.g. `SalesPerson`: Nick/TX, Sean/BH, John/TX — three rows, not nine
>> - Expand the repeating group into **one row per item** in the second table
>> - … e.g. `SalesProducts`: Nick appears three times, once per product he sold
>> - The key field is **repeated** in the second table, as the foreign key linking back
>> - Every original data value must appear **somewhere**, and no value twice in the same table
>>
>> *Latest: `9608_s15_qp_12_sc_9.b`. A format 9618 has never used — it tests normalisation as a **data** operation, not just a design one.*

> [!question] 9608 | Write the table definitions to give the database in 3NF [2]
> Write the table definitions to give the database in Third Normal Form (3NF).
>
>> [!success]- Answer — 1 mark for correct attributes, 1 for **both** primary keys
>> - `SalesPerson(FirstName, Shop)`
>> - `SalesProducts(FirstName, ProductName, NoOfProducts)` — composite key
>> - … or `SalesProducts(SalesID, FirstName, ProductName, NoOfProducts)` with a new single key
>> - `Product(ProductName, Manufacturer)`
>> - Both primary keys in the two **new** tables must be identified for the second mark
>>
>> *Latest: `9608_s15_qp_12_sc_9.c.iii`*

> [!question] Inferred | Produce a normalised design from a given set of raw data [5]
> A table of sample data is shown. Produce a normalised database design in 3NF from this data, identifying primary and foreign keys.
>
>> [!success]- Answer — 7 points for 5 marks
>> - Read the **rows**, not just the column headings — the entities are visible in which values repeat together
>> - Identify each **entity** — a group of columns whose values always travel together
>> - Create a table per entity, with a **primary key** (an existing unique field, or a new ID)
>> - Split any **non-atomic** field and remove any **repeating group** into its own table
>> - Check for a **transitive dependency** — a column determined by a non-key column
>> - Place a **foreign key** in the table on the "many" side of each relationship
>> - Use a **link table with a composite key** for any many-to-many
>>
>> *Inference: the syllabus says a normalised design may be required "for a description of a database, **a given set of data**, or a given set of tables". 9618 has examined the description and tables versions repeatedly but **never the set-of-data version**. 9608 did, twice.*

> [!question] Inferred | Justify that your normalised design is in 3NF [3]
> Explain why the database design you have produced is in Third Normal Form.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Every field holds a **single atomic value** and there are **no repeating groups**, so it is in 1NF
>> - Every table has a **primary key** that uniquely identifies each record
>> - In any table with a **composite key**, every non-key field depends on the **whole** key, so there are no partial dependencies — 2NF
>> - No non-key field depends on **another non-key field**, so there are no transitive dependencies — 3NF
>> - … each named with an example from the design, e.g. "all fields in CUSTOMER depend only on CustomerID"
>>
>> *Inference: `w22_qp_12_sc_5.a` shows two decompositions both being credited, but no question has yet asked candidates to **justify** their choice — though it is the natural follow-on, and would combine this bullet with 8.1.6.*

> [!question] SME | State the seven-step method for producing a normalised design [4]
> Describe the steps you would follow to produce a normalised database design from a written description.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **1** Read the scenario carefully and work out what **entities** are involved
>> - **2** Identify the fields, and any repeated or duplicated values — these indicate the need for more than one table
>> - **3** Apply **1NF** — remove repeating groups, split non-atomic fields
>> - **4** Apply **2NF** — remove partial dependencies
>> - **5** Apply **3NF** — remove transitive dependencies
>> - **6** Assign a **primary key** to every table
>> - **7** Use **foreign keys** to link the related tables, giving referential integrity
>>
>> *Two examiner habits worth copying: **label each stage** (1NF → 2NF → 3NF) so the marker can follow the work, and **watch for composite keys** in link tables.*

---

# 8.2 Database Management Systems (DBMS)

## 8.2.1 Features provided by a DBMS

> [!question] 9618 | Describe what is meant by a data dictionary and by a logical schema [4]
> Describe what is meant by the following DBMS features: data dictionary, logical schema.
>
>> [!success]- Answer — max 2 for each feature, 4 marks
>> - **Data dictionary** — data about the data in the database // **metadata**
>> - … identifies the **characteristics** of the data that will be stored
>> - … plus an appropriate example: field names, table name, validation rules, data types, primary / foreign keys, relationships
>> - **Logical schema** — the **conceptual design**
>> - … a platform / database **independent** overview of the database
>> - … is used to design the **physical structure**
>> - … plus an appropriate example: the design of entities, an E-R diagram, views
>>
>> *Latest: `9618_s24_qp_11_sc_6.b`*

> [!question] 9618 | State what is meant by a data dictionary and give one example of an item in it [2]
> State what is meant by a data dictionary **and** give **one** example of an item typically found in a data dictionary.
>
>> [!success]- Answer — 1 mark for the definition, 1 for the example
>> - **Definition:** data about the data in the database // data about the structure of the database // **metadata** for a database
>> - **Examples:** table names · data types · field names
>> - The example must be a **kind of metadata**, not an item of the actual data
>>
>> *Latest: `9618_s23_qp_11_sc_2.a.i`*

> [!question] 9618 | Describe the purpose and contents of the data dictionary [3]
> Describe the purpose **and** contents of the data dictionary in the DBMS.
>
>> [!success]- Answer — 1 mark for the purpose, 1 per example to max 2
>> - **Purpose:** stores **metadata** about the database
>> - **Contents:** field / attribute names
>> - … table name
>> - … validation rules
>> - … data types
>> - … primary keys // foreign keys
>> - … relationships
>> - Giving four contents and no purpose caps the answer at 2
>>
>> *Latest: `9618_w21_qp_12_sc_6.b`*

> [!question] 9618 | Give three items that are stored in a data dictionary [3]
> A database has a data dictionary. Give **three** items that are stored in a data dictionary.
>
>> [!success]- Answer — 1 mark per item to max 3
>> - **Table name**
>> - **Field name** // attribute
>> - **Data type**
>> - **Type of validation**
>> - **Primary key**
>> - **Foreign key**
>> - **Relationships**
>>
>> *Latest: `9618_s21_qp_11_sc_7.c`*

> [!question] 9618 | Identify three other items stored in a data dictionary [3]
> The data dictionary stores the attribute names, table names, foreign keys and primary keys. Identify **three other** items stored in a data dictionary.
>
>> [!success]- Answer — 1 mark each to max 3
>> - **Relationships**
>> - **Views**
>> - **Data types**
>> - **Validation rules**
>> - The four already given in the question are excluded — repeating them scores nothing
>>
>> *Latest: `9618_s25_qp_13_sc_6.d.i`*

> [!question] 9618 | Describe what is meant by a logical schema [2]
> Describe what is meant by a **logical schema**.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - The **overview of a database structure**
>> - **Models the problem / situation**
>> - … by using methods such as an **E-R diagram**
>> - **Independent of any particular DBMS**
>>
>> *Latest: `9618_w22_qp_12_sc_5.d.ii`*

> [!question] 9618 | Identify the DBMS feature that describes the relationship between data and its structure [1]
> A DBMS has several features. Identify the feature that describes the relationship between data and its structure.
>
>> [!success]- Answer — 1 mark
>> - **Logical schema**
>> - … not the data dictionary, which stores metadata about individual items rather than the structural model
>>
>> *Latest: `9618_w22_qp_13_sc_2.b`*

> [!question] 9618 | State what is meant by data integrity and give one example of how it is implemented [2]
> State what is meant by **data integrity** and give **one** example of how this is implemented in a database.
>
>> [!success]- Answer — 1 mark for the definition, 1 for the example
>> - **Definition:** methods of making sure the data is **consistent**
>> - **Examples:** enforcing **referential integrity**
>> - … if data in one table is deleted or edited, all tables are updated // **cascading update / delete**
>> - … **validation / verification** rules
>>
>> *Latest: `9618_s23_qp_11_sc_2.a.ii`*

> [!question] 9618 | Explain how a DBMS supports data integrity [3]
> A DBMS supports data integrity. Explain how a DBMS supports data integrity.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - **Referential integrity is enforced**
>> - … such as **cascade update / delete** // if the data is changed in one place it is updated in every other place
>> - … and ensures each **foreign key has a corresponding primary key**
>> - All three marks here are about **referential integrity** — a narrower answer than the general data-integrity question
>>
>> *Latest: `9618_w24_qp_13_sc_4.e`*

> [!question] 9618 | Give two ways that a DBMS can support data integrity [2]
> Give **two** ways that a DBMS can support data integrity.
>
>> [!success]- Answer — 1 mark each to max 2
>> - **Validation**
>> - Enforce **referential integrity**
>> - **Cascade update / delete**
>> - Ensuring the database is **normalised**
>> - The normalisation point is the one candidates rarely give
>>
>> *Latest: `9618_s25_qp_12_sc_5.c.ii`*

> [!question] 9618 | Describe two ways the DBMS can be used to ensure the security of the data [4]
> Describe **two** ways in which the DBMS can be used to ensure the security of the customer data.
>
>> [!success]- Answer — 1 mark for the method, 1 for the corresponding description, max 4
>> - **Authentication methods / passwords / biometrics / 2-factor authentication** can be implemented
>> - … which prevents unauthorised access to the customer's data
>> - **Access rights / privileges** can be set
>> - … so that only those with correct permissions can read / edit the customer's data
>> - **Regular backups** can be scheduled
>> - … so that a second copy of the data is available in case of loss or damage
>> - The data can be **encrypted** … so it cannot be understood by anyone who gains unauthorised access
>> - Different **views** can be created … so that not everyone can see the customer's data
>>
>> *Latest: `9618_w25_qp_13_sc_5.d`. Method **and** description — a list of five methods with no descriptions scores 2.*

> [!question] 9618 | Identify two methods the DBMS can use to protect a named table, and explain each [4]
> Identify **two** methods the DBMS can use to protect the data in the table USER from unauthorised access. Explain how each method protects the data.
>
>> [!success]- Answer — 1 mark for method, 1 for matching explanation
>> - **Access rights** — appropriate permissions for the table `USER` are needed to read or edit the data
>> - **A password** for the database or the `USER` table — prevents users without the password from accessing the data
>> - **Encrypting the database** — stops users without the decryption key from decoding / understanding the data
>> - **Views** — users can be given a view of the database that does not include the data in the table `USER`
>> - Every explanation must **refer to the named table**, not to the database in general
>>
>> *Latest: `9618_s25_qp_12_sc_5.c.i`*

> [!question] 9618 | Describe methods other than authentication that a DBMS can use to improve security [4]
> Authentication is one method a DBMS can use to improve the security of a database. Describe **other** methods a DBMS can use.
>
>> [!success]- Answer — 1 mark per bullet, max 4; **max 2 if no descriptions**
>> - **Backup / recovery procedures** … automatically takes copies of the database and stores them off site on a regular basis … so the data can be recovered if lost
>> - **Use of access rights** … some users are given different access permissions to different tables … read/write, read only, full access
>> - **Views** … different users are able to see different parts of the database … only see what they need to see
>> - **Record and table locking** … prevents simultaneous access to data … so updates are not lost and data is not overwritten
>> - **Encryption** … the data is turned into ciphertext … so it cannot be understood **without a decryption key**
>> - Authentication is **excluded by the question** — offering it scores nothing
>>
>> *Latest: `9618_w23_qp_12_sc_2.b`. Bare points cap the answer at **half marks** — every method needs its description.*

> [!question] 9618 | Describe how access rights can be used to protect data from unauthorised access [3]
> Describe the ways in which access rights can be used to protect the data in the database from unauthorised access.
>
>> [!success]- Answer — 1 mark per bullet, max 3
>> - Access rights give managers / the owner access to **different elements** of the database
>> - … by having different **accounts / logins**
>> - … which have different access rights, e.g. **read only** // no access // read / write
>> - Specific **views** can be assigned to the owner and to the managers
>> - … e.g. managers can only see the data for their own shop(s)
>>
>> *Latest: `9618_w21_qp_11_sc_5.b`*

> [!question] 9608 | Name and describe two security features provided by a DBMS [4]
> Name **and** describe **two** security features provided by a DBMS.
>
>> [!success]- Answer — 1 mark for naming, 1 for the description
>> - **Access rights // user accounts** — restrict actions (e.g. read / read-write) of specific users // unauthorised users cannot access the database
>> - **Views** — restrict which parts of the database specific users can see
>> - **Password // biometrics // PIN code** — prevents unauthorised access
>> - **Automatic backup** — creates regular copies of data in case of loss
>> - **Encryption** — data is incomprehensible to unauthorised users
>>
>> *Latest: `9608_s19_qp_12_sc_5.b.ii`*

> [!question] 9608 | Name and describe two security measures protecting data held in a DBMS [4]
> Name and describe **two** security measures that could be in place to protect the security of the data held in the DBMS.
>
>> [!success]- Answer — 1 mark for the measure, 1 for a corresponding description, max 2 per measure, max 2 measures
>> - **Physical measures** — locked doors, keypads, biometric scans controlling access to the machines
>> - **Backup of data** — regular copies are made, so if the data is corrupted it can be restored
>> - **Disk-mirroring** — all activity is duplicated to a **second disk in real time**, so if the first disk fails a complete copy is available
>> - **Access rights** — different rights for individuals / groups, to stop users editing data they are not permitted to access
>> - **Encryption** — if accessed, the data cannot be understood without the decryption key
>> - **Firewall** — stops unauthorised access / hackers reaching the network
>> - **Anti-malware program** — detects, removes and quarantines viruses and key-loggers, with regular scans
>> - **Concurrent access controls // record locking** — closes a record to a second user until the first update is complete
>>
>> *Latest: `9608_w17_qp_12_sc_3.b`. **Disk-mirroring appears in no 9618 mark scheme**, and the question is about the whole system rather than DBMS features alone.*

> [!question] 9608 | Describe two ways the Database Administrator could use the DBMS to ensure security [4]
> Describe **two** ways in which the Database Administrator (DBA) could use the DBMS software to ensure the security of the data.
>
>> [!success]- Answer — max 2 marks per method, max 2 methods
>> - **Usernames and passwords** … stops unauthorised access to the data … strong passwords, changed regularly
>> - **Access rights / privileges** … so only relevant staff can read or edit certain parts of the data … read only, or full read/write/delete
>> - **Regular / scheduled backups** … in case of loss or damage a copy is available … stored off-site or on a separate device
>> - **Encryption of data** … if accessed it cannot be understood … needs a decryption key
>> - **Definition of different views** … composed of one or more tables … controls the scope of the data accessible to authorised users
>> - **Usage monitoring / logging of activity** … creation of an **audit / activity log** … records all operations performed by all users … e.g. track who changed a student's grade
>>
>> *Latest: `9608_s16_qp_12_sc_8.a.ii`. The **audit log** point is credited in no 9618 mark scheme.*

> [!question] 9608 | Describe three factors to consider when planning a backup procedure, and justify each [6]
> Describe **three** factors to consider when planning a backup procedure for the data. Justify your decisions.
>
>> [!success]- Answer — 1 mark for the procedure point, 1 for the justification, max three procedures
>> - **How often** should the data be backed up — e.g. at the end of each day … because records may be edited each day and should not be lost
>> - **What medium** should be used — e.g. an external hard disk drive … it has large enough capacity
>> - **Where** should the backups be stored — **off-site** … so if the building is damaged only the original data is lost
>> - **What** is backed up — e.g. only updated files … there are a large number of files and they are not all updated each day
>> - **When** should the backup take place — e.g. overnight … the system is not likely to be in use then
>> - **Who** is responsible for performing the backup … otherwise it may not be done
>> - The procedure should be **written down and understood by staff** … otherwise some data may not be backed up
>>
>> *Latest: `9608_s16_qp_13_sc_5.b`. The 9618 syllabus names "backup procedures" explicitly, and **9618 has never asked about the procedure itself — only that backups happen.***

> [!question] 9608 | Match the DBMS features to their descriptions [3]
> Draw a line to match each DBMS feature — data dictionary, data security, data integrity — with its description.
>
>> [!success]- Answer — 1 mark for each correct line
>> - **Data dictionary** ↔ a file or table containing all the details of the database design
>> - **Data security** ↔ methods of protecting the data, including passwords and different access rights for different users
>> - **Data integrity** ↔ data design features to ensure the **validity** of data in the database
>> - The unused fourth description — "a model of what the database will look like, although it may not be stored in this way" — is the **logical schema**, the distractor
>>
>> *Latest: `9608_s16_qp_13_sc_5.a`*

> [!question] 9608 | Name and describe two levels of the schema of a database [4]
> Name **and** describe **two** levels of the schema of a database.
>
>> [!success]- Answer — 1 mark for each name, 1 for each matching description, max 2 per level
>> - **External** — the individual's view(s) of the database
>> - **Conceptual** — describes the data as seen by the applications making use of the DBMS // describes the 'views' which users of the database might have
>> - **Physical / Internal** — describes how the data will be **stored on the physical media**
>> - **Logical** — describes how the **relationships** will be implemented in the logical structure of the database
>>
>> *Latest: `9608_s19_qp_11_sc_2.b.ii`. The 9618 syllabus names only the **logical schema** — but the three-level architecture explains what "logical" is being contrasted with.*

> [!question] 9608 | State what DBMS stands for [1]
> State what DBMS stands for.
>
>> [!success]- Answer — 1 mark
>> - **Database Management System**
>>
>> *Latest: `9608_s16_qp_12_sc_8.a.i`. A free mark 9618 has never offered.*

> [!question] Inferred | Explain what is meant by data modelling in a DBMS [3]
> Explain what is meant by **data modelling** as a feature of a DBMS.
>
>> [!success]- Answer — 5 points for 3 marks
>> - Data modelling is the process of defining the **entities** in the system and the **relationships** between them
>> - The DBMS provides **tools** for this, such as an **E-R diagram** editor
>> - … so the structure can be designed **before** any data is stored
>> - The model produced is **independent of how the data will physically be stored** — it becomes the logical schema
>> - It ensures the design supports the queries the users will need, and that relationships are implemented with the correct keys
>>
>> *Inference: the syllabus lists five DBMS features — data management with a data dictionary, **data modelling**, logical schema, data integrity, data security. Four are examined repeatedly. **Data modelling has never been the subject of a question in either series** — it is the DBMS feature most likely to be asked next.*

> [!question] Inferred | Explain why an organisation uses a DBMS rather than writing its own software [3]
> Explain why an organisation would buy a DBMS rather than write its own file-handling software.
>
>> [!success]- Answer — 5 points for 3 marks
>> - The features are **already built and thoroughly tested** — security, integrity, backup, concurrent access
>> - … so development time and cost are far lower, and there are fewer errors
>> - Developers write **queries** in a standard language rather than file-handling code
>> - **Multi-user access, access rights and record locking** are handled centrally, not re-implemented per application
>> - The DBMS uses **industry standards (SQL)**, so staff skills and scripts transfer between systems
>>
>> *Inference: every question asks what features a DBMS has; the prior question — why buy one at all — is untested in either series.*

> [!question] SME | Describe how a DBMS addresses each limitation of a file-based approach [6]
> Describe how a Database Management System addresses the limitations of a file-based approach.
>
>> [!success]- Answer — 8 points for 6 marks
>> - **Data redundancy** → a DBMS **centralises** the data, so it is stored once and referenced when needed
>> - **Data inconsistency** → the DBMS updates a **single source of truth**, so all users see the same values
>> - **Data management** → a **data dictionary** defines all data elements across the system — field and table names, data types
>> - **Data modelling** → tools such as **E-R diagrams** define the entities and relationships
>> - **Logical schema** → describes the structure **independently of how it is stored**
>> - **Data integrity** → **constraints** such as primary and foreign keys enforce it
>> - **Data security** → **user accounts, access rights and permissions** for individuals and groups
>> - **Backup procedures** → **automated backup and recovery** tools reduce the risk of data loss
>>
>> *This maps one-to-one onto the syllabus's own list of DBMS features, so it answers any "how does a DBMS address the issues of a file-based approach" question.*

---

## 8.2.2 Software tools found within a DBMS

> [!question] 9618 | Complete the table of DBMS features and tools [4]
> Complete the table by writing down the missing names and descriptions of DBMS features and tools.
>
>> [!success]- Answer — 1 mark for each correct feature or description
>> - **Data dictionary** ↔ data about the data in the database // data about the structure of the database // metadata for a database
>> - **Query processor** ↔ software that allows the user to enter **criteria**, then finds and returns the appropriate result // software that processes and executes queries **written in SQL**
>> - **Logical schema** ↔ a model of a database that is not specific to one DBMS
>> - **Developer interface** ↔ a software tool that allows the user to create items such as tables, forms and reports
>> - Two rows give the name and want the description; two give the description and want the name
>>
>> *Latest: `9618_s23_qp_12_sc_2.a`*

> [!question] 9618 | Describe the purpose of a developer interface in a DBMS [2]
> Describe the purpose of a developer interface in a Database Management System (DBMS).
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - To allow the user to **create / modify / delete tables** // maintain the database
>> - To allow the user to set up / modify **relationships**
>> - To allow the user to create a **form** for data input
>> - To allow a user to add tools to a form — for example, drop-down boxes or buttons
>> - To allow a user to design a **report**, to show the output in an organised manner
>> - To allow a user to add a **menu**, to enable a choice of different actions
>> - To allow a user to inspect the database contents and metadata … by creating and/or running different **SQL queries**
>>
>> *Latest: `9618_w25_qp_12_sc_4.d`*

> [!question] 9618 | Explain how a database designer can make use of the developer interface [3]
> The DBMS provides a developer interface. Explain how a database designer can make use of it.
>
>> [!success]- Answer — 1 mark each to max 3
>> - To **create / modify / delete database objects**
>> - To create a **form** for data input
>> - To add **tools** to a form
>> - … for example, drop-down boxes or buttons
>> - To design a **report**, to show the output in an organised manner
>> - To add a **menu**, to enable users to choose different actions / run different queries
>>
>> *Latest: `9618_s25_qp_13_sc_6.d.ii`*

> [!question] 9618 | Describe the purpose of a query processor in a DBMS [2]
> Describe the purpose of a query processor in a DBMS.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - Allows the user to **enter criteria**
>> - **Searches for the data** that meets the entered criteria
>> - **Organises the results** to be displayed to the user
>> - Three points, two marks — but all three are worth writing, since any two score
>>
>> *Latest: `9618_w22_qp_13_sc_2.f`*

> [!question] 9608 | Identify three tasks that can be performed using the DBMS developer interface [3]
> Identify **three** tasks that can be performed using the DBMS developer interface.
>
>> [!success]- Answer — 1 mark per task to max 3
>> - **Create a table**
>> - **Set up relationships** between tables
>> - **Create / design a form**
>> - **Create / design a report**
>> - **Create / design a query** — **but NOT run a query**
>> - The bracket is the examiner's own: **designing** a query is the developer interface, **running** it is the query processor
>>
>> *Latest: `9608_s20_qp_13_sc_6.b`. That distinction has never been tested in 9618 and is exactly the trap a new question would set.*

> [!question] 9608 | Describe, using examples, how the developer interface and query processor are used [5]
> Describe, using examples, how a business can use the following DBMS tools: developer interface, query processor.
>
>> [!success]- Answer — max 2 per tool, plus 1 mark for a suitable example for each
>> - **Developer interface:** to create **user-friendly features** — e.g. forms to enter new bookings
>> - … to create **outputs** — e.g. a report of bookings on a given date
>> - … to create **interactive features** — e.g. buttons and menus
>> - **Query processor:** to create **SQL / QBE queries**
>> - … to search for data that meets **set criteria** — e.g. all bookings for next week
>> - … to **perform calculations on extracted data** — e.g. the number of empty rooms tomorrow
>> - The **calculation** point is credited in no 9618 mark scheme
>>
>> *Latest: `9608_w19_qp_13_sc_3.b`*

> [!question] 9608 | Name the missing DBMS software tools [2]
> Fill in the names of the missing software tools: a ______ allows a developer to extract data from a database; a ______ enables a developer to create user-friendly forms and reports.
>
>> [!success]- Answer — 1 mark per bullet
>> - Extracting data from a database → **query processor**
>> - Creating user-friendly forms and reports → **developer interface**
>>
>> *Latest: `9608_s19_qp_12_sc_5.b.iii`*

> [!question] Inferred | Describe the internal components of the query processor [3]
> Describe the components of the query processor in a DBMS.
>
>> [!success]- Answer — 5 points for 3 marks
>> - **DDL interpreter** — interprets Data Definition Language commands such as `CREATE`, `ALTER` and `DROP`
>> - … and **updates the data dictionary** with the resulting structure
>> - **DML compiler** — compiles Data Manipulation Language statements such as `SELECT`, `INSERT`, `UPDATE` into low-level instructions
>> - … and **optimises** the query so it runs efficiently
>> - **Query evaluation engine** — executes the compiled instructions to retrieve or manipulate the actual data
>>
>> *Inference: 9618 asks only what the query processor does for the user. SME's three-part breakdown is in no mark scheme in either series, but it is the natural next level of a bullet that already carries four questions.*

> [!question] Inferred | Compare SQL with query-by-example [2]
> Explain the difference between writing a query in SQL and using a query-by-example (QBE) tool.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **QBE** is a **visual, simplified** tool — the user fills in criteria on a grid or form
>> - … which is quicker and easier for a non-specialist, but limited in what it can express
>> - **SQL** is written as text, so it is **more flexible**
>> - … allowing more **complex and precise** queries to search, update or manage the data
>>
>> *Inference: 9608 credits "SQL/QBE queries" and "the DBMS will have a query language / QBE form"; 9618 never mentions QBE. It links 8.2 directly to 8.3.*

> [!question] SME | State the purpose of each DBMS software tool in one line [2]
> State the purpose of the developer interface and of the query processor.
>
>> [!success]- Answer — 1 mark each
>> - **Developer interface** — where the database is **built**: tables, relationships, forms for input, reports for output, menus and buttons, and where SQL is written
>> - **Query processor** — where the database is **interrogated**: it takes the criteria, searches for matching data, performs calculations on it, and organises the results for display
>>
>> *The one-line version of both tools; 9618 marks each at 2 when asked separately.*

---

# 8.3 Data Definition Language (DDL) and Data Manipulation Language (DML)

> [!note] Where the marks actually are
> Of the 39 pages in the 9618 DDL/DML Legend, **14 are DDL and 22 are DML**. DML is the larger and more heavily examined half: `SELECT … FROM … WHERE` with a join and an aggregate appears in **every series**. DDL is narrower and far more predictable — `CREATE DATABASE`, `CREATE TABLE` with data types and a key, and `ALTER TABLE … ADD`.

## 8.3.1–8.3.2 DDL and DML as concepts

> [!question] Inferred | Explain the difference between DDL and DML [3]
> Explain the difference between Data Definition Language (DDL) and Data Manipulation Language (DML).
>
>> [!success]- Answer — 5 points for 3 marks
>> - **DDL** is used to build and manage the **structure** of a relational database
>> - … it defines how data is stored, by creating and modifying **tables, fields, indexes and relationships**
>> - **DML** is used to manage the **data stored within** those structures
>> - … it deals with **adding, updating, deleting and retrieving** data
>> - Both use **SQL** syntax, and both are carried out by the DBMS
>> - The one-line summary: **DDL structures the database; DML maintains its contents**
>>
>> *Inference: **both syllabus bullets have completely empty pages in the Legend** — no question has ever been set on either, in either series. The understanding is assumed and tested only through the SQL questions.*

> [!question] Inferred | Sort SQL commands into DDL and DML [4]
> Tick one box in each row to show whether each SQL command belongs to DDL or DML.
>
>> [!success]- Answer — 1 mark per pair of rows, 4 marks
>> - `CREATE DATABASE` → **DDL**
>> - `CREATE TABLE` → **DDL**
>> - `ALTER TABLE` → **DDL**
>> - `PRIMARY KEY` / `FOREIGN KEY` definitions → **DDL**
>> - `SELECT … FROM` → **DML**
>> - `INSERT INTO` → **DML**
>> - `UPDATE … SET` → **DML**
>> - `DELETE FROM` → **DML**
>>
>> *Inference: a tick table would test both empty bullets at once, in a format 9618 already uses for normalisation stages and for hardware/software interrupts. It is the obvious way to examine two bullets that currently carry no questions at all.*

---

## 8.3.3 SQL as the industry standard

> [!question] 9618 | Identify and correct the errors in a given SQL script [4]
> The SQL script should return the number of riders with the rider level beginner who have a lesson booked on 09/09/2023. There are **four** errors in the script. Identify **and** correct each error.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - **`SUM` should be `COUNT`** — SUM totals a numeric column, COUNT counts rows … `SELECT COUNT(STUDENT.RiderLevel)`
>> - **The WHERE statement needs the table names before each field name** … `WHERE STUDENT.StudentID = LESSON.StudentID`
>> - **The `OR` should be `AND`** … `AND Date = #09/09/2023#`
>> - **The string is missing its speech marks** … `STUDENT.RiderLevel = "Beginner";`
>> - Each mark needs **both** halves — identifying the error and writing the correction
>> - These four are also the four things candidates get wrong in their **own** scripts, so use them as a checklist
>>
>> *Latest: `9618_s23_qp_12_sc_2.c.iii`*

> [!question] Inferred | State what SQL is and why an industry standard matters [2]
> State what SQL stands for and explain why it is useful that it is an industry standard.
>
>> [!success]- Answer — 4 points for 2 marks
>> - **Structured Query Language**
>> - It is the standard for **both DDL and DML**, so one language both defines the structure and manipulates the data
>> - Because it is an **industry standard**, the same statements work across different DBMSs
>> - … so scripts and staff skills **transfer** between systems, and training is not tied to one product
>>
>> *Inference: the only 9618 question under this bullet is the error-spotting one. The syllabus note "understand a given SQL statement" has never been asked as a definition.*

> [!question] Inferred | Explain in words what a given SQL statement returns [3]
> State what the following SQL script returns: `SELECT CUSTOMER.Name, COUNT(OrderID) AS Total FROM CUSTOMER INNER JOIN ORDER ON CUSTOMER.CustomerID = ORDER.CustomerID WHERE Paid = FALSE GROUP BY CUSTOMER.CustomerID;`
>
>> [!success]- Answer — 5 points for 3 marks
>> - It returns the **customer's name** and a **count of their orders**, under the heading `Total`
>> - … from the `CUSTOMER` and `ORDER` tables, **joined** on `CustomerID`
>> - … for orders that have **not been paid** for
>> - … with **one row per customer**, because of the `GROUP BY`
>> - Work the clauses in order: SELECT **what**, FROM **which tables**, joined **how**, filtered by **which conditions**, grouped by **what**
>> - A `GROUP BY` means "one row per group"; an aggregate with no `GROUP BY` means a **single value**
>>
>> *Inference: the syllabus says "understand a given SQL statement", and the only question under that bullet asks for error correction rather than interpretation.*

---

## 8.3.4 Writing SQL (DDL) statements

> [!question] 9618 | Write an SQL script to define a database [1]
> Write a Structured Query Language (SQL) script to define the database called SHOP.
>
>> [!success]- Answer — 1 mark
>> ```sql
>> CREATE DATABASE SHOP;
>> ```
>> - The name from the scenario and the **semicolon** are all that is needed
>> - `CREATE DATABASE SHOPORDERS;` for `s21_qp_11_sc_7.b.iii`
>>
>> *Latest: `9618_w23_qp_11_sc_3.c.i`; `9618_s21_qp_11_sc_7.b.iii`*

> [!question] 9618 | Write an SQL script to define a table, from sample data [4]
> Some example data from the table STAFF is shown. Write a Structured Query Language (SQL) script to define the table STAFF.
>
>> [!success]- Answer — 1 mark per bullet, max 4
>> - `CREATE TABLE` with **opening and closing brackets** and **commas** separating the attributes
>> - Appropriate data types for the **text** fields
>> - Appropriate data types for the **numeric / Boolean** fields
>> - **Primary key correctly defined**
>> ```sql
>> CREATE TABLE STAFF(
>>   StaffID INTEGER,
>>   StaffFirstName VARCHAR(50),
>>   StaffLastName VARCHAR(50),
>>   Department CHAR,
>>   RemoteWorker BOOLEAN,
>>   PRIMARY KEY (StaffID)
>> );
>> ```
>> - `PRIMARY KEY (field)` on its own line **and** `StaffID INTEGER NOT NULL PRIMARY KEY` inline are **both accepted**
>> - Read the sample data to choose types: "Yes/No" → `BOOLEAN`, a single letter → `CHAR`
>>
>> *Latest: `9618_w25_qp_13_sc_5.b`*

> [!question] 9618 | Write an SQL script to define a table, including constraints [5]
> Write an SQL script to define the table BATCH. Include constraints (restrictions) on the data that can be entered into each field where appropriate.
>
>> [!success]- Answer — 1 mark for each bullet, 5 marks
>> - `CREATE TABLE BATCH` with opening and closing brackets, **all statements within the brackets**
>> - The text fields as **varchar or equivalent**
>> - … **with suitable constraint(s)**
>> - The numeric and date fields as **decimal / currency / date** as appropriate
>> - **Primary key identified**
>> ```sql
>> CREATE TABLE BATCH(
>>   BatchID VARCHAR(6) NOT NULL,
>>   Type VARCHAR(20) NOT NULL,
>>   Flavour VARCHAR(20) NOT NULL,
>>   Size FLOAT,
>>   SellingPrice CURRENCY,
>>   EndDate DATE,
>>   PRIMARY KEY(BatchID)
>> );
>> ```
>> - "Include constraints where appropriate" means **`NOT NULL`** — it is a named mark point, and omitting it costs a mark on every 5-mark version
>>
>> *Latest: `9618_w24_qp_13_sc_4.c.i`*

> [!question] 9618 | Write an SQL script to define a table with a composite primary key [5]
> The table shows sample data for the table REPAIR_PART. Write an SQL script to define it, including constraints where appropriate.
>
>> [!success]- Answer — 1 mark for each bullet, 5 marks
>> - `CREATE TABLE REPAIR_PART` with brackets, all statements inside them
>> - The two ID fields as **varchar (or equivalent)**
>> - The quantity as **integer**
>> - At least **1 appropriate constraint**
>> - **Dual / composite primary key**
>> ```sql
>> CREATE TABLE REPAIR_PART(
>>   PartID VARCHAR(20) NOT NULL,
>>   RepairNumber VARCHAR(4) NOT NULL,
>>   Quantity INT NOT NULL,
>>   PRIMARY KEY (PartID, RepairNumber)
>> );
>> ```
>> - A link table always takes this form — **one `PRIMARY KEY` line naming both fields**, never two separate lines
>>
>> *Latest: `9618_w24_qp_11_sc_2.b.ii`*

> [!question] 9618 | Write an SQL script to define a table including a foreign key [4]
> Sample data for the table PERFORMANCE is shown. Write a Structured Query Language (SQL) script to define the table PERFORMANCE.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - Creating the table with **opening and closing brackets**
>> - Setting **all four attributes with appropriate data types**
>> - Setting `PerformanceID` as the **primary key**
>> - Setting `ShowID` as a **foreign key referencing the SHOW table**
>> ```sql
>> CREATE TABLE PERFORMANCE(
>>   PerformanceID VARCHAR NOT NULL,
>>   ShowID VARCHAR,
>>   ShowDate DATE,
>>   StartTime TIME,
>>   PRIMARY KEY(PerformanceID),
>>   FOREIGN KEY(ShowID) REFERENCES SHOW(ShowID)
>> );
>> ```
>> - Note `DATE` and `TIME` as **separate types** — the sample data shows a date column and a time column
>>
>> *Latest: `9618_s24_qp_13_sc_4.b`*

> [!question] 9618 | Write an SQL script to define a table from a restricted list of data types [4]
> The database only supports these data types: character, varchar, Boolean, integer, real, date, time. Write an SQL script to define the table BIRD_TYPE.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - `CREATE TABLE` start **and end bracket**
>> - `BirdID` as **CHAR / VARCHAR**
>> - `Name` **and** `Size` as **VARCHAR / CHAR** — one mark for both
>> - `BirdID` as **primary key**
>> ```sql
>> CREATE TABLE BIRD_TYPE(
>>   BirdID CHAR(4) NOT NULL,
>>   Name VARCHAR(9),
>>   Size VARCHAR(6),
>>   PRIMARY KEY (BirdID)
>> );
>> ```
>> - Sizing each `VARCHAR` to **fit the longest value in the sample data** shows the data has been read
>> - Using a type **not on the list given** loses the mark, even if it would be valid SQL
>>
>> *Latest: `9618_s23_qp_11_sc_2.b.iii`*

> [!question] 9618 | Complete a given DDL statement [4]
> Complete the following Data Definition Language (DDL) statement to define the table RENTAL.
>
>> [!success]- Answer — 1 mark for each correctly completed line
>> ```sql
>> CREATE TABLE RENTAL(
>>   RentalID INTEGER NOT NULL,
>>   CustomerID INTEGER NOT NULL,
>>   HouseID VARCHAR(5) NOT NULL,
>>   MonthlyCost REAL NOT NULL,
>>   DepositPaid BOOLEAN NOT NULL,
>>   PRIMARY KEY (RentalID)
>> );
>> ```
>> - The gaps always fall on the same four things: the word **`TABLE`** and the table name
>> - … a **`VARCHAR(n)`** for a text field
>> - … a **`REAL` / `CURRENCY`** for a money field
>> - … **`PRIMARY KEY`** before the bracketed field
>>
>> *Latest: `9618_s21_qp_12_sc_1.c.i`*

> [!question] 9618 | Write an SQL script to add one field to an existing table [2]
> Write a Structured Query Language (SQL) script to add **one** field to the table CONTAINER to store the date of last inspection.
>
>> [!success]- Answer — 1 mark for the ALTER TABLE statement, 1 for the field with a suitable name and type
>> ```sql
>> ALTER TABLE CONTAINER
>> ADD InspectionDate DATE;
>> ```
>> - The **type must match what is stored** — `DATE` for a date
>> - For a resolution such as "1920 × 1068": `ALTER TABLE PHOTOGRAPH ADD Resolution TEXT;` or `VARCHAR(11)` (`w22_qp_13_sc_2.d`)
>>
>> *Latest: `9618_w25_qp_12_sc_4.b`*

> [!question] 9618 | Write an SQL script to add two fields to an existing table [3]
> Write an SQL script to include **two** new fields in CAMERA_DATA, to store the number of photographs currently on the camera **and** the date the camera was last used.
>
>> [!success]- Answer — 1 mark for each bullet, 3 marks
>> - `ALTER TABLE CAMERA_DATA`
>> - `ADD NumberStored INTEGER`
>> - `, LastUsed DATE;`
>> ```sql
>> ALTER TABLE CAMERA_DATA
>> ADD NumberStored INTEGER, LastUsed DATE;
>> ```
>> - **One `ADD`, two fields separated by a comma** — a second `ALTER TABLE` line is not needed
>>
>> *Latest: `9618_w22_qp_11_sc_4.d`*

> [!question] 9618 | Write DDL statements to include a field to store a date [3]
> Write DDL statements to include a field in the table PURCHASE to store the date of the order.
>
>> [!success]- Answer — 1 mark per bullet, 3 marks
>> - `ALTER TABLE PURCHASE`
>> - `ADD OrderDate`
>> - A suitable data type, e.g. `DATE`
>> ```sql
>> ALTER TABLE PURCHASE
>> ADD OrderDate DATE;
>> ```
>>
>> *Latest: `9618_w21_qp_12_sc_6.c.ii`*

> [!question] 9618 | Write an SQL script to link a foreign key to an existing table [2]
> The table EXAM_QUESTION has been created but the foreign key has not been linked. Write an SQL script to update EXAM_QUESTION and link the foreign key to EXAM.
>
>> [!success]- Answer — 1 mark each, 2 marks
>> - **Altering** the correct table
>> - **Adding the foreign key** referencing the correct table and field
>> ```sql
>> ALTER TABLE EXAM_QUESTION
>> ADD FOREIGN KEY (ExamID) REFERENCES EXAM(ExamID);
>> ```
>> - The table altered is the one **containing** the foreign key, **not** the one being referenced
>> - Same pattern for `EVENT` → `PLAYER` (`s24_qp_11_sc_6.c.i`)
>>
>> *Latest: `9618_s24_qp_12_sc_4.c`; `9618_s24_qp_11_sc_6.c.i`*

> [!question] Inferred | Explain what a NOT NULL constraint is and why it is used [2]
> Explain what is meant by the `NOT NULL` constraint and why it would be applied to a field.
>
>> [!success]- Answer — 4 points for 2 marks
>> - `NOT NULL` means the field **cannot be left empty** when a record is stored
>> - The DBMS **rejects** any record that does not supply a value for it
>> - It is **essential for a primary key**, which must always have a value to identify the record uniquely
>> - It is a form of **validation** — a presence check — enforced by the DBMS rather than by the application
>>
>> *Inference: "include constraints where appropriate" is a named mark point in the two 5-mark CREATE TABLE questions, yet no question asks **what a constraint is** or **why it matters**. It is the link between 8.3 and the data-integrity feature in 8.2.*

> [!question] SME | State the DDL command set and the seven data types [4]
> State the DDL commands in the syllabus sub-set and the data types available for attributes.
>
>> [!success]- Answer — 6 points for 4 marks
>> - `CREATE DATABASE <name>` — creates a new database
>> - `CREATE TABLE <name> ( … )` — creates a table with fields and data types
>> - `ALTER TABLE <name> ADD <field> <type>` — changes an existing table definition
>> - `PRIMARY KEY (field)` — sets the unique identifier
>> - `FOREIGN KEY (field) REFERENCES Table(Field)` — sets up the relationship
>> - The **seven data types**: **CHARACTER** fixed-length text · **VARCHAR(n)** variable-length text to max n · **BOOLEAN** true/false · **INTEGER** whole numbers · **REAL** decimals · **DATE** a calendar date · **TIME** a time of day
>>
>> *These seven are the only types named in the syllabus — offering `TEXT`, `FLOAT` or `CURRENCY` is credited in some mark schemes, but the seven are always safe.*

---

## 8.3.5 Writing SQL (DML) scripts

> [!question] 9618 | Write a script with a join, a condition and an ORDER BY [5]
> Write an SQL script to return only the ProductID, ProductName and ComplaintDetails for all products with a rating of 5 or less. The results need to be displayed in descending order of rating.
>
>> [!success]- Answer — 1 mark per bullet, max 5
>> - `SELECT` and the **correct attributes**
>> - `FROM` and the **correct tables**
>> - **Tables joined correctly**
>> - **Correct condition** for the rating
>> - **Correct ORDER BY clause**
>> ```sql
>> SELECT PRODUCT.ProductID, ProductName, ComplaintDetails
>> FROM PRODUCT INNER JOIN COMPLAINT
>> ON PRODUCT.ProductID = COMPLAINT.ProductID
>> WHERE Rating <= 5
>> ORDER BY Rating DESC;
>> ```
>> - The `FROM A, B WHERE A.key = B.key` form is **equally credited** — the mark is for joining, not the keyword
>> - `ProductID` must be **qualified** with its table, because it exists in both
>> - "descending" → **`DESC`**
>>
>> *Latest: `9618_w25_qp_13_sc_5.c`. The only 9618 question ever to use `ORDER BY`.*

> [!question] 9618 | Write a script using COUNT across two joined tables [4]
> Write an SQL script to return the number of containers stored in the database for the ship with the name Caledonia.
>
>> [!success]- Answer — 1 mark per bullet, max 4
>> - `SELECT COUNT` statement
>> - Using the **correct tables**
>> - **Joining** the tables
>> - The **condition for the name**
>> ```sql
>> SELECT COUNT(ContainerID)
>> FROM CONTAINER, SHIP
>> WHERE CONTAINER.ShipID = SHIP.ShipID
>> AND ShipName = "Caledonia";
>> ```
>> - "the number of" → **`COUNT`**, never `SUM`
>>
>> *Latest: `9618_w25_qp_12_sc_4.c`; also `s25_qp_12_sc_5.d.i`, `w23_qp_11_sc_3.c.ii`*

> [!question] 9618 | Write a script using COUNT with AS and several conditions [4]
> Write an SQL script to return the total number of placements completed by the student with ID LDEA01 at the company with ID NEAM. The total should be given an appropriate name.
>
>> [!success]- Answer — 1 mark per bullet, max 4
>> - `SELECT COUNT` of any appropriate field
>> - **`AS` and an appropriate name**
>> - `FROM` and correct table, and `WHERE` with **one** correct condition
>> - **Two `AND` clauses** with the other two conditions
>> ```sql
>> SELECT COUNT(CompanyID) AS TotalPlacements
>> FROM PLACEMENT
>> WHERE CompanyID = "NEAM"
>> AND StudentID = "LDEA01"
>> AND Complete = TRUE;
>> ```
>> - Whenever the question says "given an appropriate name" or "with an appropriate title", the **`AS` carries its own mark**
>> - "completed" is a **third** condition — `Complete = TRUE` — easily missed
>>
>> *Latest: `9618_w25_qp_11_sc_2.c.ii`*

> [!question] 9618 | Write a script using SUM with a date range [3]
> Write an SQL script to return the total quantity of ice cream sold to the customer with the ID of 0034E in the year 2023.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - `SELECT SUM(Quantity)`
>> - `FROM SALE WHERE` and **one** correct condition
>> - `AND` with the **remainder** of the correct conditions
>> ```sql
>> SELECT SUM(Quantity)
>> FROM SALE
>> WHERE CustomerID = "0034E"
>> AND Date >= #01/01/2023# AND Date <= #31/12/2023#;
>> ```
>> - Dates are wrapped in **`#…#`**, strings in speech marks
>> - **"in the year 2023" needs two conditions**, not one
>> - "the total quantity" → **`SUM`**, not `COUNT`
>>
>> *Latest: `9618_w24_qp_13_sc_4.b`; also `w24_qp_12_sc_6.b.ii`, `w24_qp_11_sc_2.b.iii`*

> [!question] 9618 | Write a script using COUNT with GROUP BY [3]
> Write an SQL script to return the number of events that each player has completed.
>
>> [!success]- Answer — 1 mark each, 3 marks
>> - Selecting `PlayerID` from `EVENT`
>> - **Counting** `EventID`
>> - **Grouping by** `PlayerID`
>> ```sql
>> SELECT PlayerID, COUNT(EventID)
>> FROM EVENT
>> GROUP BY PlayerID;
>> ```
>> - **"the number of X for each Y" always means `GROUP BY Y`** — and Y must also appear in the `SELECT`
>>
>> *Latest: `9618_s24_qp_11_sc_6.c.ii`*

> [!question] 9618 | Write a script using COUNT, a join and GROUP BY, with a title [4]
> Write an SQL script to return the number of times each show is scheduled. The result needs to include the show name and a suitable field name for the number of times it is scheduled.
>
>> [!success]- Answer — 1 mark each for, 4 marks
>> - Selecting `COUNT` of an attribute in `PERFORMANCE` **with a suitable name**
>> - `FROM` clause
>> - **Joining** the tables
>> - **Grouping by the title and selecting the title**
>> ```sql
>> SELECT SHOW.Title, COUNT(PERFORMANCE.PerformanceID) AS NumberOfShowings
>> FROM PERFORMANCE INNER JOIN SHOW
>> ON PERFORMANCE.ShowID = SHOW.ShowID
>> GROUP BY SHOW.Title;
>> ```
>> - The last mark needs **both** — grouping by the title **and** selecting it
>>
>> *Latest: `9618_s24_qp_13_sc_4.c`*

> [!question] 9618 | Write a script using COUNT, a join, a condition and GROUP BY [4]
> Write an SQL script to return the customer name for each customer that has orders they have not collected. Include the number of orders each customer has not collected, with an appropriate title.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - Selection of customer name **and** counting any field from `ORDER` as an appropriate identifier
>> - **Joining** the tables `ORDER` and `CUSTOMER`
>> - `AND` (or `WHERE`) clause: `Collected = FALSE`
>> - **Grouping** by customer ID or customer name
>> ```sql
>> SELECT CustomerName, COUNT(OrderID) AS NotCollected
>> FROM ORDER, CUSTOMER
>> WHERE ORDER.CustomerID = CUSTOMER.CustomerID
>> AND Collected = FALSE
>> GROUP BY CUSTOMER.CustomerID;
>> ```
>> - A **Boolean is compared to `TRUE`/`FALSE`**, not to a string — `= "FALSE"` is wrong
>>
>> *Latest: `9618_s25_qp_13_sc_6.c`*

> [!question] 9618 | Write a script using SUM, a join, a condition and GROUP BY [4]
> Write an SQL script to output the customer ID, the customer's name and the total cost of the customer's orders that have **not** been paid. The output of the total cost must have an appropriate title.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - Selecting the customer ID, customer name and **sum of TotalCost with an appropriate identifier**
>> - `FROM` clause with a suitable **join** of tables (`ON` **or** `WHERE`)
>> - `ORDER.Paid = FALSE` condition **with the correct key word**
>> - `GROUP BY` condition
>> ```sql
>> SELECT CUSTOMER.CustomerID, CUSTOMER.Name, SUM(ORDER.TotalCost) AS TotalOwed
>> FROM CUSTOMER INNER JOIN ORDER
>> ON CUSTOMER.CustomerID = ORDER.CustomerID
>> WHERE ORDER.Paid = FALSE
>> GROUP BY CUSTOMER.CustomerID;
>> ```
>> - "with the correct key word" means `WHERE` if it is the first condition, `AND` if the join is already in the `WHERE`
>>
>> *Latest: `9618_s25_qp_11_sc_5.e`*

> [!question] 9618 | Write a script using SUM across two joined tables [4]
> Write the SQL script to return the total quantity of items that the customer with the ID of HJ231 has ordered.
>
>> [!success]- Answer — 1 mark for each line, max 4
>> ```sql
>> SELECT SUM(Quantity)
>> FROM ORDER_ITEM, SHOP_ORDER
>> WHERE ORDER_ITEM.OrderNo = SHOP_ORDER.OrderNo
>> AND SHOP_ORDER.CustomerID = 'HJ231';
>> ```
>> - Equally credited:
>> ```sql
>> SELECT SUM(Quantity)
>> FROM ORDER_ITEM INNER JOIN SHOP_ORDER
>> ON ORDER_ITEM.OrderNo = SHOP_ORDER.OrderNo
>> WHERE SHOP_ORDER.CustomerID = 'HJ231';
>> ```
>> - The quantity is in one table and the customer in the other — hence the join
>>
>> *Latest: `9618_w23_qp_11_sc_3.c.ii`*

> [!question] 9618 | Write a script using COUNT with a date condition and AS [4]
> Write the SQL script to return the total number of courses that have started after 9 September 2023. The value returned must have an appropriate field name.
>
>> [!success]- Answer — 1 mark for each bullet, 4 marks
>> - `SELECT Count(CourseID)`
>> - `AS NumOfCourses`
>> - `FROM COURSE_SCHEDULE`
>> - `WHERE DateStarted > "09/09/23";`
>> ```sql
>> SELECT Count(CourseID) AS NumOfCourses
>> FROM COURSE_SCHEDULE
>> WHERE DateStarted > "09/09/23";
>> ```
>> - A **single-table** query can still be worth four marks if it has four clauses
>> - "after" → **`>`**, not `>=`
>>
>> *Latest: `9618_w23_qp_13_sc_3.b.ii`*

> [!question] 9618 | Write a script using OR for two alternative values [4]
> Write a Structured Query Language (SQL) script to return the names of all the horses that have the horse level intermediate or beginner.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - `SELECT` field name
>> - `FROM` table `HORSE`
>> - `WHERE` with Intermediate / Beginner
>> - `OR` with the other one
>> ```sql
>> SELECT Name
>> FROM HORSE
>> WHERE HorseLevel = "Intermediate"
>> OR HorseLevel = "Beginner";
>> ```
>> - **The field name must be repeated on both sides of the `OR`** — `WHERE HorseLevel = "A" OR "B"` is wrong
>>
>> *Latest: `9618_s23_qp_12_sc_2.c.ii`*

> [!question] 9618 | Write a script using LIKE with a wildcard [4]
> Complete the SQL script to return the total number of telescopes owned by the company whose ID begins with HW.
>
>> [!success]- Answer — 1 mark for each correctly completed missing part
>> ```sql
>> SELECT COUNT (TelescopeID)
>> FROM TELESCOPE
>> WHERE CompanyID LIKE 'HW%';
>> ```
>> - **"begins with" / "starting with" → `LIKE`** with a trailing wildcard
>> - Both `'HW%'` and `'HW*'` are credited
>> - Same pattern for camera IDs starting with CAN (`w22_qp_11_sc_4.c.ii`)
>>
>> *Latest: `9618_w22_qp_13_sc_2.c`*

> [!question] 9618 | Complete a partly written SQL script [5]
> Complete the SQL script to return the number of birds of each size seen by the person with the ID of J_123.
>
>> [!success]- Answer — 1 mark for each correctly completed space
>> ```sql
>> SELECT BIRD_TYPE.Size, COUNT(BIRD_TYPE.BirdID) AS NumberOfBirds
>> FROM BIRD_TYPE, BIRD_SEEN
>> WHERE BIRD_SEEN.PersonID = "J_123"
>> AND BIRD_TYPE.BirdID = BIRD_SEEN.BirdID
>> GROUP BY BIRD_TYPE.Size;
>> ```
>> - The **tariff equals the number of gaps**, and they always fall on the same landmarks:
>> - … the **aggregate function**, the **second table name** in the `FROM`, the **qualified field name** in the `WHERE`, the **join condition**, and the **`GROUP BY`**
>> - "of each size" → `GROUP BY … Size`, with `Size` also in the `SELECT`
>>
>> *Latest: `9618_s23_qp_11_sc_2.b.iv`*

> [!question] 9618 | Write a script to insert a new record [4]
> A new product needs to be entered into the database. Write a Structured Query Language (SQL) script to enter the new product into the table PRODUCT.
>
>> [!success]- Answer — 1 mark each, 4 marks
>> - `INSERT INTO PRODUCT`
>> - `VALUES` with **opening and closing brackets**
>> - Inserting the **string** fields correctly, **including quotation marks**, into the correct fields
>> - Inserting the **numeric** fields correctly into the correct fields
>> ```sql
>> INSERT INTO PRODUCT (ProductID, ProductName, QuantityInBox, Cost, SupplierID)
>> VALUES ("002323", "Blue ball point 2 mm", 50, 5.00, "SFX223");
>> ```
>> - Naming the fields is **optional** — `INSERT INTO PRODUCT VALUES (…)` is equally credited
>> - … but then the **order must match the table definition exactly**
>> - An ID like `"002323"` is a **string** — the leading zeros would be lost as a number
>>
>> *Latest: `9618_s25_qp_13_sc_6.b`; also `w22_qp_12_sc_5.b`, `w21_qp_11_sc_5.c.ii`*

> [!question] 9618 | Write a script to update existing data [3]
> The character with the ID "0002" needs its level changed to 3 and its money changed to 10000.00. Write an SQL script to change the character's data.
>
>> [!success]- Answer — 1 mark for each point, 3 marks
>> - `UPDATE` the correct table
>> - `SET` **both** fields
>> - `WHERE` condition
>> ```sql
>> UPDATE CHARACTER
>> SET Level = 3, Money = 10000.00
>> WHERE CharacterID = "0002";
>> ```
>> - Two fields are set in **one `SET` clause**, separated by a comma — not two statements
>> - **Omitting the `WHERE` updates every record** in the table
>>
>> *Latest: `9618_s25_qp_12_sc_5.d.ii`*

> [!question] 9618 | Write a script to delete records [2]
> Write a Structured Query Language (SQL) script to delete all placements that have been completed.
>
>> [!success]- Answer — 1 mark per bullet, max 2
>> - `DELETE FROM` and the correct table
>> - The **correct condition**
>> ```sql
>> DELETE FROM PLACEMENT
>> WHERE Complete = TRUE;
>> ```
>> - `DELETE FROM` removes **records**, not fields or tables — `DROP` is not the answer
>> - Without a `WHERE`, every record in the table is deleted
>>
>> *Latest: `9618_w25_qp_11_sc_2.c.i`*

> [!question] 9618 | Complete a DML statement using COUNT and GROUP BY [3]
> Complete the DML statements to return the number of cars for sale in each shop.
>
>> [!success]- Answer — 1 mark per correctly completed statement
>> ```sql
>> SELECT COUNT(RegistrationNumber)
>> FROM CAR
>> GROUP BY ShopID;
>> ```
>> - Counting the **primary key** of the table is always a safe choice for `COUNT`
>> - The `SUM` variant: `SELECT SUM(Quantity) FROM PURCHASE_ITEM WHERE PurchaseID = "3011A";` (`w21_qp_12_sc_6.c.i`)
>>
>> *Latest: `9618_w21_qp_11_sc_5.c.i`*

> [!question] Inferred | Write a script using AVG with a title [3]
> Write an SQL script to return the average cost of all the products, with an appropriate title.
>
>> [!success]- Answer — 5 points for 3 marks
>> - `SELECT AVG(Cost)`
>> - `AS` and an appropriate name
>> - `FROM PRODUCT;`
>> ```sql
>> SELECT AVG(Cost) AS AverageCost
>> FROM PRODUCT;
>> ```
>> - `AVG` behaves exactly like `SUM` — it takes a **numeric field**, and needs an `AS` whenever a title is asked for
>> - With a condition or a join it marks the same way as any other aggregate question
>>
>> *Inference: the syllabus names `SUM`, `COUNT` **and `AVG`**. SUM and COUNT appear in almost every paper; **`AVG` has never appeared in a question in either series**. It is the clearest untested item in 8.3.*

> [!question] Inferred | Write a script using ORDER BY on two fields [3]
> Write an SQL script to return all customers, sorted by town in ascending order and then by surname in ascending order.
>
>> [!success]- Answer — 5 points for 3 marks
>> - `SELECT * FROM CUSTOMER`
>> - `ORDER BY` the **first** field
>> - … then the **second**, separated by a comma
>> ```sql
>> SELECT *
>> FROM CUSTOMER
>> ORDER BY Town ASC, Surname ASC;
>> ```
>> - `ASC` is the **default** and may be omitted; `DESC` must always be written
>> - The **leftmost field is the primary sort**; the second only breaks ties
>>
>> *Inference: `ORDER BY` is named in the syllabus and appears in exactly **one** 9618 question — `w25_qp_13_sc_5.c`, the most recent series. `ASC` versus `DESC` and multi-field sorting have never been tested, and a second appearance is likely.*

> [!question] Inferred | Explain what an INNER JOIN does [2]
> Explain what an `INNER JOIN` does in an SQL query.
>
>> [!success]- Answer — 4 points for 2 marks
>> - It **combines rows from two tables** into a single result
>> - … where the value of the **joining field matches** in both tables
>> - Rows in either table with **no matching row** in the other are **excluded** from the result
>> - The join condition is written in the `ON` clause, or as a condition in the `WHERE` clause — both are equivalent
>>
>> *Inference: every mark scheme accepts both join forms and most print both, but no question has ever asked what an inner join **does**.*

> [!question] SME | State the DML command set [4]
> State the SQL commands used to query and to maintain the data in a database.
>
>> [!success]- Answer — 6 points for 4 marks
>> - **Retrieving:** `SELECT … FROM` chooses the columns and tables · `WHERE` filters on a condition
>> - … `ORDER BY … ASC/DESC` sorts the results · `GROUP BY` groups rows sharing a value, so an aggregate returns one row per group
>> - … `INNER JOIN … ON` combines rows from two tables on a matching key
>> - … `SUM()` totals a numeric column · `COUNT()` counts rows · `AVG()` averages a numeric column
>> - **Maintaining:** `INSERT INTO … VALUES (…)` adds a record
>> - … `UPDATE … SET … WHERE` modifies existing data · `DELETE FROM … WHERE` removes records
>>
>> *The three habits that protect marks: **qualify every field with its table** as soon as two tables are involved; put **strings in quotation marks and dates in `#…#`**; and give every aggregate an **`AS` name** whenever the question mentions a title, a name or a heading.*
