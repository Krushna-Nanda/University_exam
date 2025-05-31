## ✅ Q. Write the taxonomy of parallel architectures with neat diagram. Compare and contrast centralized shared-memory architecture and distributed shared memory architecture. (16 Marks)
---

### ✍️ **Introduction: Flynn’s Taxonomy**

* Parallel architecture means multiple processors work together to do tasks faster.
* To understand these systems, Flynn’s Taxonomy classifies them based on:

  * **Instruction stream:** sequence of instructions sent to processors
  * **Data stream:** sequence of data being processed
* Using these, Flynn defined 4 types of architectures, which is the most used model to understand parallel computers.

---

#### ➤ 1. SISD (Single Instruction, Single Data)

* This is the simplest form of architecture.
* A **single processor** executes one instruction at a time on a single piece of data.
* These systems work sequentially and are used in basic microprocessors.
* **Example**: 8085 microprocessor, single-core systems.

---

#### ➤ 2. SIMD (Single Instruction, Multiple Data)

* A single instruction operates on **multiple data elements** in parallel.
* It is useful for tasks like image processing or matrix operations.
* This type of architecture is used in **vector and graphics processors**.
* **Example**: GPU (Graphics Processing Unit), vector processors.

---

#### ➤ 3. MISD (Multiple Instruction, Single Data)

* Multiple instructions are executed on the **same data item**.
* This type is extremely rare and mostly used in **fault-tolerant systems**.
* It increases reliability by using different methods to process the same data.
* **Example**: Redundant systems in aerospace or defense.

---

#### ➤ 4. MIMD (Multiple Instruction, Multiple Data)

* Multiple processors work independently on different data with different instructions.
* This is the most common architecture used in modern multiprocessors.
* **Example**: Multicore CPUs like Intel i7, AMD Ryzen, supercomputers.

---

## ✍️ **2. Centralized Shared Memory Architecture**

* In this architecture, all processors **share a single common memory**.
* The memory is accessed through a **shared bus** or interconnection system.
* It provides a **uniform memory model**, where all processors can access data directly.
* This model is easier to program and manage.

**Example**: Dual-core or quad-core processors using shared RAM.

**Advantages**:

* Simple to design and program.
* Fast communication among processors (for small systems).

**Disadvantages**:

* As more processors are added, the **bus becomes a bottleneck**.
* **Limited scalability**, suitable only for small multiprocessor systems.

---

## ✍️ **3. Distributed Shared Memory (DSM) Architecture**

* In this system, each processor has **its own private memory**.
* Processors communicate with each other using **message passing**.
* However, the system provides a **shared memory abstraction** using software.

**Example**: Cluster computers, cloud-based parallel systems.

**Advantages**:

* **Highly scalable** — works well even with hundreds of processors.
* Reduces traffic on a single memory bus.

**Disadvantages**:

* **Memory consistency** becomes harder to maintain.
* Data access may be slower due to network communication.

---

## ✅ **4. Differences Between Centralized and Distributed Shared Memory**

### ➤ Centralized Shared Memory:

* One global memory shared by all processors.
* Easier to program.
* Suitable for small-scale systems.
* Memory access is faster but not scalable.

### ➤ Distributed Shared Memory:

* Each processor has its own memory.
* Communication is done through messages.
* Suitable for large-scale, distributed systems.
* More complex, but scalable.

---

## ✅ **Conclusion**

Flynn’s taxonomy helps us understand the different types of parallel architectures based on instruction and data streams. Among these, **MIMD** is the most widely used today.
When designing multiprocessor systems, we choose between **centralized shared memory** (simple but limited) and **distributed shared memory** (complex but scalable), depending on the system's size and performance needs.

---

Alright, here’s clear, crisp, and easy-to-understand answers for both your questions — perfect for exams!

---

### k) Explain the memory consistency issue in a shared memory architecture.

* **Memory consistency** means ensuring all processors in a shared memory system **see the same values** when they access shared data.
* The problem: When multiple processors read and write to the same memory locations, **updates by one processor may not be immediately visible to others**.
* This can cause processors to have **different views of memory at the same time**, leading to errors and unpredictable results.
* For example, if Processor A updates a variable, Processor B might still read the old value because the update hasn't been shared or synchronized yet.
* **Consistency models** (like Sequential Consistency, Weak Consistency) define rules to manage how and when updates become visible to all processors.
* Ensuring memory consistency is **challenging** and requires hardware or software techniques like cache coherence protocols and memory barriers.

---

### l) Write short notes on cluster computing.

* **Cluster computing** is a type of distributed computing where multiple independent computers (called nodes) are connected through a network to work together as a single system.
* Nodes in a cluster share resources like processing power, storage, and data to perform tasks more efficiently and reliably.
* Clusters are used for high-performance computing, big data processing, scientific simulations, and web services.
* Advantages include **scalability** (add more nodes to increase power), **fault tolerance** (if one node fails, others keep working), and **cost-effectiveness** (uses off-the-shelf hardware).
* Examples: Google’s data centers, supercomputers made from clusters of PCs.
* Clusters can be managed by software that schedules tasks and manages communication between nodes.

---

Want me to make these answers more detailed or add examples?


