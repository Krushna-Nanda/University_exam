### **Grammar:**  
```
S → aaaS | ε
```  

### **Explanation:**  
- The only input symbol is **'a'**.  
- The rule `S → aaaS` ensures that 'a' appears in multiples of 3.  
- The rule `S → ε` allows an empty string (which has 0 'a's, divisible by 3).  

### **Generated Strings:**  
- `ε` (0 a’s, divisible by 3)  
- `aaa` (3 a’s, divisible by 3)  
- `aaaaaa` (6 a’s, divisible by 3)  
- `aaaaaaaaa` (9 a’s, divisible by 3)  

Thus, this grammar ensures that the number of 'a's is always a multiple of 3. ✅

# lq no 4

## Regular Expressions

### (i) A string that starts with 'a' and ends with 'b'.  
```regex
a (a | b)* b
```
✅ **Explanation:**  
- `a` → Ensures the string starts with 'a'.  
- `(a | b)*` → Allows any combination of 'a' and 'b' in between (including empty).  
- `b` → Ensures the string ends with 'b'.  

✅ **Examples:** `ab`, `aab`, `abb`, `aabb`, `abab`  
❌ **Invalid:** `ba`, `bb`, `aa`, `b`, `a`  

---

### (ii) A string that starts with 'b' and ends with 'a'.  
```regex
b (a | b)* a
```
✅ **Explanation:**  
- `b` → Ensures the string starts with 'b'.  
- `(a | b)*` → Any combination of 'a' and 'b' in between.  
- `a` → Ensures the string ends with 'a'.  

✅ **Examples:** `ba`, `bba`, `baba`, `bbaa`, `bbabba`  
❌ **Invalid:** `ab`, `bb`, `aa`, `aba`, `b`  

---

### (iii) A string that starts with 'a' and ends with 'bb'.  
```regex
a (a | b)* bb
```
✅ **Explanation:**  
- `a` → Starts with 'a'.  
- `(a | b)*` → Any combination of 'a' and 'b' in between.  
- `bb` → Ends with 'bb'.  

✅ **Examples:** `abb`, `aabb`, `ababb`, `aaabb`, `ababbb`  
❌ **Invalid:** `ab`, `bb`, `aaa`, `aab`, `babb`  

---

### (iv) A string that contains at least two 'a's.  
```regex
(a | b)* a (a | b)* a (a | b)*
```
✅ **Explanation:**  
- `(a | b)*` → Allows any combination of 'a' and 'b' before, between, and after the two 'a's.  
- `a` → Ensures there is **at least one 'a'**.  
- `(a | b)*` → More characters can follow.  
- `a` → Ensures **another 'a' appears somewhere**.  

✅ **Examples:** `aa`, `aab`, `aba`, `bbaa`, `babaa`, `baab`  
❌ **Invalid:** `b`, `bb`, `bbb`, `ba`, `ab` (only one 'a')  

---

### **Final Answer:**  
1️⃣ **Starts with 'a', ends with 'b'** → `a (a | b)* b`  
2️⃣ **Starts with 'b', ends with 'a'** → `b (a | b)* a`  
3️⃣ **Starts with 'a', ends with 'bb'** → `a (a | b)* bb`  
4️⃣ **Contains at least two 'a's** → `(a | b)* a (a | b)* a (a | b)*`  

✅ These are correctly formatted and easy to read.


Why is it used?
Pattern Matching: Helps in searching, replacing, and validating text patterns.
Lexical Analysis: Used in compilers for tokenizing programming language syntax.
Automata Theory: Converts into Finite Automata (DFA/NFA) for language recognition.
String Processing: Commonly used in text editors, search engines, and programming.
Properties of Regular Expressions:

Closure Properties: Regular languages are closed under union, concatenation, and Kleene star.
Finite Representation: Regular expressions provide a finite way to represent infinite languages.
No Memory: R.E. cannot count occurrences beyond a fixed pattern (e.g., cannot check balanced parentheses).
Equivalent to Finite Automata: Every R.E. has an equivalent DFA/NFA, and vice versa.

===============================================================

What is a Finite Automaton?
A Finite Automaton (FA) is a mathematical model of a system that reads input symbols one by one and changes its state accordingly. It consists of:

A finite set of states
An input alphabet (symbols it can read)
Transition function (rules for moving between states)
Start state (where it begins)
Final state(s) (accepting states)

There are **four types of automata** based on computational power:  

1. **Finite Automata (FA)** – Used for pattern recognition.  
   - **Example:** DFA for strings ending with '1' in binary.  

2. **Pushdown Automata (PDA)** – Recognizes Context-Free Languages (CFL) using a stack.  
   - **Example:** PDA for balanced parentheses `{ (()), (()()) }`.  

3. **Linear Bounded Automata (LBA)** – A restricted Turing machine used for Context-Sensitive Languages (CSL).  
   - **Example:** LBA for the language `{ a^n b^n c^n | n ≥ 1 }`.  

4. **Turing Machine (TM)** – The most powerful automaton, used for solving any computable problem.  
   - **Example:** TM for palindrome checking.


ε-NFA (Epsilon NFA)
An ε-NFA is a Nondeterministic Finite Automaton that allows transitions without consuming input (ε-moves).
NFA (without ε-transitions)
An NFA without ε-moves only changes states when an actual symbol is read.


Grammar
A grammar is a set of rules that defines how strings in a language are formed. It consists of:

Terminals (Σ): Actual symbols in the language.
Non-terminals (V): Variables representing groups of strings.
Start Symbol (S): The initial non-terminal.
Production Rules (P): Rules to generate valid strings.
✅ Example: Grammar for strings containing only 'a' and 'b':

V = {S}, Σ = {a, b}, S = S
P:
S → aS | bS | ε
(Generates strings like "", "a", "b", "ab", "ba", "aaa", etc.)

Regular Grammar
A Regular Grammar is a type of grammar where production rules follow a specific format to generate regular languages. It is of two types:

Right Linear Grammar (RLG): Rules are of the form A → aB or A → a, where the terminal appears before the non-terminal.
Left Linear Grammar (LLG): Rules are of the form A → Ba or A → a, where the terminal appears after the non-terminal.

Regular Expression (R.E.)
A Regular Expression (R.E.) is a sequence of characters that defines a pattern for a set of strings in a regular language. It is used to represent languages recognized by Finite Automata.

Example:
Language: Strings over {0,1} that contain at least one '1'.
✅ Regular Expression: 1(0|1)*
👉 This means:

'1' must appear at least once.
(0|1)* allows any number of 0s or 1s after the first '1'.
✅ Valid Strings: "1", "10", "101", "111", "1001", etc.
