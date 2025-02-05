# 2024 COA QUESTION PAPER

Here is the question as it is:  

---

### **Part-I (2 x 10)**  

a) What are the functionalities of program counter, instruction register, and data register?  
b) What is a parallel computer?  
c) What do you mean by Cache coherence?  
d) What are the issue policies for superscalar instructions?  
e) A four-stage pipeline has stage delays as 150, 120, 160 and 140 ns respectively. Registers are used between the stages and have a delay of 5 ns each. Assuming constant clocking rate, calculate the total time taken to process 1000 data items on this pipeline.  
f) What do you mean by logical organization of parallel programming platforms?  
g) Is VLIW a RISC or CISC? Justify.  
h) What is meant by anti-dependence? How is it removed?  
i) What are the disadvantages of using symmetric shared memory?  
j) Given page reference string: 1, 2, 3, 4, 2, 1, 5, 6, 2, 1, 2, 3, 7, 6, 3, 2, 1, 2, 3, 6. Find the number of page faults for optimal page replacement algorithm.  

---

### **Part-II Focused-Short Answer Type Questions (Answer Any Eight out of Twelve) (6 × 8)**  

a) Write the Amdahl’s law and its significance.  
b) Consider a 4-stage pipeline that consists of Instruction Fetch (IF), Instruction Decode (ID), Execute (Ex) and Write Back (WB) stages. The times taken by these stages are 50 ns, 60 ns, 110 ns, and 80 ns respectively. The pipeline registers are required after every pipeline stage, and each of these pipeline register consumes 10ns delay. What is the speedup of the pipeline under ideal conditions compare to the corresponding non-pipelined implementation?  
c) Distinguish between Instruction pipeline and Arithmetic Pipeline.  
d) Explain the memory interleaving technique with suitable example.  
e) A computer has an 8 GByte memory with 64-bit word sizes. Each block of memory stores 16 words. The computer has a direct-mapped cache of 128 blocks. The computer uses word level addressing. What is the address format? If we change the cache to a 4-way set associative cache, what is the new address format?  
f) Describe Flynn’s classification of computer architecture.  
g) What do you mean by Speed-Up of pipeline? Derive equations of Speed-Up and Efficiency for Pipeline, Super pipeline, and Super scalar architecture.  
h) A block-set associative cache consists of a total of 64 blocks divided into 4 blocks sets. The main memory contains 4096 blocks, each consisting of 128 words.  
   - I. How many bits are there in the main memory address?  
   - II. How many bits are there in each of the TAG, SET and WORD fields?  
i) Define demand paging? Explain the various page replacement techniques.  
j) Compare the features of Array Processor and Vector Processors.  
k) Explain memory consistency issue in shared memory architecture.  
l) What is cloud computing explain its characteristics and features?  

---

### **Part-III Long Answer Type Questions (Answer Any Two out of Four)**  

Q3 Define the term pipelining. Distinguish between Instruction pipeline and Arithmetic Pipeline. Explain different types of hazards that occur in instruction pipeline and how to handle them. (16)  

Q4 Describe cache memory and mapping policies with suitable examples. Consider a 16-way set-associative cache having 64 bits long Data words. The cache holds 2 Mbytes of data, and each block holds 16 data words. Physical addresses are 64 bits long. How many bits of tag, index, and offset are needed to support references to this cache? (16)  

Q5 Briefly describe the VLIW processor architecture. What are the differences between a superscalar processor and V.L.I.W. processor? Suppose your program consists of 2500 instructions. The proportion of different kinds of instructions in the program is as follows: Data transfer instruction 50%, arithmetic instruction 30%, and branching related instructions 20%. The cycles consumed by these types of instructions are 2, 5, and 10 respectively. What will be the execution time for a 4 GHz processor to execute your program? (16)  

Q6 Write the taxonomy of parallel architectures with neat diagram. Compare and contrast centralized shared-memory architecture and distributed shared memory architecture. (16)  

---

# 2023 COA QUESTION PAPER

Here is the question as it is:  

---

### **Part-I (2 x 10)**  

a) State and explain Amdahl’s law.  
b) The memory access time is 1 nanosecond for a read operation with a hit in cache, 5 nanoseconds for a read operation with a miss in cache, 2 nanoseconds for a write operation with a hit in cache and 10 nanoseconds for a write operation with a miss in cache. Execution of a sequence of instructions involves 100 instruction fetch operations, 60 memory operand read operations and 40 memory operand write operations. The cache hit-ratio is 0.9. Compute the average memory access time (in nanoseconds) in executing the above sequence of instructions.  
c) Write the procedure of optimal page replacement with a suitable example.  
d) Define arithmetic pipelining.  
e) What do you mean by Cache coherence?  
f) The content of the top of a memory stack is 5320. The content of the stack pointer SP is 3560. A two-word call subroutine instruction is in memory at address 1120 followed by the address field of 6720 at location 1121. What is the content of PC, SP, and the top of the stack?  
g) Give an example of data hazard in a pipeline architecture.  
h) A four-stage pipeline has stage delays as 150, 120, 160 and 140 ns respectively. Registers are used between the stages and have a delay of 5 ns each. Assuming constant clocking rate, calculate the total time taken to process 1000 data items on this pipeline.  
i) Distinguish between Superpipelined and Superscalar processor.  
j) Differentiate between Microprogramming and Hardwired control unit.  

---

### **Part-II (Focused-Short Answer Type Questions) (Answer Any Eight out of Twelve) (6 × 8)**  

a) Design the control unit of a basic computer. A computer has 16 registers, an ALU with 32 operations, and a Shifter with eight operations, all connected to a common bus system.  
   - (a) Formulate a control word for a microoperation.  
   - (b) Specify the number of bits in each field of the control word and give an encoding scheme.  

b) A computer uses chips of 1024x1 capacity.  
   - (a) How many chips are needed and how should their address lines be connected to provide a memory capacity of 1024 bytes?  
   - (b) How many chips are needed to provide a memory capacity of 16 K bytes? Explain in words how the chips are to be connected to the address bus.  

c) Consider the following instruction sequence where registers R1, R2, and R3 are general-purpose, and MEMORY[X] denotes the content at the memory location X:  

| Instruction | Semantics | Instruction Size (bytes) |
|-------------|------------|-------------------------|
| MOV R1, (5000) | R1 ← MEMORY[5000] | 4 |
| MOV R2, (R3) | R2 ← MEMORY[R3] | 4 |
| ADD R2, R1 | R2 ← R1 + R2 | 2 |
| MOV (R3), R2 | MEMORY[R3] ← R2 | 4 |
| INC R3 | R3 ← R3 + 1 | 2 |
| DEC R1 | R1 ← R1 – 1 | 2 |
| BNZ 1004 | Branch if not zero to the given absolute address | 2 |
| HALT | Stop | 1 |

   Assume that the content of the memory location 5000 is 10, and the content of register R3 is 3000. The content of each of the memory locations from 3000 to 3010 is 50. The instruction sequence starts from memory location 1000. All the numbers are in decimal format, and memory is byte-addressable. Find the content of memory location 3010 after the execution of the program.  

d) Assume a cache miss penalty is 100 clock cycles, and all instructions take 1.0 clock cycle. Let the average miss rate be 2%, there is an average of 1.5 memory references per instruction, and the average number of cache misses per 1000 instructions is 30. What is the impact on performance, and calculate the impact using both misses per instruction and miss rate?  

e) What is virtual memory? How is a logical address mapped to a physical address in the virtual concept? Explain with an example and diagram.  

f) What is a Pipeline Hazard? How is a control hazard detected and resolved? Explain with an example.  

g) Define demand paging? Explain the various page replacement techniques.  

h) What are the criteria on which memory hierarchy is formed? What information does it convey? Differentiate between main memory and cache memory.  

i) What is the basic working principle of a VLIW processor? What are the advantages of a VLIW processor?  

j) Compare the features of Array Processor and Vector Processors.  

k) Explain the memory consistency issue in a shared memory architecture.  

l) Write short notes on cluster computing.  

---

### **Part-III (Long Answer Type Questions) (Answer Any Two out of Four) (16 × 2)**  

**Q3.** Define the term pipelining. Distinguish between Instruction pipeline and Arithmetic Pipeline. Explain different types of hazards that occur in instruction pipeline and how to handle them.  

**Q4.** Explain the role of cache in memory hierarchy. Explain direct, associative, and set-associative cache mapping techniques with suitable examples. A block-set associative cache consists of a total of 64 blocks divided into 4 block sets. The main memory contains 4096 blocks, each consisting of 128 words.  

   - (i) How many bits are there in the main memory address?  
   - (ii) How many bits are there in each of the TAG, SET, and WORD fields?  

**Q5.** Discuss the basic concepts for increasing Instruction-Level Parallelism. A superscalar processor has 5 issue slots that can be filled up in a single clock cycle. During execution of a certain application consisting of 1000 instructions, the following observations were made:  

   - 10% of the instructions were issued by filling up exactly 1 issue slot only,  
   - 20% of the instructions were issued by filling up exactly 2 issue slots only,  
   - 20% of the instructions were issued by filling up exactly 3 issue slots only,  
   - 48% of the instructions were issued by filling up exactly 4 issue slots only,  
   - The remaining instructions were issued by filling up all the slots.  

   However, due to some reason, it was found that a total of 500 clock cycles were consumed while issuing all these 1000 instructions. Find out the speedup factor in issuing instructions when there is zero vertical waste compared to the scenario with vertical waste.  

**Q6.** Write the taxonomy of parallel architectures with a neat diagram. Compare and contrast centralized shared-memory architecture and distributed shared memory architecture.  

---

