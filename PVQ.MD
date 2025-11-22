Based on the images provided, here is the exact transcription of the Operating System examination paper, organized by the sections visible in the documents.

### **Exam Header Details**
* **Examination:** 1st Semester Regular/Back Examination: 2022-23
* **Subject:** Operating System
* **Branch(S):** MCA (2 Yrs)
* **Time:** 3 Hours
* **Max Marks:** 100
* **Q.Code:** L625

---

### **Part-I**
**Answer Question No.1 (Part-1) which is compulsory.**
*(2 x 10 = 20 Marks)*

**Q1. Answer the following questions:**
* **a)** What do you mean by spooling? Give one example.
* **b)** Differentiate between hard real time and soft real time operating system.
* **c)** What is problem of priority scheduling? Write down its solution.
* **d)** Write the difference between light weight process and heavy weight process.
* **e)** At a particular time of computation, the value of a counting semaphore is 7, then 20 P-operation and 15 V-operation were completed on the semaphore. What is the resulting value of semaphore?
* **f)** What is spinlock? Write down its advantages.
* **g)** What is Belady anomaly? Why it occurs?
* **h)** Let an instruction takes i ms and page fault takes additional j ms. If the average page fault after k instruction what is the average instruction time.
* **i)** If page size is 4KB and logical addresses 22 bits, what is the number of entries in page table?
* **j)** Differentiate between direct access and sequential access of file accessing method.

---

### **Part-II**
**Only Focused-Short Answer Type Questions- (Answer Any Eight out of Twelve)**
*(6 x 8 = 48 Marks)*

**Q2.**
* **a)** Define thread. What are similarities and differences between thread and process?
* **b)** Differentiated between deadlock and starvation. State four conditions of deadlock.
* **c)** Define process. Explain different states of a process with the help of state diagram.
* **d)** What is race condition? What are all the conditions that should hold good for its solution?
* **e)** Distinguish between multiprogramming and multiprocessing. What is the key motivation for the development of each one?
* **f)** Consider a system with main memory access line of 100ns and TLB access time=20ns TLB hit ratio=95%
    What is effective memory access time with and without TLB?
* **g)** Explain the structure of a disk with neat diagram. * **h)** Write the difference between paging and segmentation.
* **i)** How does the system detect thrashing? Once it detects thrashing, what can the system do to eliminate this problem?
* **j)** Explain contiguous linked and index allocation of disk space with its relative advantages and disadvantages.
* **k)** Given a memory partition of 200k, 500k, 300k and 600k (in order). How would each of first-fit, best-fit, worst-fit algorithms place processes of 212 k, 417 k, 112 k and 426 k(in order)? Which algorithm makes the most efficient use of memory?
* **l)** Define virtual memory. What are the implementation techniques of Virtual memory

---

### **Part-III**
**Only Long Answer Type Questions (Answer Any Two out of Four)**
*(16 Marks each)*

**Q3.**
* **a)** What are the major activities of an operating system? What are the main advantages of layered approach to system design? (8)
* **b)** Consider the following set of processes, with the arrival times and CPU burst time given in ms (8)

| Process | Arrival Time | Burst Time |
| :--- | :--- | :--- |
| P1 | 0 | 5 |
| P2 | 1 | 3 |
| P3 | 2 | 3 |
| P4 | 4 | 1 |

What is average turnaround time (average waiting and average response time) for these processes with the Shortest Remaining Processing Time First?

**Q4.**
* **a)** What is the producer consumer problem? Write down solutions for producer consumer problem? (8)
* **b)** Consider the following snapshot of a system (8)

| | **ALLOCATION** | **MAX** | **AVAILABLE** |
| :--- | :--- | :--- | :--- |
| **PR** | **A B C D** | **A B C D** | **A B C D** |
| $P_0$ | 0 0 1 2 | 0 0 1 2 | 1 5 2 0 |
| $P_1$ | 1 0 0 0 | 1 7 5 0 | |
| $P_2$ | 1 3 5 4 | 2 3 5 6 | |
| $P_3$ | 0 6 3 2 | 0 6 5 2 | |
| $P_4$ | 0 0 1 4 | 0 6 5 6 | |

Answer the following questions using the Banker's algorithm:
(i) What is the content of matrix Need?
(ii) Is the system in a safe state? If yes, what is the safe sequence? Show the detailed steps as per Banker's Algorithm.

**Q5.**
* **a)** Suppose we have a disk with 512 cylinders, and the disk is currently at cylinder 110(and has previously just processed a request for cylinder 105) and the disk queue contains read/write requests for sectors on cylinders 84, 302, 103, 96, 407 and 113. (Cylinders start at number 1). How far must the read travel to satisfy the requests in the queue using FCFS, SCAN, CSCAN and SSTF? (8)
* **b)** A process has been allocated 3 pages frames. Assume that none of pages of the process are available in the memory initially. The process makes the following sequence page reference
    `1 2 1 3 7 4 5 6 3 1`
    What is number of page fault occurs in FIFO, LRU and Optimal Page replacement algorithm? (8)

**Q6.**
* **a)** Define RAID. Explain different level of RAID with its relative advantages and Disadvantages. (8)
* **b)** Consider a Unix system
    10 direct block pointer
    One single indirect Pointer
    One double indirect pointer
    Block Size =8KB
    Disk Size=8KB
    Block Pointer Size= 8B
    What is the Maximum file size? (8)

---
*Would you like me to solve any specific problem from this question paper (e.g., the CPU scheduling problem in Q3b or the Banker's Algorithm in Q4b)?*


Based on the images provided, here is the exact transcription of the Operating System examination paper, organized by the sections visible in the documents.

### **Exam Header Details**
* **Examination:** 1st Semester Regular/Back Examination: 2022-23
* **Subject:** Operating System
* **Branch(S):** MCA (2 Yrs)
* **Time:** 3 Hours
* **Max Marks:** 100
* **Q.Code:** L625

---

### **Part-I**
**Answer Question No.1 (Part-1) which is compulsory.**
*(2 x 10 = 20 Marks)*

**Q1. Answer the following questions:**
* **a)** What do you mean by spooling? Give one example.
* **b)** Differentiate between hard real time and soft real time operating system.
* **c)** What is problem of priority scheduling? Write down its solution.
* **d)** Write the difference between light weight process and heavy weight process.
* **e)** At a particular time of computation, the value of a counting semaphore is 7, then 20 P-operation and 15 V-operation were completed on the semaphore. What is the resulting value of semaphore?
* **f)** What is spinlock? Write down its advantages.
* **g)** What is Belady anomaly? Why it occurs?
* **h)** Let an instruction takes i ms and page fault takes additional j ms. If the average page fault after k instruction what is the average instruction time.
* **i)** If page size is 4KB and logical addresses 22 bits, what is the number of entries in page table?
* **j)** Differentiate between direct access and sequential access of file accessing method.

---

### **Part-II**
**Only Focused-Short Answer Type Questions- (Answer Any Eight out of Twelve)**
*(6 x 8 = 48 Marks)*

**Q2.**
* **a)** Define thread. What are similarities and differences between thread and process?
* **b)** Differentiated between deadlock and starvation. State four conditions of deadlock.
* **c)** Define process. Explain different states of a process with the help of state diagram.
* **d)** What is race condition? What are all the conditions that should hold good for its solution?
* **e)** Distinguish between multiprogramming and multiprocessing. What is the key motivation for the development of each one?
* **f)** Consider a system with main memory access line of 100ns and TLB access time=20ns TLB hit ratio=95%
    What is effective memory access time with and without TLB?
* **g)** Explain the structure of a disk with neat diagram. * **h)** Write the difference between paging and segmentation.
* **i)** How does the system detect thrashing? Once it detects thrashing, what can the system do to eliminate this problem?
* **j)** Explain contiguous linked and index allocation of disk space with its relative advantages and disadvantages.
* **k)** Given a memory partition of 200k, 500k, 300k and 600k (in order). How would each of first-fit, best-fit, worst-fit algorithms place processes of 212 k, 417 k, 112 k and 426 k(in order)? Which algorithm makes the most efficient use of memory?
* **l)** Define virtual memory. What are the implementation techniques of Virtual memory

---

### **Part-III**
**Only Long Answer Type Questions (Answer Any Two out of Four)**
*(16 Marks each)*

**Q3.**
* **a)** What are the major activities of an operating system? What are the main advantages of layered approach to system design? (8)
* **b)** Consider the following set of processes, with the arrival times and CPU burst time given in ms (8)

| Process | Arrival Time | Burst Time |
| :--- | :--- | :--- |
| P1 | 0 | 5 |
| P2 | 1 | 3 |
| P3 | 2 | 3 |
| P4 | 4 | 1 |

What is average turnaround time (average waiting and average response time) for these processes with the Shortest Remaining Processing Time First?

**Q4.**
* **a)** What is the producer consumer problem? Write down solutions for producer consumer problem? (8)
* **b)** Consider the following snapshot of a system (8)

| | **ALLOCATION** | **MAX** | **AVAILABLE** |
| :--- | :--- | :--- | :--- |
| **PR** | **A B C D** | **A B C D** | **A B C D** |
| $P_0$ | 0 0 1 2 | 0 0 1 2 | 1 5 2 0 |
| $P_1$ | 1 0 0 0 | 1 7 5 0 | |
| $P_2$ | 1 3 5 4 | 2 3 5 6 | |
| $P_3$ | 0 6 3 2 | 0 6 5 2 | |
| $P_4$ | 0 0 1 4 | 0 6 5 6 | |

Answer the following questions using the Banker's algorithm:
(i) What is the content of matrix Need?
(ii) Is the system in a safe state? If yes, what is the safe sequence? Show the detailed steps as per Banker's Algorithm.

**Q5.**
* **a)** Suppose we have a disk with 512 cylinders, and the disk is currently at cylinder 110(and has previously just processed a request for cylinder 105) and the disk queue contains read/write requests for sectors on cylinders 84, 302, 103, 96, 407 and 113. (Cylinders start at number 1). How far must the read travel to satisfy the requests in the queue using FCFS, SCAN, CSCAN and SSTF? (8)
* **b)** A process has been allocated 3 pages frames. Assume that none of pages of the process are available in the memory initially. The process makes the following sequence page reference
    `1 2 1 3 7 4 5 6 3 1`
    What is number of page fault occurs in FIFO, LRU and Optimal Page replacement algorithm? (8)

**Q6.**
* **a)** Define RAID. Explain different level of RAID with its relative advantages and Disadvantages. (8)
* **b)** Consider a Unix system
    10 direct block pointer
    One single indirect Pointer
    One double indirect pointer
    Block Size =8KB
    Disk Size=8KB
    Block Pointer Size= 8B
    What is the Maximum file size? (8)

---
*Would you like me to solve any specific problem from this question paper (e.g., the CPU scheduling problem in Q3b or the Banker's Algorithm in Q4b)?*