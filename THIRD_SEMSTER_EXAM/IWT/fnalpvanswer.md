Alright bro, here is the **cleanest, easiest, exam-ready answer** for the four array functions:
**shift(), slice(), concat(), push()** — each with short explanation + simple example.
Write this and you will get FULL MARKS 💯🔥

---

# ⭐ **1) shift()**

### **Use:**

Removes the **first element** of the array and returns it.
It also **changes the original array**.

### Example:

```javascript
let arr = [10, 20, 30];
let x = arr.shift();

console.log(x);    // 10  (removed element)
console.log(arr);  // [20, 30]
```

---

# ⭐ **2) slice()**

### **Use:**

Returns **a portion of the array** without modifying the original array.
`slice(start, end)` → end is **not included**.

### Example:

```javascript
let arr = [10, 20, 30, 40, 50];
let part = arr.slice(1, 4);

console.log(part); // [20, 30, 40]
console.log(arr);  // [10, 20, 30, 40, 50] (unchanged)
```

---

# ⭐ **3) concat()**

### **Use:**

Joins two or more arrays and returns a **new array**.
Original arrays are **not changed**.

### Example:

```javascript
let a = [1, 2];
let b = [3, 4];

let result = a.concat(b);

console.log(result); // [1, 2, 3, 4]
console.log(a);      // [1, 2] (unchanged)
```

---

# ⭐ **4) push()**

### **Use:**

Adds one or more elements to the **end** of an array and returns the **new length**.
Original array is **modified**.

### Example:

```javascript
let arr = [10, 20];
arr.push(30);

console.log(arr);    // [10, 20, 30]
```

---

# ⭐ **Short Exam Summary**

| Function     | Meaning                | Modifies Original? |
| ------------ | ---------------------- | ------------------ |
| **shift()**  | Removes first element  | ✔ Yes              |
| **slice()**  | Extracts part of array | ❌ No               |
| **concat()** | Joins arrays           | ❌ No               |
| **push()**   | Adds element at end    | ✔ Yes              |

---

If you want bro, I can also give:

🔥 pop(), unshift(), splice()
🔥 map(), filter(), reduce()
🔥 6-mark array functions answer

Just tell me!
Alright Krushna, let’s blast through these two **4-mark answers**—clean, short, exam-ready. 💥📚

---

# **(c) Create a list in HTML and using CSS change the bullet to lower alphabet and start numbering from 'c'.**

### **HTML + CSS Code (simple & small)**

```html
<!DOCTYPE html>
<html>
<head>
<style>
    ol {
        list-style-type: lower-alpha; /* a, b, c, d... */
    }
</style>
</head>
<body>

<ol start="3">   <!-- Starting with 'c' because c is 3rd alphabet -->
    <li>Apple</li>
    <li>Banana</li>
    <li>Mango</li>
</ol>

</body>
</html>
```

### **Explanation (short)**

* `list-style-type: lower-alpha;` → bullets become **a, b, c...**
* `start="3"` → numbering begins from **c** (c = 3rd in alphabet).

---

# **(d) GET Method in Forms (4-mark answer)**

### **When do we submit data using GET?**

* When the data is **not sensitive** (like search boxes).
* When we want data to be visible in the **URL**.
* When bookmarking or sharing the URL with parameters is useful.

### **How is data sent to the server?**

* Data is appended to the URL as a **query string** after a `?`
  Example:
  `example.com/search?name=krushna&age=20`

### **Which attribute holds the server address?**

* The **`action`** attribute of the `<form>` tag.

Example:

```html
<form action="process.php" method="get">
```

---

If you want, I can also convert these into exact **exam 4-marker paragraphs**.
