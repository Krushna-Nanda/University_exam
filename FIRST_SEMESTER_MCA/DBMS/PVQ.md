Thank you for sharing the 2022-2023 previous year questions! Here's a concise breakdown with corresponding modules:

---

### **Part-I (2 x 10 = 20 Marks)**  
2-mark questions:

(a) In the Relational model, what do you mean by cardinality?  
**Module:** Unit 2 - Relational Model  

(b) Explain the following constraints: Primary Key and Foreign Key with an example of each.  
**Module:** Unit 2 - Relational Model  

(c) How can you map a conceptual model to a relational model?  
**Module:** Unit 2 - E-R Model  

(d) Differentiate between the following: Theta Join, Equi Join, Natural Join, and Outer Join.  
**Module:** Unit 2 - Relational Algebra  

(e) A primary key if combined with a foreign key creates what?  
**Module:** Unit 2 - Relational Model  

(f) Differentiate between:  
   i) Procedural and non-procedural DML  
   ii) Catalog and metadata  
**Module:**  
   i) Unit 4 - SQL  
   ii) Unit 1 - Introduction to DBMS  

(g) What is the ACID property?  
**Module:** Unit 4 - Transaction Management  

(h) A primary key if combined with a foreign key creates what?  
**Module:** Unit 2 - Relational Model  

(i) What is the possible violation if an application program uses isolation level "Repeatable Read"?  
**Module:** Unit 4 - Transaction Management  

(j) Define the properties of a transaction and who ensures them?  
**Module:** Unit 4 - Transaction Management  

---

### **Part-II (6 x 8 = 48 Marks)**  
6-mark questions:  

(a) What do you understand by a data model? Explain the difference between the conceptual data model and the internal model.  
**Module:** Unit 1 - Introduction to DBMS  

(b) What are the basic operations for a relational language? How are basic operations represented in relational algebra and SQL?  
**Module:** Unit 2 - Relational Algebra  

(c) What is the use of DML in DBMS?  
**Module:** Unit 4 - SQL  

(d) Which protocol always ensures a recoverable schedule?  
**Module:** Unit 4 - Transaction Management  

(e) Does a relation in 3rd Normal Form satisfy the properties of Lossless decomposition and dependency preservation? Explain with an example.  
**Module:** Unit 3 - Schema Refinement  

(f) Given R with FD set F = {A → B, B → C, D → B, C → D, D → E}, find the number of redundant FDs in F.  
**Module:** Unit 3 - Schema Refinement  

(g) Given R(ABCDEFGH) with FDs F = {A → C, B → D, E → F, G → H, C → G}. How many candidate keys are there? Which normal form is R in?  
**Module:** Unit 3 - Schema Refinement  

(h) Why do query optimizers consider only left-deep join trees? Give an example of a query and a plan that would not be considered because of this restriction.  
**Module:** Unit 4 - SQL  

(i) What is normalization? Explain the first and second normal forms using appropriate examples.  
**Module:** Unit 3 - Schema Refinement  

(j) What is the possible violation if an application program uses isolation level "Repeatable Read"?  
**Module:** Unit 4 - Transaction Management  

(k) Explain the entity integrity and referential integrity constraints. How are they useful in database design?  
**Module:** Unit 2 - Relational Model  

(l) Explain with the help of examples, the concept of insertion anomalies and deletion anomalies.  
**Module:** Unit 3 - Schema Refinement  

---

### **Part-III (16 Marks)**  
16-mark questions:  

(3) a. Describe the various database recovery techniques in brief.  
**Module:** Unit 4 - Transaction Management  

b. Use relational algebra to express the queries for given relations.  
**Module:** Unit 2 - Relational Algebra  

(4) a. Explain various locking techniques for concurrency control.  
**Module:** Unit 4 - Transaction Management  

b. How do multiversion timestamp ordering and multiversion two-phase concurrency control schemes execute concurrent transactions in a controlled manner?  
**Module:** Unit 4 - Transaction Management  

(5) a. Discuss the correspondence between the E-R model constructs and the relational model constructs.  
**Module:** Unit 2 - E-R Model  

b. Define a view in SQL. Construct a view for the given relations.  
**Module:** Unit 4 - SQL  

(6) a. Show that the decomposition of R into R1 and R2 is lossless-join but not dependency-preserving.  
**Module:** Unit 3 - Schema Refinement  

b. Give SQL expressions for queries based on the provided relations.  
**Module:** Unit 4 - SQL  

--- 

Let me know if you'd like to dive deeper into any specific question!

# 2023 - 2024

Here is the extracted and formatted content with the corresponding module information added below each question:

---

**Part-I (2 x 10 = 20 Marks)**

Answer the following questions:

a) What is a discriminator in the ER model?  
**Module: Database Design (Unit 2)**  

b) How many n-ary relations can be formed over n sets having p elements each?  
**Module: Counting and Relations (Unit 3)**  

c) What is lossless join decomposition?  
**Module: Schema Refinement and Normal Forms (Unit 3)**  

d) What is a foreign key? Give an example.  
**Module: Database Design (Unit 2)**  

e) Define 5NF (Fifth Normal Form).  
**Module: Schema Refinement and Normal Forms (Unit 3)**  

f) Differentiate candidate key vs. super key.  
**Module: Database Design (Unit 2)**  

g) What do you mean by the ACID property of transactions?  
**Module: DBMS Transactions (Unit 4)**  

h) What are the various causes of database failure?  
**Module: DBMS Transactions (Unit 4)**  

i) What is deadlock in a database?  
**Module: DBMS Transactions (Unit 4)**  

j) What are the various states of a transaction in a database?  
**Module: DBMS Transactions (Unit 4)**  

---

**Part-II (6 x 8 = 48 Marks)**

Only Focused-Short Answer Type Questions (Answer Any Eight out of Twelve):

a) Discuss in detail views and also creating, altering, and destroying of views.  
**Module: SQL and Advanced Database Concepts (Unit 4)**  

b) Discuss the anomalies in designing a relational database.  
**Module: Schema Refinement and Normal Forms (Unit 3)**  

c) Consider the relation R(ABCDEFG) and the set of functional dependencies {BCD → A, BC → E, A → F, F → G, C → D, A → G}. Decompose R up to 3rd Normal Form (3NF).  
**Module: Schema Refinement and Normal Forms (Unit 3)**  

d) Let's consider a relational table R with attributes A, B, C, D, and E. The set of functional dependencies (FDs) defined on relation R are FDs = {A → B; BC → E; ED → A}. Decompose relation R up to Boyce-Codd Normal Form (BCNF).  
**Module: Schema Refinement and Normal Forms (Unit 3)**  

e) i. Write a relational algebra (RA) query for the following SQL statement: `SELECT Roll No, Name, Age FROM Student WHERE Branch = 'IT' AND Age > 15;`  
   ii. Write a tuple relational calculus (TRC) query for the following SQL statement: `SELECT Instructor ID FROM Instructor WHERE Salary > 100,000;`  
**Module: SQL and Advanced Database Concepts (Unit 4)**  

f) i. Write a correlated sub-query to retrieve employee details of an organization earning the highest salary.  
   ii. Express R ⋈ S (natural join) in terms of π (projection), σ (selection), and × (Cartesian product) operators.  
**Module: SQL and Advanced Database Concepts (Unit 4)**  

g) Differentiate nested loop, hash join, and merge join.  
**Module: SQL and Advanced Database Concepts (Unit 4)**  

h) Explain about Integrity Constraints over relations in detail.  
**Module: Database Design (Unit 2)**  

i) Consider the transactions T1, T2, and T3 and the schedules S1 and S2 given below. Test for conflict serializability of S1 and S2.  

    T1: r1(X); r1(Z); w1(X); w1(Z)  
    T2: r2(Y); r2(Z); w2(Z)  
    T3: r3(Y); r3(X); w3(Y)  

    S1: r1(X); r3(Y); r3(X); r2(Y); r2(Z); w3(Y); w2(Z); r1(Z); w1(X); w1(Z)  
    S2: r1(X); r3(Y); r2(Y); r3(X); r1(Z); r2(Z); w3(Y); w1(X); w2(Z); w1(Z)  
**Module: DBMS Transactions (Unit 4)**  

j) Consider the following database schedule with two transactions, T1 and T2:  

    S = r2(X); r1(X); r2(Y); w1(X); r1(Y); w2(X); a1; a2  

    where ri(Z) denotes a read operation by transaction Ti on a variable Z, wi(Z) denotes a write operation by Ti on a variable Z and ai denotes an abort by transaction Ti. Comment on the following properties of the schedule: cascadelessness, recoverability, deadlock, conflict serializability.  
**Module: DBMS Transactions (Unit 4)**  

k) Explain about aggregate operators in SQL with examples.  
**Module: SQL and Advanced Database Concepts (Unit 4)**  

l) Explain about remote backup systems.  
**Module: Advanced Database Topics (Unit 4)**  

---

**Part-III (Only Long Answer Type Questions - Answer Any Two out of Four) (16 marks each)**

Q3) Construct an ER-diagram for a company that is organized into departments. Each department has a unique name, a unique number, and a particular employee who manages the department. We keep track of the start date when that employee began managing the department. A department may have several locations. A department controls a number of projects, each of which has a unique number and a single location. We store each employee's name, social security number, address, salary, sex, and birth date. An employee is assigned to one department but may work on several projects, which are not necessarily controlled by the same department. We keep track of the number of hours per week that an employee works on each project. We also keep track of the direct supervisor of each employee. We want to keep track of the dependents of each employee for insurance purposes. We keep each dependent's first name, sex, birth date, and relationship to the employee. Write the steps to convert an ER-diagram into equivalent relational tables. Convert the above ER-diagram into equivalent relational tables.  
**Module: Database Design (Unit 2)**  

Q4) Explain the 3-schema database architecture. Discuss the roles of database DB users and DB administrators.  
**Module: Database Management Systems Overview (Unit 1)**  

Q5) What is a lock in DBMS? Describe the two-phase locking (2PL) protocol. What are the variations of the 2PL protocol? Discuss the cascadelessness, recoverability, deadlock, and conflict serializability of all variations.  
**Module: DBMS Transactions (Unit 4)**  

Q6) Write short notes on any two of the following:  

    i. Cursor vs. Trigger  
    ii. Query optimization  
    iii. Data warehouse  
    iv. Log-based Database Recovery  
**Module: SQL and Advanced Database Concepts (Unit 4)**
