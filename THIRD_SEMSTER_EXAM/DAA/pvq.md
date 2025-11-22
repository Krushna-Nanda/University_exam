Based on the images provided, here is the exact transcription of the **Design Analysis and Algorithms** examination paper, organized by section.

### **Exam Header Details**

  * **Examination:** 2nd Semester Regular/Back Examination: 2023-24
  * **Subject:** Design Analysis and Algorithms
  * **Branch(S):** MCA
  * **Time:** 3 Hours
  * **Max Marks:** 100
  * **Q.Code:** P186

-----

### **Part-I**

**Answer Question No.1 (Part-1) which is compulsory, any eight from Part-II and any two from Part-III.**
**The figures in the right hand margin indicate marks.**

**Q1. Answer the following questions:** *(2 x 10)*

  * **a)** Is $f(n) = 3n^2 + 5n + 6 = O(n^3)$?
  * **b)** Write two advantages of depth first search over breadth first search.
  * **c)** Assume that a merge sort algorithm in the worst case takes 30 seconds for an input size 64. Find out the most closely approximates the maximum input size of a problem that can be solved in 6 minutes.
  * **d)** Define Dis-joint set. Write the operation supported by the dis-joint set.
  * **e)** Differentiate between Decision problem and optimization problem.
  * **f)** Find the minimum number of comparisons required to determine if an integer appears more than $n/2$ times in a sorted array of $n$ integers.
  * **g)** What is the time required for finding the shortest path in a graph with n-vertices and e-edges?
  * **h)** Differentiate between Greedy approach and Dynamic programming.
  * **i)** What are the constraints required for a Backtracking method?
  * **j)** Determine whether the following problems are P, NP or NP-Complete, Satisfiability problem, Hamiltonian cycle, TSP problem, Knapsack problem, Clique, Set partitioning.

-----

### **Part-II**

**Only Focused-Short Answer Type Questions- (Answer Any Eight out of Twelve)** *(6 x 8)*

**Q2.**

  * **a)** State the Greedy Knapsack? Find an optimal solution to the Knapsack instance $n = 3$, $m = 20$, $(P1, P2, P3) = (25, 24, 15)$ and $(W1, W2, W3) = (18, 15, 10)$

  * **b)** Explain the Divide and Conquer technique. Design a recursive algorithm for binary search.

  * **c)** Differentiate between Prim's and Kruskal algorithm. Let G be the complete undirected graph on 4 vertices having 6 edges weights 1, 2, 3, 4, 5, 6. What is the maximum possible weight that a minimum weight spanning tree of G can have?

  * **d)** Arrange following elements by using heap sort and demonstrate each step:
    $22, 34, 57, 20, 81, 14, 47, 43, 48, 61$

  * **e)** Determine Longest Common Subsequence of `<1,0,0,1,0,1,0,1>` and `<0,1,0,1,1,0,1,1,0>`

  * **f)** Apply the Bottom up Dynamic Approach to the following instance of 0/1 knapsack problem. The maximum capacity of the knapsack is 10.

    | Item | Weight | Profit |
    | :--- | :--- | :--- |
    | 1 | 7 | 42 |
    | 2 | 3 | 12 |
    | 3 | 4 | 40 |
    | 4 | 5 | 25 |

  * **g)** Define Big-Oh and Big-omega notation. Find Big-Oh for the function $f(n) = 4n^2 + 2n + 7$.

  * **h)** Sort the following elements by using merge sort 34, 67, 10, 33, 65, 88, 13, 23.

  * **i)** Design a polynomial time algorithm that verifies whether a graph is 4-colourable. The algorithm should read a string $s$, where $i^{th}$ character of the string represents the colour of node $i$. The output of the algorithm is TRUE or FALSE.

  * **j)** Solve the following recurrence relation:
    $T(n) = 2T(n/2) + n^3$
    $T(n) = 16T(n/4) + n$

  * **k)** Find the minimum number of scalar multiplications required to multiply 5 matrices described by $(p_0, p_1, p_5) = (15, 20, 5, 10, 25, \text{and } 10)$. Determine the order of matrices to be multiplied so that this minimum can be achieved.

  * **l)** Find the time complexity of below Psuedocode.

    ```text
    A()
    {
        Int i, j, k, n;
        For(i=1; i<=n; i++)     - n times
        {
            For(j=1; j<=i; j++)
            {
                For(k=1; k<=100; k++)   100 times
                {
                    Printf("Hello")
                }
            }
        }
    }
    ```

-----

### **Part-III**

**Only Long Answer Type Questions (Answer Any Two out of Four)**

**Q3.**

  * **a)** Sort the following elements using Quick sort algorithm. Analyze the time complexity. **(8)**
    $54, 26, 93, 17, 7731, 44, 55, 20$
  * **b)** The characters a to h has the following set of frequencies based on Fibonacci numbers as follows: **(8)**
    a:1, b:1, c:2, d:3, e:5, f:8, g:13, h:21
    A Huffman code is used to represent the characters. What is the sequence of characters corresponding to following code?
    `110111100111010`

**Q4.**

  * **a)** We are given 9 tasks $T_1, T_2, T_3........T_9$. The execution of each requires 1 unit of times. **(8)**
    What is the maximum profit earned? Consider the following table:

    | TASK | $T_1$ | $T_2$ | $T_3$ | $T_4$ | $T_5$ | $T_6$ | $T_7$ | $T_8$ | $T_9$ |
    | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
    | Profit ($P_i$) | 15 | 20 | 30 | 18 | 18 | 10 | 23 | 16 | 25 |
    | Deadline ($D_i$) | 7 | 2 | 5 | 3 | 4 | 5 | 2 | 7 | 3 |

  * **b)** Find out the shortest path from following graph G using Bellman Ford algorithm taking source vertex S. What its time complexity? **(8)**

**Q5.**

  * **a)** What is a branch and bound technique? How the TSP can be solved using this technique? **(8)**
  * **b)** Discuss the concept of pattern matching algorithm? Write the Rabin-Karp algorithm for the string matching. Suppose $T = 2 \ 5 \ 6 \ 3 \ 1 \ 5 \ 8 \ 9 \ 0 \ 4$, $P = 6 \ 3 \ 1$, $q = 13$ then Find the position where Pattern matching occurs **(8)**

**Q6.**

  * **a)** Discuss the relation between P, NP, NP-complete and NP-Hard problem with suitable example. **(8)**
  * **b)** Discuss the 4 - queen's problem. Draw the portion of the state space tree for $n = 4$ queens using backtracking algorithm. **(8)**


  Based on the images provided, here is the exact transcription of the **Analysis and Design of Algorithms** examination paper (2022-23), organized by section.

### **Exam Header Details**
* **Examination:** 2nd Semester Regular / Back Examination: 2022-23
* **Subject:** Analysis and Design of Algorithms
* **Branch(S):** MCA
* **Time:** 3 Hour
* **Max Marks:** 100
* **Q.Code:** M181

---

### **Part-I**
**Answer Question No.1 (Part-1) which is compulsory, any eight from Part-II and any two from Part-III.**
**The figures in the right hand margin indicate marks.**

**Q1. Answer the following questions:** *(2 x 10)*
* **a)** Arrange the following functions from the lowest asymptotic order to the highest asymptotic order: $7n, 2n, 10n, \log n, 4n^3, 5n^2, 2 \log n, n! \ \& \ \log n$.
* **b)** How the Backtracking of algorithm differs from that of branch and bound algorithm?
* **c)** State three properties of Greedy Method.
* **d)** Define Dis-joint set. Write the operation supported by the dis-joint set.
* **e)** Differentiate between Deterministic and nondeterministic algorithm.
* **f)** Differentiate between Dynamic Programming and Greedy methods.
* **g)** What is the time required for finding the shortest path in a graph with n-vertices and e-edges?
* **h)** Define an Algorithm. Describe the different criteria that satisfy the algorithm.
* **i)** Show that given a maximum flow in a network with edge, a maximum cut of N can be computed in O(m) times.
* **j)** Define polynomial time reducibility.

---

### **Part-II**
**Only Focused-Short Answer Type Questions- (Answer Any Eight out of Twelve)** *(6 x 8)*

**Q2.**
* **a)** Find an optimal solution with optimal value to the given knapsack instance $n=7, m=18, (p1, p2, p3, p4, p5, p6, p7) = (10, 15, 12, 5, 16, 18, 20)$ and $(w1, w2, w3, w4, w5, w6, w7) = (2, 3, 5, 7, 2, 4, 5)$.
* **b)** Define Big-Oh and Big-omega notation. Find Big-Oh for the function $f(n) = 4n^2 + 2n + 7$.
* **c)** Explain Activity Selection Problem along with algorithm.

    | Job | 1 | 2 | 3 | 4 | 5 | 6 |
    | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
    | Start time | 1 | 3 | 0 | 5 | 3 | 7 |
    | Finish Time | 4 | 5 | 6 | 7 | 9 | 9 |

* **d)** Construct a min-heap using the following elements and demonstrate each step:
    $4, 5, 18, 13, 16, 35, 8, 26, 45$.
* **e)** What is single source shortest path problem? What its advantage?
* **f)** Suppose that all characters in the pattern p are different. Show how to accelerate NAIVE-STRING-MATCHING to run in time O(n) on an n-character text T.
* **g)** Define Big-Oh and Big-omega notation. Find Big-Oh for the function $f(n) = 4n^2 + 2n + 7$.
* **h)** Prove that the fractional knapsack problem has the greedy-choice property.
* **i)** The directed Hamiltonian cycle is NP-complete. Prove that the undirected Hamiltonian cycle is reducible to the directed Hamiltonian cycle.
* **j)** Solve the following recurrence relation:
    $T(n) = 2T(n/2) + n^3$
    $T(n) = 16T(n/4) + n$
* **k)** Give the control Abstraction for divide-and-conquer. Use divide and conquer paradigm to devise recurrence relation for analysis of quick sort. use the same to find best case analysis for quick sort.
* **l)** Construct a Huffman tree for the following data obtain its Huffman code

    | Character | A | b | c | d | e | f |
    | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
    | No. of Occurrences | 2 | 3 | 3 | 4 | 6 | 10 |

---

### **Part-III**
**Only Long Answer Type Questions (Answer Any Two out of Four)**
*(16 Marks Each - Note: Marks per sub-question are 8)*

**Q3.**
* **a)** Describe and justify Kruskal's algorithm for finding the minimum spanning tree of an undirected graph. **(8)**
* **b)** Compute m and s table and find optimal parenthesis for multiplication of matrices parenthesis for the matrices $A1_{2 \times 3}, A2_{3 \times 5}, A3_{5 \times 4}, A4_{4 \times 6}$ using Matrix chain multiplications. **(8)**

**Q4.**
* **a)** Explain the algorithm for finding length of LCS. Determine LCS of $<1, 0, 0, 1, 0, 1, 0, 1>$ and $<0, 1, 0, 1, 1, 0, 1, 1, 0>$. **(8)**
* **b)** Find out the shortest path from following graph G using Bellman Ford algorithm taking source vertex S. What its time complexity? **(8)**
    
**Q5.**
* **a)** Explain the approximation algorithm for solving the TSP (Travelling Salesman Problem) problem. **(8)**
* **b)** Discuss the concept of pattern matching algorithm? Write the Rabin-karp algorithm for the string matching. Suppose $T = 2 \ 5 \ 6 \ 3 \ 1 \ 5 \ 8 \ 9 \ 0 \ 4, P = 6 \ 3 \ 1, q = 13$ then Find the position where Pattern matching occurs. **(8)**

**Q6.**
* **a)** Discuss the relation between P, NP, NP-complete and NP-Hard problem with suitable example. **(8)**
* **b)** Write short note on any (TWO) of the following **(8)**
    a) NP-Complete
    b) N-Queen's Problem
    c) Vertex-Cover Algorithm



    Based on the images provided, here is the exact transcription of the **Analysis and Design of Algorithms** examination paper for the academic session 2021-22.

### **Exam Header Details**
* **Examination:** 2nd Semester Regular / Back Examination: 2021-22
* **Subject:** Analysis and Design of Algorithms
* **Branch(S):** MCA (2 Yrs)
* **Time:** 3 Hours
* **Max Marks:** 100
* **Q.Code:** J473

---

### **Part-I**
**Answer Question No.1 (Part-1) which is compulsory, any eight from Part-II and any two from Part-III.**
**The figures in the right hand margin indicate marks.**

**Q1. Answer the following questions:**
*(2 x 10 = 20 Marks)*

* **a)** Explain the situations when insertion sort performs the worst and the best.
* **b)** What are the characteristics of a Red-Black tree.
* **c)** Write the advantages and disadvantages of Depth First Search over Breadth First Search.
* **d)** Explain the principle of optimality with example.
* **e)** Write the recursion of binary search and solve it by Master's method.
* **f)** Given three matrices $A(10 \times 50)$, $B(50 \times 100)$ and $C(100 \times 5)$. What is the minimum number of scalar multiplications required to multiply these three matrices.
* **g)** What is the limitation of Rabin-Karp algorithm?
* **h)** Explain the greedy technique to solve the Travelling Salesman Problem.
* **i)** Differentiate between deterministic and non deterministic algorithm.
* **j)** Write two real-life applications of Travelling Salesman Problem.

---

### **Part-II**
**Only Focused-Short Answer Type Questions- (Answer Any Eight out of Twelve)**
*(6 x 8 = 48 Marks)*

**Q2.**
* **a)** Explain the physical significance of asymptotic notations $O$, $\Omega$ and $\Theta$ with example.
* **b)** Solve the following recurrence using Master's method.
    $T(n) = 1$ for $n=1$
    $= T(n/2) + cn^2$ for other values of $n$
* **c)** Construct the AVL tree for the given set of elements
    $12, 67, 34, 78, 23, 45, 69, 17, 28, 10, 27, 59$
* **d)** Write the Prim's algorithm to construct the minimum spanning tree and find the time complexity.
* **e)** Is greedy technique suitable to find the optimal solution of 0/1 knapsack problem? Justify your answer.
* **f)** Construct the state space tree for solving sum of subset problem and explain how backtracking can be used to solve the problem with reduced time complexity.
* **g)** What is the limitation of finite automata method for string matching problem? How KMP algorithm overcomes it?
* **h)** Define optimal binary search tree problem. Explain how dynamic programming technique finds the optimal solution of it.
* **i)** Explain the mathematical analysis of recursive and nonrecursive algorithms.
* **j)** What is reducibility? Explain with example.
* **k)** Compare the advantages and disadvantages of linked list representation and tree representation of a disjoint set.
* **l)** Explain the following problems.
    Vertex cover decision problem and Vertex cover optimization problem,
    Clique Decision problem and Max Clique problem,
    Chromatic number Decision problem and Chromatic number optimization problem

---

### **Part-III**
**Only Long Answer Type Questions (Answer Any Two out of Four)**
*(16 Marks Each)*

**Q3.**
* **a)** Write the algorithm to create a heap by using heapify procedure and find the time complexity. **(8)**
* **b)** Compute the worst case and average case time complexity of quick sort. Explain the situation where quick sort performs the worst. **(8)**

**Q4.**
* **a)** Construct the decode tree for the given letters and their frequencies of occurrence in the message. **(8)**
    $(a, b, c, d, e, f, g) = (2, 3, 5, 7, 9, 13, 20)$
* **b)** Find the longest common subsequence in the following given two sequences **(8)**
    $X=$ "RAMAYAN" $Y=$ "ATMAN"

**Q5.**
* **a)** Explain how the backtracking algorithm works to solve the 4-queen problem. Explain by constructing the state space tree. **(8)**
* **b)** Explain with example how Rabin Karp algorithm works to find a exact and spurious match of substring in a string. **(8)**

**Q6.**
* **a)** What is approximation algorithm? Can we say greedy algorithm is an approximation algorithm? Justify your answer. **(8)**
* **b)** Explain P, NP, NP-hard and NP-complete class of problems. **(8)**