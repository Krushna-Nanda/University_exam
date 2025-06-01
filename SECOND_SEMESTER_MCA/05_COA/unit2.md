---

## ✅ Q3. Define the term pipelining. Distinguish between Instruction pipeline and Arithmetic Pipeline. Explain different types of hazards that occur in instruction pipeline and how to handle them. (16 Marks)

---

### 🔹 Definition of Pipelining (2 Marks)
* Pipelining is a technique used in modern computer architecture to improve the performance of a processor.
It allows multiple instructions to be executed simultaneously by dividing the process into separate stages.
It divides the instruction execution process into separate stages (like Fetch, Decode, Execute, etc.).

---

### 🔹 Instruction Pipeline vs Arithmetic Pipeline (4 Marks)

#### 🔸 Instruction Pipeline:

* Used to execute multiple instructions in a program in a pipeline fashion.
* Common stages: Instruction Fetch, Instruction Decode, Execute, Memory Access, and Write Back.
* Suitable for general-purpose instructions like Load, Store, Add, etc.
* Example: While one instruction is being executed, the next is being decoded, and a third is being fetched.

#### 🔸 Arithmetic Pipeline:

* Used to break down a complex arithmetic operation into stages.
* Each stage performs a part of the operation like multiplication, addition, or normalization.
* Mostly used in floating point units or high-speed multipliers.
* Example: Performing a floating point multiplication using multiple pipeline stages like partial product generation and summation.

---
---
 What is a Hazard?
A hazard is a situation that causes a delay or stall in instruction pipeline execution.

It prevents the next instruction from executing in its expected clock cycle.

Hazards reduce the performance and speed of pipelining.

 Types of Hazards in Instruction Pipeline (6 Marks)
🔸 1. Data Hazard:
Occurs when an instruction depends on the result of a previous instruction which has not yet completed.

Example:

Instruction 1: ADD R1, R2 → R3

Instruction 2: SUB R3, R4 → R5

Here, Instruction 2 needs the updated value of R3 from Instruction 1, which may not be available yet.

🔸 2. Control Hazard:
Occurs due to branch instructions like if, goto, or loops.

The CPU does not know which instruction to fetch next until the branch decision is made.

This can lead to incorrect instruction fetching and requires correction.

🔸 3. Structural Hazard:
Happens when hardware resources are insufficient or shared between instructions.

Example: Both instructions need to access memory at the same time, but there is only one memory unit.

This causes one instruction to wait, leading to a delay.

---


### 🔹 Techniques to Handle Hazards (4 Marks)

#### 🔸 Handling Data Hazards:

* **Forwarding (Bypassing)**: Sends the result of an operation directly to the next instruction without waiting to store it in the register.
* **Stalling (Pipeline Interlock)**: Delays the execution of dependent instruction until the required data is ready.

#### 🔸 Handling Control Hazards:

* **Branch Prediction**: CPU predicts the outcome of a branch and fetches instructions accordingly.
* **Branch Delay Slot**: Places a useful instruction after the branch to reduce waste.
* **Flushing**: If the prediction was wrong, the incorrect instructions are removed (flushed) from the pipeline.

#### 🔸 Handling Structural Hazards:

* **Resource Duplication**: Add more hardware units like separate instruction and data memory.
* **Instruction Scheduling**: Rearrange the instructions to avoid conflict for resources.

---

### 🔹 Conclusion:

* Pipelining is essential for achieving high instruction throughput in modern processors.
* Although hazards reduce its efficiency, they can be minimized using proper hardware techniques like forwarding, prediction, and resource duplication.

---

