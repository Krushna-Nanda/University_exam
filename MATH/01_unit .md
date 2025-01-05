Here is the text in normal format:

1. **Subsets of a Set**:  
If a set has **n** elements, the total number of subsets is given by the formula:  

Number of Subsets = 2^n  

This includes both the empty set and the set itself.

2. **Proper Subsets of a Set**:  
A proper subset of a set is any subset that is not equal to the set itself. The formula to find the number of proper subsets is:  

Number of Proper Subsets = 2^n - 1  

Here’s a comprehensive overview of **sets**, their **types**, and related **terminology** in mathematics, with proper examples:

Here’s the content in a simple text format that you can copy and paste:

---

## **1. Set**
- A **set** is a collection of well-defined, distinct objects.
- Denoted by curly brackets **{}**.

### Example:
- \( A = \{1, 2, 3\} \) (A set of numbers)
- \( B = \{\text{apple, banana, mango}\} \) (A set of fruits)

---

## **2. Types of Sets**
### **a) Empty Set (Null Set)**
- A set with no elements.
- Denoted by \( \emptyset \) or \( \{\} \).

**Example:**  
\( A = \{x | x > 5, x < 3\} = \emptyset \) (No element satisfies the condition.)

---

### **b) Finite Set**
- A set with a finite number of elements.

**Example:**  
\( A = \{1, 2, 3, 4, 5\} \) (5 elements)

---

### **c) Infinite Set**
- A set with an infinite number of elements.

**Example:**  
\( A = \{1, 2, 3, \dots\} \) (The set of all natural numbers)

---

### **d) Universal Set**
- The set containing all possible elements in a specific context.
- Denoted by \( U \).

**Example:**  
If studying natural numbers, \( U = \mathbb{N} = \{1, 2, 3, \dots\} \).

---

### **e) Subset**
- A set \( A \) is a **subset** of \( B \) if every element of \( A \) is also an element of \( B \).  
- Denoted by \( A \subseteq B \).

**Example:**  
\( A = \{1, 2\}, B = \{1, 2, 3, 4\} \)  
Here, \( A \subseteq B \).

---

### **f) Proper Subset**
- A set \( A \) is a **proper subset** of \( B \) if \( A \subseteq B \) but \( A \neq B \).  
- Denoted by \( A \subset B \).

**Example:**  
\( A = \{1, 2\}, B = \{1, 2, 3\} \)  
Here, \( A \subset B \).

---

### **g) Power Set**
- The **power set** of a set \( A \) is the set of all subsets of \( A \), including \( \emptyset \) and \( A \) itself.  
- Denoted by \( P(A) \).

**Example:**  
For \( A = \{1, 2\} \):  
\( P(A) = \{\emptyset, \{1\}, \{2\}, \{1, 2\}\} \).

---

### **h) Singleton Set**
- A set with only one element.

**Example:**  
\( A = \{5\} \)

---

### **i) Equal Sets**
- Two sets \( A \) and \( B \) are **equal** if they have exactly the same elements.  
- Denoted by \( A = B \).

**Example:**  
\( A = \{1, 2, 3\}, B = \{3, 2, 1\} \)  
Here, \( A = B \).

---

### **j) Disjoint Sets**
- Two sets are **disjoint** if they have no elements in common.  

**Example:**  
\( A = \{1, 2\}, B = \{3, 4\} \)  
Here, \( A \cap B = \emptyset \).

---

### **k) Overlapping Sets**
- Sets that have at least one common element.

**Example:**  
\( A = \{1, 2\}, B = \{2, 3\} \)  
Here, \( A \cap B = \{2\} \).

---

### **l) Complement of a Set**
- The **complement** of set \( A \) (denoted as \( A' \)) contains all elements of the universal set \( U \) that are not in \( A \).  

**Example:**  
If \( U = \{1, 2, 3, 4\}, A = \{1, 2\} \),  
then \( A' = \{3, 4\} \).

---

## **3. Set Operations**
### **a) Union (\( \cup \))**
- The set of all elements in \( A \) or \( B \) or both.  

**Example:**  
\( A = \{1, 2\}, B = \{2, 3\} \),  
\( A \cup B = \{1, 2, 3\} \).

---

### **b) Intersection (\( \cap \))**
- The set of elements common to both \( A \) and \( B \).  

**Example:**  
\( A = \{1, 2\}, B = \{2, 3\} \),  
\( A \cap B = \{2\} \).

---

### **c) Difference (\( A \setminus B \))**
- The set of elements in \( A \) but not in \( B \).  

**Example:**  
\( A = \{1, 2, 3\}, B = \{2, 4\} \),  
\( A \setminus B = \{1, 3\} \).

---

### **d) Symmetric Difference (\( A \Delta B \))**
- The set of elements in \( A \) or \( B \), but not in both.  

**Example:**  
\( A = \{1, 2, 3\}, B = \{2, 4\} \),  
\( A \Delta B = \{1, 3, 4\} \).

---

### **e) Cartesian Product (\( A \times B \))**
- The set of all ordered pairs \( (a, b) \), where \( a \in A \) and \( b \in B \).  

**Example:**  
\( A = \{1, 2\}, B = \{a, b\} \),  
\( A \times B = \{(1, a), (1, b), (2, a), (2, b)\} \).

---

## **4. Venn Diagrams**
- A visual representation of sets using overlapping circles to show relationships (union, intersection, difference, etc.).

**Example:**  
A Venn diagram can depict \( A \cup B \), \( A \cap B \), and \( A \setminus B \).

---

---

## **5. Terminology Cheat Sheet**
| **Term**              | **Symbol**       | **Definition**                                   |
|-----------------------|------------------|------------------------------------------------|
| Universal Set         | \( U \)         | Contains all elements in the context.          |
| Subset                | \( A \subseteq B \) | \( A \) is contained in \( B \).                |
| Proper Subset         | \( A \subset B \) | \( A \) is a subset of \( B \), but not equal. |
| Power Set             | \( P(A) \)      | Set of all subsets of \( A \).                 |
| Union                 | \( A \cup B \)  | Elements in \( A \) or \( B \) or both.        |
| Intersection          | \( A \cap B \)  | Elements common to both \( A \) and \( B \).   |
| Complement            | \( A' \)        | Elements not in \( A \) but in \( U \).        |
| Difference            | \( A \setminus B \) | Elements in \( A \) but not in \( B \).         |
| Symmetric Difference  | \( A \Delta B \) | Elements in \( A \) or \( B \), not both.      |
| Cartesian Product     | \( A \times B \) | All ordered pairs from \( A \) and \( B \).    |

Let me know if you'd like any specific part explained further!

# ===========================


## Summary Table of Set Operations

| **Operation**            | **Symbol**   | **Description**                                          |
|--------------------------|--------------|----------------------------------------------------------|
| Union                    | \( \cup \)   | All elements in either set or both.                      |
| Intersection             | \( \cap \)   | All elements common to both sets.                        |
| Difference               | \( \setminus \) | All elements in set \( A \) but not in \( B \).           |
| Symmetric Difference     | \( \Delta \) | Elements in \( A \) or \( B \), but not both.            |
| Complement               | \( A' \)     | All elements in the universal set but not in \( A \).    |
| Cartesian Product        | \( A \times B \) | Set of all ordered pairs from \( A \) and \( B \).        |
| Subset                   | \( \subseteq \) | Set \( A \) is contained within \( B \).                 |
| Proper Subset            | \( \subset \) | Set \( A \) is a subset of \( B \), but not equal.       |
| Power Set                | \( P(A) \)   | Set of all subsets of \( A \).                           |
| Disjoint                 | \( A \cap


# =============================================================================================

Here’s the solution in a clean, normal format for easy copy-pasting:

---

**Given Information:**

- Total students: 120  
- Students studying French (F): 20  
- Students studying English (E): 50  
- Students studying Hindi (H): 70  
- Students studying both English and French (E ∩ F): 5  
- Students studying both English and Hindi (E ∩ H): 20  
- Students studying both Hindi and French (H ∩ F): 10  
- Students studying all three languages (F ∩ E ∩ H): 3  

---

**(i) Hindi alone**  
Formula:  
Hindi alone = |H| - |H ∩ E| - |H ∩ F| + |F ∩ E ∩ H|  

Calculation:  
Hindi alone = 70 - 20 - 10 + 3 = 43  

**Answer:** Hindi alone = 43  

---

**(ii) French alone**  
Formula:  
French alone = |F| - |F ∩ E| - |F ∩ H| + |F ∩ E ∩ H|  

Calculation:  
French alone = 20 - 5 - 10 + 3 = 8  

**Answer:** French alone = 8  

---

**(iii) English but not Hindi**  
Steps:  

1. English alone = |E| - |E ∩ H| - |E ∩ F| + |F ∩ E ∩ H|  
   English alone = 50 - 20 - 5 + 3 = 28  

2. English and French but not Hindi = (E ∩ F) - (F ∩ E ∩ H)  
   English and French but not Hindi = 5 - 3 = 2  

3. Total = English alone + (English and French but not Hindi)  
   Total = 28 + 2 = 30  

**Answer:** English but not Hindi = 30  

---

**(iv) Hindi but not French**  
Steps:  

1. Hindi alone = |H| - |H ∩ F| - |H ∩ E| + |F ∩ E ∩ H|  
   Hindi alone = 70 - 10 - 20 + 3 = 43  

2. Hindi and English but not French = (H ∩ E) - (F ∩ E ∩ H)  
   Hindi and English but not French = 20 - 3 = 17  

3. Total = Hindi alone + (Hindi and English but not French)  
   Total = 43 + 17 = 60  

**Answer:** Hindi but not French = 60  

---

**Final Answers:**  
1. Hindi alone = 43  
2. French alone = 8  
3. English but not Hindi = 30  
4. Hindi but not French = 60  

--- 

You can copy and paste this format easily. Let me know if anything else is needed! 😊
