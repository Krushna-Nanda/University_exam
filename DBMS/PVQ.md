2022 - 23

Part-I (2 x 10 = 20 Marks)

Answer the following questions:

a) In the Relational model, what do you mean by cardinality?
b) Explain the following constraints: Primary Key and Foreign key with an example of each.
c) How can you map a conceptual model to a relational model?
d) Differentiate between the following: Theta Join, Equi Join, Natural Join, and Outer Join.
e) A primary key if combined with a foreign key creates what?
f) Differentiate between:
i) Procedural and non-procedural DML
ii) Catalog and metadata
g) What is the ACID property?
h) A primary key if combined with a foreign key creates what? (This appears to be a duplicate of 'e')
i) What is the possible violation if an application program uses isolation level "Repeatable Read"?
j) Define the properties of a transaction and who ensures them?

Part-II (6 x 8 = 48 Marks)

Only Focused-Short Answer Type Questions (Answer Any Eight out of Twelve):

a) What do you understand by a data model? Explain the difference between the conceptual data model and the internal model.
b) What are the basic operations for a relational language? How are basic operations represented in relational algebra and SQL?
c) What is the use of DML in DBMS?
d) Which protocol always ensures a recoverable schedule?
e) Does a relation in 3rd Normal Form satisfy the properties of Lossless decomposition and dependency preservation? Explain with an example.
f) Given R with FD set F = {A → B, B → C, D → B, C → D, D → E}, find the number of redundant FDs in F.
g) Given R(ABCDEFGH) with FDs F = {A → C, B → D, E → F, G → H, C → G}. How many candidate keys are there? Which normal form is R in?
h) Why do query optimizers consider only left-deep join trees? Give an example of a query and a plan that would not be considered because of this restriction.
i) What is normalization? Explain the first and second normal forms using appropriate examples.
j) What is the possible violation if an application program uses isolation level "Repeatable Read"?
k) Explain the entity integrity and referential integrity constraints. How are they useful in database design?
l) Explain with the help of examples, the concept of insertion anomalies and deletion anomalies.   

Part-III (Only Long Answer Type Questions - Answer Any Two out of Four) (8x2 = 16 Marks each)

Q3) a. Describe the various database recovery techniques in brief.

b. Consider the relations:
    PROJECT(proj#, proj_name, chief_architect)
    EMPLOYEE(emp#, emp_name)
    ASSIGNED(proj#, emp#)

    Use relational algebra to express the following queries:
    (a) Get details of employees working on project COMP33.
    (b) Get the employee number of employees who work on all projects.
    (c) Get details of projects on which employee with name 'RAM' is working.
Q4) a. Explain various locking techniques for concurrency control.

b. How do multiversion timestamp ordering and multiversion two-phase concurrency control schemes execute concurrent transactions in a controlled manner?
Q5) a. Discuss the correspondence between the E-R model constructs and the relational model constructs. Show how each E-R model construct can be mapped to the relational model using suitable examples.

b. Define a view in SQL. Construct a view for the above relations which has the S#, SNAME, P#, PNAME renamed as SNO, NAME, PNO, PNAME. (Note: It looks like there's a typo in this question, it likely refers to relations defined in a previous question or context, not the ones in Q3.b).
Q6) a. Suppose that we decompose the schema R(A, B, C, D, E) into R1(A, B, C) and R2(A, D, E). Show that this decomposition is lossless-join and not dependency-preserving if the following set of functional dependencies F holds:   

A → BC
C → D
B → D
E → A

b. Consider the following relations:

S(S#, SNAME, STATUS, CITY)
SP(S#, P#, QTY)
P(P#, PNAME, COLOR, WEIGHT, CITY)

Give an expression in SQL for each of the queries below:   

(a) Get supplier names for suppliers who supply at least one red part.
(b) Get supplier names for suppliers who do not supply part P2.

Let me know if you'd like any of these questions explained further or have any other questions!
