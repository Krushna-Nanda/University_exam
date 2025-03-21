Here's a super simplified **SQ (Short Questions) Answer Sheet** for you. Read this 2-3 times, and you'll remember it in 10-20 minutes easily! 🚀  

---

### **Short Questions (SQ) Answers – COA**  

#### **1. What is a Pipeline?**  
A **pipeline** is a technique where multiple instructions are processed in different stages simultaneously, like an assembly line. It increases CPU efficiency and speed.  

#### **2. What are Hazards in Pipelining?**  
Hazards are issues that **stall the pipeline** and reduce efficiency. They are of three types:  
- **Data Hazard** (dependency between instructions, e.g., RAW, WAR, WAW)  
- **Control Hazard** (caused by branch instructions)  
- **Structural Hazard** (hardware limitations, e.g., insufficient memory access)  

#### **3. How to Handle Hazards?**  
- **Data Forwarding** (bypassing)  
- **Stalling** (delaying execution)  
- **Branch Prediction** (guessing the next instruction)  

#### **4. What are RAW, WAR, and WAW?**  
These are **data hazards** in pipelines:  
WAW (Write After Write) – Conflicting Writes
This occurs when two instructions try to write to the same register at the same time, causing data inconsistency.
WAR (Write After Read) – Overwriting Issue
This happens when a later instruction tries to write to a register before an earlier instruction has finished reading from it.
RAW (Read After Write) – Missing Data Issue
This occurs when an instruction tries to read a value before the previous instruction has written it. Since the required data isn’t available yet, the pipeline has to stall. 

#### **5. What is Arithmetic in COA?**  
Arithmetic operations (Addition, Subtraction, Multiplication, and Division) are performed using different hardware units like ALU (Arithmetic Logic Unit).  

#### **6. What is Cache Memory and How is it Mapped?**  
Cache memory is a **small, fast** memory that stores frequently used data. It has **three mapping techniques**:  
- **Direct Mapping** (Each block maps to a fixed location)  
- **Fully Associative Mapping** (Any block can go anywhere)  
- **Set Associative Mapping** (A mix of both)  

#### **7. What is Memory Hierarchy?**  
Memory is arranged in levels based on **speed and size**:  
1. **Registers** (Fastest, smallest)  
2. **Cache Memory**  
3. **RAM (Main Memory)**  
4. **Hard Disk (Slowest, largest)**  

---

**🔥 Quick Revision Trick:**  
Just **visualize the CPU pipeline as a factory** and hazards as "problems" in production. **Cache memory is your quick-access notepad**, and **memory hierarchy is like storage levels from pocket money to bank deposits!**  

Revise this **twice**, and you'll crush your exam! Let me know if you want **super simplified LQ answers too!** 🚀😎
