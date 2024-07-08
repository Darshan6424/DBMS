
# Data Manipulation Language (DML) 

## Introduction

Data Manipulation Language (DML) is a subset of SQL (Structured Query Language) used for managing and manipulating data in a relational database. To focus on manipulating the existing databsase by either adding new stuff or modifying existing data to perform some analysis as well.

## Key Concepts of DML

DML commands are used to perform operations on the data stored in a database. These operations are essential for handling the data and ensuring that it meets the needs of the users or applications. Here’s a breakdown of the core DML commands:

- **SELECT**: Retrieve data from one or more tables.
- **INSERT**: Add new records to a table.
- **UPDATE**: Modify existing records in a table.
- **DELETE**: Remove records from a table.

## 1. SELECT Statement 

The `SELECT` statement is used to query and retrieve data from a database. It is one of the most frequently used DML commands.

### Syntax

```sql
SELECT column1, column2, ...
FROM table_name
WHERE condition;
```

### Example

```sql
SELECT NAME FROM TABLE1 WHERE CLASS BETWEEN 12 AND 14;
SELECT * FROM TABLE1;
SELECT NAME FROM TABLE1;
SELECT ID,NAME FRON TABLE1;
```

## 2. INSERT Statement 

The `INSERT` statement is used to add new rows to a table that is simply talking adding new rows of data into the database. Remeber rows represents the data which are also called tuple(s).

### Syntax

```sql
INSERT INTO table_name (column1, column2, ...)
VALUES (value1, value2, ...);
```

### Example

```sql
INSERT INTO employees (ID,NAME,CLASS)
VALUES (1,"Ball',13);
```

### Insert Multiple Rows

```sql
INSERT INTO employees (ID,NAME,CLASS)
VALUES (2,"Cat",13),
       (3,"Dog",14);
```



## 3. UPDATE Statement 

The `UPDATE` statement is used to modify existing records in a table.

### Syntax

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

### Example

```sql
UPDATE TABLE1
SET NAME = "APPLE" WHERE ID = 1;
```



### Tips

- **Always Use `WHERE` Clause:** Without it, all records in the table will be updated.
- **Check with `SELECT` Before `UPDATE`:** Verify the records that will be affected.

### Example of Checking Records

```sql
SELECT * FROM TABLE1 WHERE last_name = 'SUBEDI';
```

**Explanation:** This query helps verify which records will be updated.

## 4. DELETE Statement 

The `DELETE` statement is used to remove existing records from a table.

### Syntax

```sql
DELETE FROM table_name
WHERE condition;
```

### Example

```sql
DELETE NAME FROM TABLE1
WHERE ID = 1 ;
```
### something to seeeeee

- **Always Use `WHERE` Clause:** Without it, all records in the table will be deleted.

## 5. Importance of DML 

DML commands are crucial for:

- **Data Management:** Performing CRUD (Create, Read, Update, Delete) operations.
- **Data Analysis:** Querying and updating data for analysis and reporting.
- **Application Development:** Building and maintaining dynamic applications.
- **Database Maintenance:** Keeping data up-to-date and accurate.

## Conclusion

Data Manipulation Language (DML) commands are fundamental tools for managing and manipulating data in a relational database. Mastery of these commands will help you perform essential tasks such as querying data, adding new records, updating existing data, and deleting obsolete information.

**TIP FORM ME:** Practice these commands regularly to become proficient and understand the logic behind these dml commands.They are quite easy and practising 2 or 3 times will make you quite perfect.
