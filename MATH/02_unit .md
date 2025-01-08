### **Algorithm for Bubble Sort**:
Bubble Sort repeatedly compares adjacent elements and swaps them if they are in the wrong order. It "bubbles" the largest element to the end in each pass.

---

**Bubble Sort Algorithm**:
1. **Input**: An array `A` of size `n`.
2. **Steps**:
   - For `i` from `0` to `n-2` (outer loop for passes):
     1. For `j` from `0` to `n-2-i` (inner loop for comparisons):
        - If `A[j] > A[j+1]`:
          - Swap `A[j]` and `A[j+1]`.
   - Repeat until the array is sorted.
3. **Output**: A sorted array.

---

**Pseudo-code**:

```plaintext
BubbleSort(A[], n):
    for i = 0 to n-2:
        for j = 0 to n-2-i:
            if A[j] > A[j+1]:
                swap(A[j], A[j+1])
```

**Time Complexity**:
- Best Case (already sorted): **O(n)**
- Worst Case (reverse sorted): **O(n²)**

---

### **Algorithm for Insertion Sort**:
Insertion Sort builds the sorted array one element at a time by comparing and inserting the element into its correct position.

---

**Insertion Sort Algorithm**:
1. **Input**: An array `A` of size `n`.
2. **Steps**:
   - For `i` from `1` to `n-1`:
     1. Store `key = A[i]` (current element to insert).
     2. Set `j = i-1` (start comparing with previous elements).
     3. While `j >= 0` and `A[j] > key`:
        - Shift `A[j]` to `A[j+1]`.
        - Decrement `j` by 1.
     4. Place `key` at position `j+1`.
3. **Output**: A sorted array.

---

**Pseudo-code**:

```plaintext
InsertionSort(A[], n):
    for i = 1 to n-1:
        key = A[i]
        j = i - 1
        while j >= 0 and A[j] > key:
            A[j+1] = A[j]
            j = j - 1
        A[j+1] = key
```

**Time Complexity**:
- Best Case (already sorted): **O(n)**
- Worst Case (reverse sorted): **O(n²)**

---

### **Comparison**:
| Feature          | Bubble Sort          | Insertion Sort       |
|-------------------|----------------------|----------------------|
| Best Time Complexity | O(n) (already sorted) | O(n) (already sorted) |
| Worst Time Complexity | O(n²)              | O(n²)              |
| Stability         | Stable               | Stable              |
| Use Case          | Rarely used          | Useful for small datasets or nearly sorted arrays |

Let me know if you need further clarification or implementation examples!
