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


Alright Krushna, here's a **simple, clean, perfect 6-mark answer** — not too big, not too small, exactly exam style. 🔥📚

---

# ✅ **What is an Event in JavaScript?**

An **event** in JavaScript is an action or occurrence that happens in the browser and can be detected by JavaScript.
Events are used to make webpages interactive.
Common actions like clicking a button, typing in a textbox, moving the mouse, or loading a page are all considered **events**.

---

# ✅ **Examples of JavaScript Events**

Some commonly used events are:

* **onclick** – fires when a user clicks a button or element
* **onchange** – fires when the value of a form element changes
* **onmouseover** – fires when the mouse pointer moves over an element
* **onload** – fires when the webpage finishes loading
* **onkeydown** – fires when a key is pressed

---

# ✅ **HTML + JavaScript Program**

When the user enters text and clicks the button, the text becomes **uppercase**.

```html
<!DOCTYPE html>
<html>
<head>
<title>Uppercase Converter</title>
</head>
<body>

<h3>Convert Text to Uppercase</h3>

<input type="text" id="txt">
<button onclick="makeUpper()">Convert</button>

<script>
function makeUpper() {
    let input = document.getElementById("txt");
    input.value = input.value.toUpperCase();
}
</script>

</body>
</html>
```

---

# ✅ **Explanation (short)**

* `onclick` event is used on the button.
* When the button is clicked, the function `makeUpper()` runs.
* It reads the value of the text field and converts it to **uppercase** using `.toUpperCase()`.
* The updated value is placed back into the text box.

---

If you want this in **strict paragraph format** for writing in exams, tell me and I’ll convert it!



Alright Krushna, here’s a **simple, exam-perfect JavaScript solution** to find all **four perfect numbers below 10,000**.
(No fancy stuff — clean loop + function.)

---

# ✅ **JavaScript Function to Find Perfect Numbers Below 10,000**

```javascript
function findPerfectNumbers() {
    let perfects = [];

    for (let num = 1; num < 10000; num++) {
        let sum = 0;

        // Find divisors of num
        for (let i = 1; i <= num / 2; i++) {
            if (num % i === 0) {
                sum += i;
            }
        }

        // Check perfect number
        if (sum === num) {
            perfects.push(num);
        }
    }

    return perfects;
}

console.log(findPerfectNumbers());
```

---

# ✅ **Output**

The four perfect numbers below 10,000 are:

```
6, 28, 496, 8128
```

---

# ✅ **Explanation (short & exam-ready)**

* A number is perfect if the sum of its **proper divisors** (excluding itself) equals the number.
* Loop through numbers from **1 to 9999**.
* For each number, find divisors using a loop up to `num / 2`.
* Add the divisors, compare with the number.
* If equal → it's a perfect number.

---

If you want the same answer in **paragraph form** for writing in theory exams, just say the word!



Got you, bro — here’s a **super simple, exam-friendly HTML + JavaScript program** to reverse a string. 💯

No extra styling, just clean code.

---

# ✅ **HTML + JavaScript Program to Reverse a String**

```html
<!DOCTYPE html>
<html>
<head>
<title>Reverse String</title>
</head>
<body>

<h3>Reverse a String</h3>

<input type="text" id="str">
<button onclick="reverseString()">Reverse</button>

<p id="result"></p>

<script>
function reverseString() {
    let text = document.getElementById("str").value;
    let reversed = text.split("").reverse().join("");
    document.getElementById("result").innerHTML = "Reversed: " + reversed;
}
</script>

</body>
</html>
```

---

# ✅ **How it works (short explanation)**

* `split("")` breaks the string into characters
* `reverse()` reverses the array
* `join("")` puts it back into a string
* Output is displayed inside `<p id="result">`

---

If you want a **2-mark or 6-mark theory explanation** along with the program, I can whip that up too!


Nice big batch — let’s smash it in one go. I’ll keep each part short, exam-friendly, and give working HTML+JS (and CSS where asked). You can copy-paste each block into a file and run it.

---

# 1) What is an object in JavaScript + create `person` object and display it

**Definition (short):**
An **object** in JavaScript is a collection of key-value pairs (properties) and/or methods. It stores related data and behaviour.

**HTML + JS to create `person` and display details:**

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Person Object Display</title>
</head>
<body>
  <h3>Person Details</h3>
  <div id="personDetails"></div>

  <script>
    // Create person object
    const person = {
      firstName: "Priyanka",
      lastName: "Murmu",
      age: 50,
      eyeColor: "blue"
    };

    // Display on page
    const output = document.getElementById("personDetails");
    output.innerHTML =
      "<p>First Name: " + person.firstName + "</p>" +
      "<p>Last Name: " + person.lastName + "</p>" +
      "<p>Age: " + person.age + "</p>" +
      "<p>Eye Colour: " + person.eyeColor + "</p>";
  </script>
</body>
</html>
```

---

# 2) Leap year function (takes year and displays whether leap year or not)

**Rule:** Year is leap if divisible by 400 or (divisible by 4 and not by 100).

**HTML + JS:**

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Leap Year Checker</title>
</head>
<body>
  <h3>Leap Year Checker</h3>
  <input type="number" id="yearInput" placeholder="Enter year">
  <button onclick="checkLeap()">Check</button>
  <p id="leapResult"></p>

  <script>
    function isLeapYear(year) {
      return (year % 400 === 0) || (year % 4 === 0 && year % 100 !== 0);
    }

    function checkLeap() {
      const y = parseInt(document.getElementById('yearInput').value, 10);
      const res = document.getElementById('leapResult');
      if (isNaN(y)) {
        res.textContent = "Please enter a valid year.";
        return;
      }
      res.textContent = y + (isLeapYear(y) ? " is a leap year." : " is NOT a leap year.");
    }
  </script>
</body>
</html>
```

---

# 3) Use of string functions in JavaScript with examples

Provide short examples (each one-liner plus explanation):

```javascript
// i. trim()  — removes whitespace from both ends
let s1 = "   hello world   ";
console.log(s1.trim()); // "hello world"

// ii. charAt() — returns character at given index (0-based)
let s2 = "JavaScript";
console.log(s2.charAt(4)); // "S"

// iii. concat() — joins strings (can use + as well)
let a = "Hello";
let b = "Krushna";
console.log(a.concat(" ", b)); // "Hello Krushna"

// iv. split() — splits string into array by separator
let s3 = "apple,banana,mango";
console.log(s3.split(",")); // ["apple", "banana", "mango"]

// v. indexOf() — returns index of substring or -1 if not found
let s4 = "programming";
console.log(s4.indexOf("gram")); // 3

// vi. substring() — extracts part of string: substring(start, endExclusive)
let s5 = "HelloWorld";
console.log(s5.substring(0, 5)); // "Hello"
```

(Short exam note: `trim()` removes spaces at ends; `charAt()` returns single character; `concat()` joins strings; `split()` converts string to array; `indexOf()` finds position; `substring()` extracts slice.)

---

# 4) Program to change color of a link depending on visited, hover or active state (HTML/CSS)

**CSS pseudo-classes:** `:link`, `:visited`, `:hover`, `:active`

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Link States</title>
  <style>
    a:link { color: blue; }       /* unvisited link */
    a:visited { color: purple; }  /* visited link */
    a:hover { color: orange; }    /* when mouse over */
    a:active { color: red; }      /* while clicking */
  </style>
</head>
<body>
  <h3>Link State Demo</h3>
  <p><a href="https://example.com" target="_blank">Visit example.com</a></p>
  <p>Click, hover and then revisit to see different states.</p>
</body>
</html>
```

---

# 5) What is an event in JavaScript + program to display full name on submit click

**Definition (short):**
An **event** is an action or occurrence (click, keypress, load, etc.) that the browser detects and you can respond to with JavaScript.

**HTML + JS program:**

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Full Name Display</title>
</head>
<body>
  <h3>Enter Name</h3>
  <label>First Name: <input type="text" id="first"></label><br><br>
  <label>Last Name: <input type="text" id="last"></label><br><br>
  <button id="submitBtn">Submit</button>

  <p id="fullName"></p>

  <script>
    document.getElementById('submitBtn').addEventListener('click', function() {
      const f = document.getElementById('first').value.trim();
      const l = document.getElementById('last').value.trim();
      if (!f && !l) {
        document.getElementById('fullName').textContent = "Please enter first and/or last name.";
        return;
      }
      document.getElementById('fullName').textContent = "Full Name: " + (f + " " + l).trim();
    });
  </script>
</body>
</html>
```

---

# 6) Design a form (HTML + CSS) to register students for a workshop on “Internet of Things”

Simple, neat form with required fields and basic styling.

```html
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>IoT Workshop Registration</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f4f7f9;
      display: flex;
      justify-content: center;
      padding: 30px;
    }
    .form-card {
      background: white;
      padding: 20px 24px;
      border-radius: 8px;
      box-shadow: 0 6px 18px rgba(0,0,0,0.08);
      width: 420px;
    }
    .form-card h2 { margin-top: 0; }
    .form-row { margin-bottom: 12px; }
    label { display:block; font-size:14px; margin-bottom:6px; }
    input[type="text"], input[type="email"], input[type="tel"], select, textarea {
      width: 100%;
      padding: 8px 10px;
      border: 1px solid #ccc;
      border-radius: 4px;
      box-sizing: border-box;
    }
    textarea { resize: vertical; min-height: 80px; }
    .small { font-size:12px; color:#555; }
    .btn {
      background: #0073e6;
      color: white;
      border: none;
      padding: 10px 14px;
      border-radius: 6px;
      cursor: pointer;
      margin-top: 8px;
    }
    .btn:hover { opacity: 0.95; }
  </style>
</head>
<body>
  <div class="form-card">
    <h2>IoT Workshop Registration</h2>

    <form id="regForm">
      <div class="form-row">
        <label>Full Name <span class="small">(required)</span></label>
        <input type="text" id="name" required placeholder="Enter your full name">
      </div>

      <div class="form-row">
        <label>Email <span class="small">(required)</span></label>
        <input type="email" id="email" required placeholder="you@example.com">
      </div>

      <div class="form-row">
        <label>Phone</label>
        <input type="tel" id="phone" placeholder="Optional">
      </div>

      <div class="form-row">
        <label>Institute / Organization</label>
        <input type="text" id="inst" placeholder="Name of college/company">
      </div>

      <div class="form-row">
        <label>Experience Level</label>
        <select id="exp">
          <option>Beginner</option>
          <option>Intermediate</option>
          <option>Advanced</option>
        </select>
      </div>

      <div class="form-row">
        <label>Topics of Interest</label>
        <textarea id="topics" placeholder="e.g., sensors, Raspberry Pi, MQTT"></textarea>
      </div>

      <div class="form-row">
        <label>Preferred Workshop Date</label>
        <input type="text" id="date" placeholder="e.g., 10 Dec 2025">
      </div>

      <button type="button" class="btn" onclick="submitForm()">Register</button>
    </form>

    <p id="confirmation" style="margin-top:12px;color:green;"></p>
  </div>

  <script>
    function submitForm(){
      const name = document.getElementById('name').value.trim();
      const email = document.getElementById('email').value.trim();
      if(!name || !email){
        document.getElementById('confirmation').style.color='red';
        document.getElementById('confirmation').textContent = 'Please fill required fields (Name and Email).';
        return;
      }
      // simple confirmation (in real app you would send to server)
      document.getElementById('confirmation').style.color='green';
      document.getElementById('confirmation').textContent = `Thanks ${name.split(' ')[0]} — registration received!`;
      document.getElementById('regForm').reset();
    }
  </script>
</body>
</html>
```

---

If you want any of these in a single combined file, or need the answers formatted into plain written paragraphs for your exam paper (6-mark / 4-mark style), tell me which ones and I’ll convert them to neat text-only answers.

