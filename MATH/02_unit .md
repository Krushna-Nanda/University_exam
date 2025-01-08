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

===================================================================

Here's the **Algorithm** for the **Binary Search** implemented in your code:

---

### **Binary Search Algorithm**:

1. **Input**: 
   - A sorted array `arr[]` of size `n`.
   - A `target` value to search within the array.

2. **Steps**:
   - Initialize `left` to 0 (the first index) and `right` to `n - 1` (the last index).
   - While `left` is less than or equal to `right`:
     1. Compute the middle index: `mid = (left + right) / 2`.
     2. If `arr[mid]` equals `target`, then the target is found at index `mid`, and the search ends.
     3. If `arr[mid]` is less than `target`, set `left = mid + 1` to search the right half of the array.
     4. If `arr[mid]` is greater than `target`, set `right = mid - 1` to search the left half of the array.
   - If the element is found, print the index of the element.
   - If the element is not found, print a message stating that the element is not in the array.

3. **Output**:
   - The index of the `target` if found.
   - A message stating that the `target` is not found if the search is unsuccessful.

---

### **Pseudo-code**:

```plaintext
BinarySearch(arr[], target, n):
    left = 0
    right = n - 1
    
    while left <= right:
        mid = (left + right) / 2
        
        if arr[mid] == target:
            print "Element found at index", mid
            return
        
        if arr[mid] < target:
            left = mid + 1   // Search in right half
        else:
            right = mid - 1  // Search in left half

    print "Element not found in the array"
```

---

This describes the logic behind the binary search, matching the code you provided. It efficiently searches for a target element in a sorted array using the divide-and-conquer approach.

# ========================================================================================

### **Algorithm for Linear Search**:

1. **Input**: 
   - An array `arr[]` of size `n`.
   - A `target` value to search for in the array.

2. **Steps**:
   - Initialize a variable `i` to 0.
   - Traverse the array from index `i = 0` to `i = n-1`:
     1. Compare `arr[i]` with `target`.
     2. If `arr[i] == target`, print the index `i` and terminate the search.
   - If the entire array is traversed and the `target` is not found, print a message indicating that the element is not in the array.

3. **Output**:
   - The index of the `target` if found.
   - A message stating that the `target` is not found if the search is unsuccessful.

---

### **Pseudo-code**:

```plaintext
LinearSearch(arr[], target, n):
    for i = 0 to n-1:
        if arr[i] == target:
            print "Element found at index", i
            return
    print "Element not found in the array"
```

---

This algorithm describes the linear search method, where each element of the array is checked sequentially until the target value is found or the array is fully traversed. Linear search is simple but less efficient than binary search for large arrays.
