Got you bro — here’s a **clean, exam-ready explanation** of
**“JavaScript and Objects”** + **“JavaScript Built-in Objects”** with examples.
Short, clear, and full-marks friendly. 🔥📚

---

# ✅ **1. JavaScript and Objects**

JavaScript is an **object-based** (not purely object-oriented) language.
Objects in JavaScript are collections of **key–value pairs** (properties + methods).

Anything that represents real-world data or a structure can be stored as an object.

---

## ⭐ **A) Creating an Object (Object Literal)**

```javascript
let student = {
    name: "Krushna",
    age: 22,
    course: "MCA",
    greet: function () {
        console.log("Hello, " + this.name);
    }
};
```

* `name`, `age`, `course` → **properties**
* `greet()` → **method**

Accessing properties:

```javascript
console.log(student.name);      // dot notation
console.log(student["age"]);    // bracket notation
student.greet();
```

---

## ⭐ **B) Creating Objects Using Constructor Function**

```javascript
function Person(name, age) {
    this.name = name;
    this.age = age;
}

let p1 = new Person("Krushna", 22);
```

---

## ⭐ **C) Why Objects Are Important in JavaScript**

* They store structured data
* They represent real-world entities
* Built-in features like arrays, dates, math operations are implemented as objects
* DOM manipulation uses objects

---

# ✅ **2. JavaScript Built-in Objects**

JavaScript provides many **predefined (built-in) objects** that help perform common tasks.

Here are the most important ones:

---

# ⭐ **A) String Object**

Used to work with text.

### Example:

```javascript
let s = "Hello";
console.log(s.length);        // 5
console.log(s.toUpperCase()); // HELLO
```

---

# ⭐ **B) Number Object**

Used for numeric operations.

### Example:

```javascript
let n = 123.45;
console.log(n.toFixed(1));   // "123.5"
```

---

# ⭐ **C) Boolean Object**

Represents true/false.

```javascript
let x = Boolean(0); // false
```

---

# ⭐ **D) Array Object**

Stores multiple values in a single variable.

### Example:

```javascript
let arr = [10, 20, 30];
console.log(arr.length);    // 3
console.log(arr.push(40));  // adds new element
```

---

# ⭐ **E) Math Object**

Provides mathematical constants and functions.

### Example:

```javascript
console.log(Math.sqrt(25));   // 5
console.log(Math.random());   // random number (0–1)
```

---

# ⭐ **F) Date Object**

Used to work with dates and time.

### Example:

```javascript
let d = new Date();
console.log(d.getFullYear());
console.log(d.getMonth() + 1);
```

---

# ⭐ **G) JSON Object**

Used for data exchange between server and browser.

### Example:

```javascript
let obj = { name: "Krushna", age: 22 };
let str = JSON.stringify(obj);  // convert object → string
let back = JSON.parse(str);     // convert string → object
```

---

# ⭐ **H) RegExp Object**

Used for pattern matching.

```javascript
let pattern = /hello/i;
console.log(pattern.test("Hello World")); // true
```

---

# 🎯 **Short Summary (Perfect for Exams)**

### ✔ **JavaScript Objects**

Collections of key-value pairs that store structured data and behavior.
Created using literals, constructors, or classes.

### ✔ **Built-in Objects**

Ready-made objects provided by JavaScript such as:
**String, Number, Boolean, Array, Math, Date, JSON, RegExp**

They provide built-in methods for text handling, math operations, arrays, dates, and more.

---

If you want bro, I can turn this into a **6-mark long answer** or **pointwise notes**.
