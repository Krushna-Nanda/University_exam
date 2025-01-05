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

