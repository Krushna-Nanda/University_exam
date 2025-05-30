# 2024

Here are **only** the calculation-based (numerical) questions from your list, without any answers:

1. **(b)** Consider a 4-stage pipeline that consists of Instruction Fetch (IF), Instruction Decode (ID), Execute (Ex) and Write Back (WB) stages. The times taken by these stages are 50 ns, 60 ns, 110 ns, and 80 ns respectively. The pipeline registers are required after every pipeline stage, and each of these pipeline registers consumes 10 ns delay.
   **What is the speedup of the pipeline under ideal conditions compared to the corresponding non-pipelined implementation?**

2. **(e)** A computer has an 8 GByte memory with 64-bit word sizes. Each block of memory stores 16 words. The computer has a direct-mapped cache of 128 blocks. The computer uses word-level addressing.

   * **What is the address format?**
   * **If we change the cache to a 4-way set-associative cache, what is the new address format?**

3. **(g)**

   * **What do you mean by Speed-Up of a pipeline?**
   * **Derive equations for Speed-Up and Efficiency for:**

     1. Pipeline
     2. Super-pipeline
     3. Superscalar architecture

4. **(h)** A block-set-associative cache consists of a total of 64 blocks divided into 4 block-sets. The main memory contains 4096 blocks, each consisting of 128 words.

   1. **How many bits are there in the main memory address?**
   2. **How many bits are there in each of the TAG, SET and WORD fields?**

5. **(Q4)** Describe cache memory and mapping policies with suitable examples.
   **Consider a 16-way set-associative cache having 64-bit data words. The cache holds 2 Mbytes of data, and each block holds 16 data words. Physical addresses are 64 bits long.**
   **How many bits of tag, index, and offset are needed to support references to this cache?**

6. **(Q5)** Briefly describe the VLIW processor architecture. What are the differences between a superscalar processor and VLIW processor?
   **Suppose your program consists of 2500 instructions. The proportion of different kinds of instructions in the program is as follows: Data transfer instructions 50%, arithmetic instructions 30%, and branch instructions 20%. The cycles consumed by these types of instructions are 2, 5, and 10 respectively.**
   **What will be the execution time for a 4 GHz processor to execute your program?**

Let me know if you need anything else!

# 2023

Here are **exactly** the calculation‐oriented questions verbatim, copied from your prompt:

---

**Part-II (Focused-Short Answer Type Questions) (Answer Any Eight out of Twelve) (6 × 8)**

a) Design the control unit of a basic computer. A computer has 16 registers, an ALU with 32 operations, and a Shifter with eight operations, all connected to a common bus system.
  (a) Formulate a control word for a microoperation.
  (b) Specify the number of bits in each field of the control word and give an encoding scheme.

b) A computer uses chips of 1024x1 capacity.
  (a) How many chips are needed and how should their address lines be connected to provide a memory capacity of 1024 bytes?
  (b) How many chips are needed to provide a memory capacity of 16 K bytes? Explain in words how the chips are to be connected to the address bus.

c) Consider the following instruction sequence where registers R1, R2, and R3 are general-purpose, and MEMORY\[X] denotes the content at the memory location X:

| Instruction    | Semantics                                        | Instruction Size (bytes) |
| -------------- | ------------------------------------------------ | ------------------------ |
| MOV R1, (5000) | R1 ← MEMORY\[5000]                               | 4                        |
| MOV R2, (R3)   | R2 ← MEMORY\[R3]                                 | 4                        |
| ADD R2, R1     | R2 ← R1 + R2                                     | 2                        |
| MOV (R3), R2   | MEMORY\[R3] ← R2                                 | 4                        |
| INC R3         | R3 ← R3 + 1                                      | 2                        |
| DEC R1         | R1 ← R1 – 1                                      | 2                        |
| BNZ 1004       | Branch if not zero to the given absolute address | 2                        |
| HALT           | Stop                                             | 1                        |

Assume that the content of the memory location 5000 is 10, and the content of register R3 is 3000. The content of each of the memory locations from 3000 to 3010 is 50. The instruction sequence starts from memory location 1000. All the numbers are in decimal format, and memory is byte-addressable.
**Find the content of memory location 3010 after the execution of the program.**

d) Assume a cache miss penalty is 100 clock cycles, and all instructions take 1.0 clock cycle. Let the average miss rate be 2%, there is an average of 1.5 memory references per instruction, and the average number of cache misses per 1000 instructions is 30.
**What is the impact on performance, and calculate the impact using both misses per instruction and miss rate?**

---

**Part-III (Long Answer Type Questions) (Answer Any Two out of Four) (16 × 2)**

Q4. Describe cache memory and mapping policies with suitable examples. Consider a 16-way set-associative cache having 64 bits long Data words. The cache holds 2 Mbytes of data, and each block holds 16 data words. Physical addresses are 64 bits long.
**How many bits of tag, index, and offset are needed to support references to this cache?**

Q5. Briefly describe the VLIW processor architecture. What are the differences between a superscalar processor and V.L.I.W. processor? Suppose your program consists of 2500 instructions. The proportion of different kinds of instructions in the program is as follows: Data transfer instruction 50%, arithmetic instruction 30%, and branching related instructions 20%. The cycles consumed by these types of instructions are 2, 5, and 10 respectively.
**What will be the execution time for a 4 GHz processor to execute your program?**

---
