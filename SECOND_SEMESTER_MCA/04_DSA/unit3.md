

## 🔷 1. **Bubble Sort**

✅ **Idea**:
Repeatedly compare **adjacent elements** and **swap** them if they are in the wrong order. Largest element "bubbles" to the end in each pass.

🧠 **Example** (for array `[5, 3, 1]`):

* Compare 5 & 3 → swap → `[3, 5, 1]`
* Compare 5 & 1 → swap → `[3, 1, 5]`
* Again compare 3 & 1 → swap → `[1, 3, 5]`

🕐 **Time Complexity**:

* Best: `O(n)` (already sorted)
* Worst: `O(n²)`
* Space: `O(1)`

---

## 🔷 2. **Insertion Sort**

✅ **Idea**:
Build the sorted array **one element at a time**, like sorting playing cards. Pick an element and insert it at the right place in the sorted part.

🧠 **Example** (for `[5, 3, 1]`):

* Start with 5 (sorted)
* Insert 3 before 5 → `[3, 5]`
* Insert 1 before 3 → `[1, 3, 5]`

🕐 **Time Complexity**:

* Best: `O(n)`
* Worst: `O(n²)`
* Space: `O(1)`

---

## 🔷 3. **Selection Sort**

✅ **Idea**:
Find the **smallest element** and put it at the beginning. Then find the next smallest, and so on.

🧠 **Example** (for `[5, 3, 1]`):

* Smallest is 1 → swap with 5 → `[1, 3, 5]`
* Already sorted now

🕐 **Time Complexity**:

* Best/Worst: `O(n²)`
* Space: `O(1)`

---

## 🔷 4. **Quick Sort**

✅ **Idea**:
Choose a **pivot**, and **partition** the array such that:

* Left = elements < pivot
* Right = elements > pivot
  Then recursively sort left and right.

🧠 **Example** for `[5, 3, 8, 1]`, pivot = 5

* Left = `[3, 1]`, Right = `[8]`
* Recursively sort both

🕐 **Time Complexity**:

* Best/Average: `O(n log n)`
* Worst: `O(n²)` (if badly partitioned)
* Space: `O(log n)` (recursive stack)

---

## 🔷 5. **Merge Sort**

✅ **Idea**:
**Divide** the array into halves until size = 1, then **merge** back in sorted order.

🧠 Example for `[8, 4, 2, 6]`

* Split → `[8, 4]`, `[2, 6]`
* Split again → `[8] [4]` & `[2] [6]`
* Merge → `[4, 8]` & `[2, 6]` → Final: `[2, 4, 6, 8]`

🕐 **Time Complexity**:

* Best/Worst/Average: `O(n log n)`
* Space: `O(n)` (for merge arrays)

---

## 🔷 6. **Heap & Heap Sort**

✅ **Idea**:

* A **heap** is a special binary tree where the parent is always greater (Max Heap) or smaller (Min Heap) than its children.
* **Heap Sort**: Build a max heap, remove the root (max), and repeat.

🧠 Example:
Array `[4, 10, 3, 5]` → Max heap: `[10, 5, 3, 4]`
Remove 10, adjust heap → continue

🕐 **Time Complexity**:

* All cases: `O(n log n)`
* Space: `O(1)` (in-place)

---

## 🔷 7. **Radix Sort**

✅ **Idea**:
Sort elements **digit by digit** starting from the least significant digit (LSD) using a stable sort (like counting sort).

🧠 Example:
Sort `[170, 45, 75, 90, 802]`

* Sort by units → tens → hundreds
* Final result = `[45, 75, 90, 170, 802]`

🕐 **Time Complexity**:

* `O(nk)`, where **k = number of digits**
* Best for fixed-length integers
* Space: `O(n + k)`

---

## 📊 Final Comparison Table:

| Algorithm      | Best       | Average    | Worst      | Stable | In-Place             | Space    |
| -------------- | ---------- | ---------- | ---------- | ------ | -------------------- | -------- |
| Bubble Sort    | O(n)       | O(n²)      | O(n²)      | ✅      | ✅                    | O(1)     |
| Insertion Sort | O(n)       | O(n²)      | O(n²)      | ✅      | ✅                    | O(1)     |
| Selection Sort | O(n²)      | O(n²)      | O(n²)      | ❌      | ✅                    | O(1)     |
| Quick Sort     | O(n log n) | O(n log n) | O(n²)      | ❌      | ✅                    | O(log n) |
| Merge Sort     | O(n log n) | O(n log n) | O(n log n) | ✅      | ❌ (uses extra array) | O(n)     |
| Heap Sort      | O(n log n) | O(n log n) | O(n log n) | ❌      | ✅                    | O(1)     |
| Radix Sort     | O(nk)      | O(nk)      | O(nk)      | ✅      | ❌                    | O(n+k)   |

---

## 🎯 Summary for Exams:

* Use **Bubble/Insertion** for small or nearly sorted data.
* Use **Merge/Quick** for large data.
* Use **Heap Sort** if you need **in-place sorting with good performance**.
* Use **Radix Sort** for **integers with fixed length**.

---

Let me know if you want C code or diagrams for any of these! 🧠💻
