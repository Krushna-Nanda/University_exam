### **What is Serializability?**  
Serializability means making sure that when multiple transactions are running at the same time, the final result is the same as if those transactions ran one by one (in a sequence). It ensures there are no conflicts or errors caused by transactions overlapping.

---

### **Why is Serializability Important?**  
When many users or systems are working with the database at the same time, their transactions might interfere with each other. Serializability prevents problems like:  
- Incorrect data updates  
- Lost changes  
- Reading incomplete data  

---

### **Example to Understand Serializability:**  
Imagine two people (A and B) are shopping online and using the same wallet balance: ₹1,000.  

1. **Transaction 1 (A):** A wants to buy a phone for ₹800.  
2. **Transaction 2 (B):** B wants to buy a watch for ₹500.  

#### Without Serializability (Conflicts Happen):  
- Both A and B check the balance at the same time: ₹1,000.  
- A deducts ₹800, leaving ₹200, but B doesn't know the balance has changed and also deducts ₹500.  
- Final balance = ₹200 (from A) and ₹500 deducted by B → **Incorrect result!**  

#### With Serializability:  
- The database ensures one transaction finishes before the other starts.  
- A buys the phone (₹1,000 - ₹800 = ₹200).  
- Then, B tries to buy the watch but sees the balance is ₹200 and cannot proceed.  
- **Final balance is correct.**  

---

### **Key Point:**  
Serializability ensures that even though transactions may run together, the result will always be as if they ran one after the other, avoiding conflicts or errors.

# command

### Types of SQL Languages

SQL (Structured Query Language) is used to interact with databases. It is divided into several types, each serving a distinct purpose. Here’s a short note on each type of SQL language, with examples:

---

### 1. **Data Definition Language (DDL)**
DDL is used to define and modify database structures such as tables, schemas, and indexes.

- **Common Commands**:
  - `CREATE`: Creates new tables or databases.
  - `ALTER`: Modifies existing database objects.
  - `DROP`: Deletes tables, databases, or other database objects.
  - `TRUNCATE`: Removes all rows from a table but keeps the structure.

- **Example**:
  ```sql
  CREATE TABLE students (
      id INT,
      name VARCHAR(50),
      age INT
  );
  ```

---

### 2. **Data Manipulation Language (DML)**
DML is used to manipulate data within database tables. This includes inserting, updating, deleting, and selecting data.

- **Common Commands**:
  - `INSERT`: Adds new records to a table.
  - `UPDATE`: Modifies existing records.
  - `DELETE`: Removes records from a table.
  - `SELECT`: Retrieves data from one or more tables.

- **Example**:
  ```sql
  INSERT INTO students (id, name, age)
  VALUES (1, 'John Doe', 20);
  
  SELECT * FROM students;
  ```

---

### 3. **Data Query Language (DQL)**
DQL is used to query or retrieve data from the database. It primarily consists of the `SELECT` command.

- **Common Command**:
  - `SELECT`: Retrieves data from a database.
  
- **Example**:
  ```sql
  SELECT name, age FROM students WHERE age > 18;
  ```

---

### 4. **Data Control Language (DCL)**
DCL is used to control access and permissions in the database. It deals with granting or revoking privileges.

- **Common Commands**:
  - `GRANT`: Assigns specific privileges to users.
  - `REVOKE`: Removes specific privileges from users.

- **Example**:
  ```sql
  GRANT SELECT ON students TO user1;
  REVOKE SELECT ON students FROM user1;
  ```

---

### 5. **Transaction Control Language (TCL)**
TCL is used to manage transactions within the database, ensuring that changes are committed or rolled back.

- **Common Commands**:
  - `COMMIT`: Saves the changes made in the transaction.
  - `ROLLBACK`: Undoes the changes made in the transaction.
  - `SAVEPOINT`: Sets a point in a transaction to which you can later roll back.
  - `SET TRANSACTION`: Sets the properties of a transaction.

- **Example**:
  ```sql
  BEGIN;
  UPDATE students SET age = 21 WHERE id = 1;
  COMMIT;
  ```

---

### Summary Table:

| SQL Type               | Purpose                                          | Common Commands                                | Example |
|------------------------|--------------------------------------------------|------------------------------------------------|---------|
| **DDL**                | Defines database structures                     | `CREATE`, `ALTER`, `DROP`, `TRUNCATE`         | `CREATE TABLE students (...)` |
| **DML**                | Manipulates data in tables                      | `INSERT`, `UPDATE`, `DELETE`, `SELECT`         | `INSERT INTO students ...` |
| **DQL**                | Queries data from the database                  | `SELECT`                                       | `SELECT * FROM students` |
| **DCL**                | Controls database access and permissions        | `GRANT`, `REVOKE`                              | `GRANT SELECT ON students TO user1` |
| **TCL**                | Manages transactions within the database        | `COMMIT`, `ROLLBACK`, `SAVEPOINT`              | `COMMIT;` |

Each type of SQL language serves a specific role in interacting with the database, from defining structures to manipulating and querying data, controlling access, and managing transactions.
