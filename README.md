### **Super Key**:  
A **super key** is a set of one or more attributes (columns) in a table that can **uniquely identify each row** in that table. 

### **Key Characteristics of a Super Key**:
1. It may consist of a single column or a combination of multiple columns.
2. **Every table must have at least one super key**, as it is necessary to uniquely identify rows.
3. **Primary Key** is a minimal version of a super key (a super key with no redundant attributes).

---

### **Example**

#### Consider a Table: `Students`

| **StudentID** | **Name** | **Email**             | **PhoneNumber** |
|---------------|----------|-----------------------|-----------------|
| 1             | Alice    | alice@email.com       | 1234567890      |
| 2             | Bob      | bob@email.com         | 9876543210      |
| 3             | Charlie  | charlie@email.com     | 5678901234      |

#### Possible Super Keys:
A **super key** is any set of attributes that can uniquely identify a row. For the `Students` table, the following are examples of super keys:

1. `{StudentID}` (StudentID alone is sufficient to uniquely identify rows.)
2. `{Email}` (Emails are unique for every student.)
3. `{PhoneNumber}` (Phone numbers are unique.)
4. `{StudentID, Email}` (Although `StudentID` alone is sufficient, adding `Email` still uniquely identifies rows, but this is not minimal.)
5. `{StudentID, Name, PhoneNumber}` (This set also uniquely identifies rows but includes redundant attributes.)

---

### **Primary Key vs Super Key**
- A **primary key** is the **minimal super key**, meaning it contains no unnecessary attributes.  
- For example, in the table above:
  - `{StudentID}` is a **primary key**, as it is the smallest super key.
  - `{StudentID, Email}` is a **super key** but not a primary key because `Email` is redundant (not needed for unique identification).

---

### **Key Points to Remember**:
1. **Super keys** can have extra attributes that aren't necessary for unique identification.  
2. A **primary key** is a subset of a super key with no redundant attributes.  
3. All primary keys are super keys, but not all super keys are primary keys.
