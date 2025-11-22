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
