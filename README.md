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

Here are the correct **Regular Expressions (R.E.)** for each condition:  

---

### **(i) A string that starts with 'a' and ends with 'b'.**  
\[
\mathbf{a (a | b)^* b}
\]  
✅ **Explanation:**  
- `a` → Ensures the string starts with 'a'.  
- `(a | b)*` → Allows any combination of 'a' and 'b' in between (including empty).  
- `b` → Ensures the string ends with 'b'.  

✅ **Examples:** `ab`, `aab`, `abb`, `aabb`, `abab`  
❌ **Invalid:** `ba`, `bb`, `aa`, `b`, `a`  

---

### **(ii) A string that starts with 'b' and ends with 'a'.**  
\[
\mathbf{b (a | b)^* a}
\]  
✅ **Explanation:**  
- `b` → Ensures the string starts with 'b'.  
- `(a | b)*` → Any combination of 'a' and 'b' in between.  
- `a` → Ensures the string ends with 'a'.  

✅ **Examples:** `ba`, `bba`, `baba`, `bbaa`, `bbabba`  
❌ **Invalid:** `ab`, `bb`, `aa`, `aba`, `b`  

---

### **(iii) A string that starts with 'a' and ends with 'bb'.**  
\[
\mathbf{a (a | b)^* bb}
\]  
✅ **Explanation:**  
- `a` → Starts with 'a'.  
- `(a | b)*` → Any combination of 'a' and 'b' in between.  
- `bb` → Ends with 'bb'.  

✅ **Examples:** `abb`, `aabb`, `ababb`, `aaabb`, `ababbb`  
❌ **Invalid:** `ab`, `bb`, `aaa`, `aab`, `babb`  

---

### **(iv) A string that contains at least two 'a's.**  
\[
\mathbf{(a | b)^* a (a | b)^* a (a | b)^*}
\]  
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

✅ These are correct and cover all cases.
