### UNIT – 1: Introduction to DBMS

#### **1. File System vs. DBMS**
- **File System**:
  - Stores data in separate files.
  - Data is processed manually or using programming languages.
  - Example: Text files, spreadsheets.
  - Issues:
    - **Data Redundancy**: Same data stored in multiple files.
    - **Data Inconsistency**: Different files may have conflicting data.
    - **No Data Security**: Difficult to restrict access.
    - **Limited Query Capability**: Cannot run complex queries.

- **DBMS (Database Management System)**:
  - Software for managing and querying structured data.
  - Centralized storage of data, reducing redundancy and inconsistency.
  - Provides tools for secure, efficient data access.

  **Advantages of DBMS over File System**:
  - **Reduced Redundancy**: Data is stored only once.
  - **Consistency**: Single source of truth.
  - **Data Security**: Controlled access to sensitive data.
  - **Efficient Queries**: Powerful query languages like SQL.
  - **Data Integrity**: Enforces rules to maintain valid data.
  - **Concurrency Control**: Multiple users can access data safely.

---

#### **2. Storing Data and Queries**
- **Storing Data**: Data is stored in tables (rows and columns) within databases.
- **Queries**: Instructions to retrieve, insert, update, or delete data. Examples:
  - `SELECT` retrieves data.
  - `INSERT` adds new records.

---

#### **3. DBMS Structure**
- DBMS has layers that manage storage, query execution, and data retrieval:
  1. **Application Layer**: User interface for interacting with the DBMS.
  2. **Query Processor**: Converts user queries into low-level instructions.
  3. **Storage Manager**: Manages the physical storage of data on disk.

---

#### **4. Types of Databases**
- **Hierarchical Database**:
  - Data is organized like a tree with parent-child relationships.
  - Example: File systems, where folders contain subfolders/files.

- **Network Database**:
  - Data is organized as a graph, allowing many-to-many relationships.
  - Example: Transport networks.

- **Relational Database**:
  - Data is stored in tables with rows and columns.
  - Relationships are managed using keys.
  - Example: MySQL, PostgreSQL.

- **Key-Value Database**:
  - Simple storage of key-value pairs.
  - Example: Redis, DynamoDB.

- **Object-Oriented Database**:
  - Data is stored as objects with attributes and methods.
  - Example: db4o, ObjectDB.

- **XML Database**:
  - Stores and retrieves data in XML format.
  - Example: BaseX, MarkLogic.

---

#### **5. File Structures in Database**
- Databases organize data in various file structures for efficiency:
  - **Heap Files**: Unordered data storage.
  - **Indexed Files**: Uses indexes for faster searching.
  - **Hashed Files**: Hash functions for quick lookups.

---

#### **6. 3-Schema Architecture of DBMS**
1. **External Schema**:
   - User's view of the data.
   - Tailored for specific users or applications.
2. **Conceptual Schema**:
   - Logical structure of the database.
   - Defines tables, relationships, and constraints.
3. **Internal Schema**:
   - Physical storage of data.
   - How data is stored on the hardware.

---

#### **7. Data Independence**
- Ability to change schema levels without affecting others:
  - **Logical Data Independence**: Changes in conceptual schema don’t affect external schema.
  - **Physical Data Independence**: Changes in physical schema don’t affect conceptual schema.

---

#### **8. E.F. Codd's Rules**
Codd proposed 12 rules for relational databases to ensure consistency:
1. **Information Rule**: Data stored in tables.
2. **Guaranteed Access Rule**: Every value is accessible via table name, primary key, and column.
3. **Systematic Treatment of Nulls**: Support null values for missing data.
4. **Dynamic Online Catalog**: Metadata stored in the database.
5. **Comprehensive Data Sub-Language**: Supports SQL-like queries.
6. **View Updating Rule**: Views should reflect base table updates.
7. **High-Level Insert, Update, Delete**: Data manipulation operations are supported.
8. **Physical Data Independence**: Physical storage changes don’t affect logic.
9. **Logical Data Independence**: Schema changes don’t affect applications.
10. **Integrity Independence**: Constraints are separate from application logic.
11. **Distribution Independence**: Location of data is transparent.
12. **Non-Subversion Rule**: Only authorized users can modify the database.

Would you like to dive deeper into any specific topic?


Before learning the **ER (Entity-Relationship) Model**, there are a few basic terms you should understand. Let's explain each term with **real-world examples** so they’re easy to grasp.

---
