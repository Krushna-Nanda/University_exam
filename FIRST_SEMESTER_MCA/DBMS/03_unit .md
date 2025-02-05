### **Normalization and Normal Forms**

**Normalization** is a database design technique used to minimize data redundancy and improve data integrity by organizing data into well-structured tables. It involves decomposing a table into smaller, related tables while maintaining the same data.

A **normal form** is a level or stage of database normalization. There are several normal forms, and each builds upon the previous one, ensuring better structure and fewer anomalies.

---

### **Types of Normal Forms**
1. **First Normal Form (1NF)**
   - A table is in 1NF if:
     - Each column contains atomic (indivisible) values.
     - Each row is unique and identified by a primary key.
     - There are no repeating groups or arrays.
   - **Example:**
     Before 1NF:
     | ID  | Name       | Subjects        |
     |-----|------------|-----------------|
     | 1   | John       | Math, Science   |
     | 2   | Alice      | English, History|

     After 1NF:
     | ID  | Name  | Subject    |
     |-----|-------|------------|
     | 1   | John  | Math       |
     | 1   | John  | Science    |
     | 2   | Alice | English    |
     | 2   | Alice | History    |

2. **Second Normal Form (2NF)**
   - A table is in 2NF if:
     - It is in 1NF.
     - All non-key attributes are fully dependent on the **entire primary key** (no partial dependency).
   - **Example:**
     Before 2NF:
     | StudentID | CourseID | CourseName | Instructor |
     |-----------|----------|------------|------------|
     | 1         | 101      | Math       | Mr. Smith  |
     | 2         | 102      | Science    | Dr. Brown  |

     After 2NF (split tables):
     - **Student-Course Table**:
       | StudentID | CourseID |
       |-----------|----------|
       | 1         | 101      |
       | 2         | 102      |

     - **Course Table**:
       | CourseID | CourseName | Instructor |
       |----------|------------|------------|
       | 101      | Math       | Mr. Smith  |
       | 102      | Science    | Dr. Brown  |

3. **Third Normal Form (3NF)**
   - A table is in 3NF if:
     - It is in 2NF.
     - There are no transitive dependencies (non-key attributes depend only on the primary key and not on other non-key attributes).
   - **Example:**
     Before 3NF:
     | StudentID | CourseID | Instructor | InstructorPhone |
     |-----------|----------|------------|-----------------|
     | 1         | 101      | Mr. Smith  | 1234567890      |
     | 2         | 102      | Dr. Brown  | 9876543210      |

     After 3NF (split tables):
     - **Student-Course Table**:
       | StudentID | CourseID |
       |-----------|----------|
       | 1         | 101      |
       | 2         | 102      |

     - **Instructor Table**:
       | Instructor | InstructorPhone |
       |------------|-----------------|
       | Mr. Smith  | 1234567890      |
       | Dr. Brown  | 9876543210      |

4. **Boyce-Codd Normal Form (BCNF)**
   - A table is in BCNF if:
     - It is in 3NF.
     - For every functional dependency (A → B), A must be a superkey (uniquely identifies each row in the table).
   - **Example:**
     If a professor teaches only one course:
     | Professor  | Course    |
     |------------|-----------|
     | Dr. Brown  | Physics   |
     | Dr. Smith  | Chemistry |

     This violates BCNF because `Course → Professor` is a dependency, but `Course` is not a superkey. To fix:
     - **Decomposed Tables**:
       | Course    | Professor |
       |-----------|-----------|
       | Physics   | Dr. Brown |
       | Chemistry | Dr. Smith |

---

### Higher Normal Forms:
5. **Fourth Normal Form (4NF)**
   - A table is in 4NF if:
     - It is in BCNF.
     - There are no multivalued dependencies (MVDs), meaning a column should not have multiple independent values for a single primary key.

6. **Fifth Normal Form (5NF)**
   - A table is in 5NF if:
     - It is in 4NF.
     - It eliminates **join dependency**, meaning it cannot be decomposed further without losing data integrity.

7. **Sixth Normal Form (6NF)**
   - Rarely used in practice.
   - It ensures that every table represents a unique relationship, usually applied in temporal databases.

---

### Summary Table for Normal Forms:

| **Normal Form** | **Key Requirements**                                                                 |
|------------------|--------------------------------------------------------------------------------------|
| 1NF              | Eliminate repeating groups and ensure atomic values.                               |
| 2NF              | Eliminate partial dependencies (dependence on part of a composite primary key).     |
| 3NF              | Eliminate transitive dependencies (non-key attributes depend only on the primary key). |
| BCNF             | Every determinant is a superkey.                                                   |
| 4NF              | Eliminate multivalued dependencies.                                                |
| 5NF              | Eliminate join dependencies.                                                       |

