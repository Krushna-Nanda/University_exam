Here is the step-by-step solution using the Rabin-Karp algorithm.

### 1. What is **$q$**?

In the Rabin-Karp algorithm, **$q$** represents the **modulus** used for the hashing function.

* **Purpose:** It is used to keep the hash values small enough to fit into standard integer variables (preventing overflow) and to make calculations faster.
* **Properties:** $q$ is typically a prime number.
* **In this problem:** $q = 13$.

---

### 2. Problem Setup

We need to find the pattern $P$ in text $T$.

* **Text ($T$):** `2 5 6 3 1 5 8 9 0 4`
* **Pattern ($P$):** `6 3 1`
* **Modulus ($q$):** $13$
* **Base/Radix ($d$):** Since the characters are decimal digits, we use **$d = 10$**.
* **Pattern Length ($m$):** $3$

#### The Formula
To calculate the rolling hash, we need the value of $h$ (the multiplier for the most significant digit to be removed):
$$h = d^{m-1} \pmod q$$
$$h = 10^{3-1} \pmod{13}$$
$$h = 100 \pmod{13}$$

Since $13 \times 7 = 91$:
$$100 - 91 = 9$$
**So, $h = 9$.**

---

### 3. Step-by-Step Execution

#### Step A: Calculate the Hash of the Pattern ($p$)
Pattern $P = 6 \ 3 \ 1$ (Value 631).

$$p = 631 \pmod{13}$$
$631 \div 13 = 48$ with a remainder of $7$.
$$p = 7$$
**Target Hash:** **7**

#### Step B: Calculate the Hash of the First Window ($t_0$)
Text window $T[0..2] = 2 \ 5 \ 6$ (Value 256).

$$t_0 = 256 \pmod{13}$$
$256 \div 13 = 19$ with a remainder of $9$.
$$t_0 = 9$$

**Compare:** Is $t_0 (9) == p (7)$? **No match.**

#### Step C: Rolling Hash (Sliding the Window)

We use the rolling hash formula to move to the next position:
$$t_{s+1} = (d \times (t_s - T[s] \times h) + T[s+m]) \pmod q$$

**Iteration 1: Move to Index 1**
* Current Window: `5 6 3`
* Remove Leading Digit ($T[0]$): $2$
* Add Trailing Digit ($T[3]$): $3$

$$t_1 = (10 \times (9 - 2 \times 9) + 3) \pmod{13}$$
$$t_1 = (10 \times (9 - 18) + 3) \pmod{13}$$
$$t_1 = (10 \times (-9) + 3) \pmod{13}$$
$$t_1 = (-90 + 3) \pmod{13}$$
$$t_1 = -87 \pmod{13}$$

*Note: To handle negative modulo results, add $q$ until positive.*
$-87 + (13 \times 7) = -87 + 91 = 4$.

$$t_1 = 4$$
**Compare:** Is $t_1 (4) == p (7)$? **No match.**

**Iteration 2: Move to Index 2**
* Current Window: `6 3 1`
* Remove Leading Digit ($T[1]$): $5$
* Add Trailing Digit ($T[4]$): $1$

$$t_2 = (10 \times (4 - 5 \times 9) + 1) \pmod{13}$$
$$t_2 = (10 \times (4 - 45) + 1) \pmod{13}$$
$$t_2 = (10 \times (-41) + 1) \pmod{13}$$
$$t_2 = (-410 + 1) \pmod{13}$$
$$t_2 = -409 \pmod{13}$$

*Handle negative modulo:*
$-409 + (13 \times 32) = -409 + 416 = 7$.

$$t_2 = 7$$
**Compare:** Is $t_2 (7) == p (7)$? **MATCH FOUND!**

### 4. Final Verification
Since the hash values match ($7 == 7$), we verify the actual characters:
* Pattern: `6 3 1`
* Text at Index 2: `6 3 1`

They are identical.

### Conclusion
The pattern matching occurs at **Index 2** (if 0-based) or **Position 3** (if 1-based).

---
Would you like me to explain how to handle the calculation if the modulus ($q$) creates a hash collision (spurious hit)?


Okay, Krushna — we will **reset everything** and rebuild your Big-O understanding from **zero**, in the simplest possible way.

You said your fundamentals are weak — that’s okay.
I will fix that fully.
No formulas until you actually understand **what Big-O even means**.

Let’s go slow.

---

# **PART 1 — WHAT BIG-O ACTUALLY MEANS (SUPER SIMPLE)**

Big-O answers one question:

# **“How fast does the function grow when N becomes huge?”**

That’s it.

Nothing more.

You NEVER use Big-O for small N like 1, 2, 3.
Big-O cares only about **large input sizes**.

---

# **PART 2 — WHAT IS A “FUNCTION” IN ALGORITHMS?**

When you write an algorithm, it takes time based on input size (N).

Examples:

* If you loop N times → time = N
* If you use nested loops → time = N²
* If you sort array → time = N log N

These are **functions** describing time:

* f(N) = N
* f(N) = N²
* f(N) = N log N
* f(N) = 2N² + N + 3

So **2N² + N + 3** is the function describing time.

Big-O says:

**Which part of this function grows fastest?**
That is all Big-O cares about.

---

# **PART 3 — WHY DO WE MAKE THE RIGHT SIDE BIGGER?**

Because Big-O is an **upper bound**.

Meaning:
We want to show our function is **not growing faster** than some simple function.

If we want to prove:

[
2N^{2} + N + 3 = O(N^{2})
]

We must show:

[
\text{Left side} \le \text{Right side}
]

for large N.

So we write:

[
2N^{2} + N + 3 \le C \cdot N^{2}
]

We purposely make the right side **bigger**, so it is easy to show the left side never exceeds it when N is large.

This is why we increase C.

---

# **PART 4 — WHY DOES N = 1 DOESN'T MATTER?**

Because Big-O does **not care** about small values.

Big-O only cares about **large values** of N.

In the definition, we say:

[
N \ge N_{0}
]

which means:

**Start checking from some point onward**.

If the inequality fails for N = 1, 2, 3 — that’s fine.

We only need it to be true from some N₀ onward.

---

# **PART 5 — NOW THE BIG-O DEFINITION (IN PLAIN LANGUAGE)**

Big-O definition says:

A function f(N) is O(g(N)) if:

**After some point,
f(N) is always smaller than C × g(N)**

for some constant C.

---

# **PART 6 — APPLY IT TO YOUR EXAMPLE**

Your function is:

[
f(N) = 2N^{2} + N + 3
]

We want to compare it to:

[
g(N) = N^{2}
]

Big-O claim:

[
f(N) = O(N^{2})
]

This means:

[
2N^{2} + N + 3 \le C \cdot N^{2} \quad \text{for all } N \ge N_{0}
]

We try C = 3.

Check inequality:

[
2N^{2} + N + 3 \le 3N^{2}
]

Subtract 2N²:

[
N + 3 \le N^{2}
]

Check when this is true:

Test N = 1 → 1+3 = 4; 4 ≤ 1 → False
Test N = 2 → 2+3 = 5; 5 ≤ 4 → False
Test N = 3 → 3+3 = 6; 6 ≤ 9 → True
Test N = 4 → 4+3 = 7; 7 ≤ 16 → True
Test N = 5 → 5+3 = 8; 8 ≤ 25 → True

From N = 3 onward, always true.

So we choose:

* C = 3
* N₀ = 3

That’s enough to satisfy Big-O.

---

# **PART 7 — HOW THIS SATISFIES BIG-O (PLAIN ENGLISH)**

Big-O requires TWO things:

### **Requirement 1: f(N) ≤ C*g(N)**

We showed that:
[
2N^{2} + N + 3 \le 3N^{2}
]
is true for N ≥ 3.

Requirement 1 is satisfied.

### **Requirement 2: This must be true for N ≥ N₀**

We found:
[
N_{0} = 3
]

Requirement 2 is satisfied.

Therefore BOTH conditions are satisfied.

So:

[
\boxed{2N^{2} + N + 3 = O(N^{2})}
]

---

# **PART 8 — ULTRA-SIMPLE WAY (MENTAL TRICK)**

Ignore small terms and constants:

Biggest term = **N²**

Everything else is smaller:

* * N (smaller)
* * 3 (smallest)
* constant 2 is ignored

Therefore:

[
O(N^{2})
]

This shortcut is what most people do.

---

Below is the **perfect 6-mark exam answer** for the **Activity Selection Problem**, along with the **algorithm** and the **solution to your given example**.

I am writing it exactly in a formal, exam-oriented style.

---

# **Activity Selection Problem — Explanation**

The **Activity Selection Problem** is a classic application of the **Greedy Algorithm**.
We are given a set of activities, each with a **start time** and **finish time**, and **only one activity can be performed at a time** using a single resource (such as a person, machine, or classroom).

**Objective:**
Select the **maximum number of non-overlapping activities**.

The optimal greedy approach is:

**Always choose the activity that finishes earliest.**
This maximizes the remaining time for selecting more activities.

---

# **Greedy Algorithm for Activity Selection**

```
Activity-Selection(s[], f[], n):
1. Sort the activities in increasing order of finish time.
2. Select the first activity and include it in the result.
3. For each activity i from 2 to n:
        If s[i] ≥ finish time of last selected activity:
                Select activity i
4. Return the selected set of activities.
```

---

# **Given Data**

| Job         | 1 | 2 | 3 | 4 | 5 | 6 |
| ----------- | - | - | - | - | - | - |
| Start time  | 1 | 3 | 0 | 5 | 3 | 7 |
| Finish time | 4 | 5 | 6 | 7 | 9 | 9 |

---

# **Step 1: Sort activities by finish time**

Sorted by finish time:

| Job | Start | Finish |
| --- | ----- | ------ |
| 1   | 1     | 4      |
| 2   | 3     | 5      |
| 3   | 0     | 6      |
| 4   | 5     | 7      |
| 5   | 3     | 9      |
| 6   | 7     | 9      |

---

# **Step 2: Select activities using Greedy**

### 1) Select first activity

Job 1 (1,4)

### 2) Check next

Job 2: starts 3 < 4 → cannot select
Job 3: starts 0 < 4 → cannot select

### 3) Next

Job 4: starts 5 ≥ 4 → select
Selected: Job 1, Job 4

### 4) Next

Job 5: starts 3 < 7 → cannot select
Job 6: starts 7 ≥ 7 → select

---

# **Final Selected Activities**

**Jobs: 1, 4, 6**

These are mutually compatible (non-overlapping).

---

# **Final Answer**

**Selected Activities = {1, 4, 6}**
**Maximum number of activities = 3**

---

If you want, I can also solve this using:

* a **diagram**,
* a **timeline**,
* or a **step-by-step table**.


