# Keys
Keys are the unique identifier used in **DBMS** to uniquely identify a tuple(s)or rows n a table.

We can easily understand the idea of the keys by visualizing the following example of student databse with their project.

### **College Database Example**

We have the following tables for the database:

1. **Students**
2. **Projects**

### **Tables and Data**

#### **1. Students Table**

| ID | Name             | Address   | Course   | CitizenshipNumber | PANNumber      |
|----|------------------|-----------|----------|-------------------|----------------|
| 1  | Darshan Subedi    | Kawasoti  | Physical | 1234567890        | 123456789       |
| 2  | Creation Duwal    | Bhaktapur  | Physical | 0987654321        | 987654321       |
| 3  | Bimin Kiran Koju  | Bhaktapur  | Biology   | 1122334455        | 112233445       |
| 4  | Srijan Pokhrel    | Kawasoti  | Biology   | 5566778899        | 556677889       |

#### **2. Projects Table**

| ProjectNumber | ProjectName      |
|---------------|------------------|
| 101           | Quantum Mechanics |
| 102           | Astrophysics     |
| 103           | Molecular Biology |
| 104           | Cell Biology     |

#### **3. StudentProjects Table**

| ID | ProjectNumber | Role         |
|----|---------------|--------------|
| 1  | 101           | Lead Researcher |
| 1  | 102           | Contributor   |
| 2  | 102           | Lead Researcher |
| 3  | 103           | Researcher     |
| 4  | 104           | Contributor   |

### **Types of Keys Explained**

Let’s break down the different types of keys using the **Students** and **StudentProjects** tables:

---

#### **1. Primary Key**

**Definition:** A primary key is a field (or a combination of fields) that uniquely identifies each record in a table. It ensures that every record is unique and not null.

**Example:**

- **Students Table:** `ID` is the primary key.

| ID | Name             | Address   | Course   | CitizenshipNumber | PANNumber      |
|----|------------------|-----------|----------|-------------------|----------------|
| 1  | Darshan Subedi    | Kawasoti  | Physical | 1234567890        | 123456789       |
| 2  | Creation Duwal    | Bhaktapur  | Physical | 0987654321        | 987654321       |
| 3  | Bimin Kiran Koju  | Bhaktapur  | Biology   | 1122334455        | 112233445       |
| 4  | Srijan Pokhrel    | Kawasoti  | Biology   | 5566778899        | 556677889       |

**Why It Matters:** `ID` must be unique for each student, ensuring no two students have the same ID and every student can be uniquely identified.

#### **2. Foreign Key**

**Definition:** A foreign key is a field (or a combination of fields) in one table that refers to the primary key in another table. It creates a relationship between the two tables.

**Examples:**

- **StudentProjects Table:** 
  - `ID` is a foreign key that refers to `ID` in the Students table.
  - `ProjectNumber` is a foreign key that refers to `ProjectNumber` in the Projects table.

| ID | ProjectNumber | Role         |
|----|---------------|--------------|
| 1  | 101           | Lead Researcher |
| 1  | 102           | Contributor   |
| 2  | 102           | Lead Researcher |
| 3  | 103           | Researcher     |
| 4  | 104           | Contributor   |

**Why It Matters:** It links `StudentProjects` with `Students` and `Projects`, ensuring that every `ID` and `ProjectNumber` in `StudentProjects` correspond to valid entries in `Students` and `Projects`, respectively.

#### **3. Composite Key**

**Definition:** A composite key uses two or more columns to uniquely identify a record in a table.

**Example:**

- **StudentProjects Table:** `ID` and `ProjectNumber` together form the composite key.

| ID | ProjectNumber | Role         |
|----|---------------|--------------|
| 1  | 101           | Lead Researcher |
| 1  | 102           | Contributor   |
| 2  | 102           | Lead Researcher |
| 3  | 103           | Researcher     |
| 4  | 104           | Contributor   |

**Why It Matters:** `ID` + `ProjectNumber` together ensure that each record is unique. This combination is used to track which student works on which project.

#### **4. Candidate Key**

**Definition:** A candidate key is a column or a set of columns that can be a primary key. There can be multiple candidate keys in a table, but only one is chosen as the primary key.

**Example:**

- **Students Table:** `ID` and `PANNumber` are both candidate keys.

| ID | PANNumber  |
|----|------------|
| 1  | 123456789  |
| 2  | 987654321  |
| 3  | 112233445  |
| 4  | 556677889  |

**Why It Matters:** `ID` is chosen as the primary key, but `PANNumber` is also unique and could serve as a primary key.

#### **5. Alternate Key**

**Definition:** An alternate key is a candidate key that is not selected as the primary key.

**Example:**

- **Students Table:**
  - **Primary Key:** `ID`
  - **Alternate Key:** `PANNumber`

| ID | PANNumber  |
|----|------------|
| 1  | 123456789  |
| 2  | 987654321  |
| 3  | 112233445  |
| 4  | 556677889  |

**Why It Matters:** `PANNumber` is a unique identifier but is not used as the primary key. It provides an alternative unique way to identify students.

#### **6. Artificial Key**

**Definition:** An artificial key (or surrogate key) is a key created specifically to uniquely identify records, often using an auto-incremented integer.

**Example:**

- **Students Table:** `ID` is an artificial key.

| ID | Name             | Address   | Course   | CitizenshipNumber | PANNumber      |
|----|------------------|-----------|----------|-------------------|----------------|
| 1  | Darshan Subedi    | Kawasoti  | Physical | 1234567890        | 123456789       |
| 2  | Creation Duwal    | Bhaktapur  | Physical | 0987654321        | 987654321       |
| 3  | Bimin Kiran Koju  | Bhaktapur  | Biology   | 1122334455        | 112233445       |
| 4  | Srijan Pokhrel    | Kawasoti  | Biology   | 5566778899        | 556677889       |

**Why It Matters:** `ID` is auto-generated to ensure that each student has a unique identifier, even if there is no natural key for this purpose.

### **Summary of Key Types**

| Key Type         | Definition                                               | Example                                | Why It Matters                                              |
|------------------|----------------------------------------------------------|----------------------------------------|-------------------------------------------------------------|
| **Primary Key**  | Uniquely identifies each record in a table             | `ID` in Students Table                | Ensures no two records are the same and cannot be null.     |
| **Foreign Key**  | Refers to the primary key in another table               | `ID` in StudentProjects Table          | Links tables together and ensures referential integrity.    |
| **Composite Key**| Uses two or more columns to uniquely identify a record   | `ID` + `ProjectNumber` in StudentProjects Table | Allows for complex uniqueness requirements.               |
| **Candidate Key**| Potential primary keys from which one is chosen          | `ID` and `PANNumber` in Students Table  | Multiple options for primary keys; only one is chosen.      |
| **Alternate Key**| A candidate key not chosen as the primary key            | `PANNumber` in Students Table           | Provides additional unique ways to identify records.        |
| **Artificial Key**| A key created specifically to uniquely identify records | `ID` (auto-incremented)                  | Ensures a unique identifier even if there is no natural key.|

[**Go back to homepage**](readme.md)

