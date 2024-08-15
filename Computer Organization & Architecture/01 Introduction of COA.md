
There are 3 main parts of a computer

1. CPU
	1. ALU
	2. CU
	3. Registers
		1. Special Purpose Registers
		2. General Purpose Registers
2. Memory
	1. Main / Primary Memory
	2. Secondary / Auxilliary Memory
3. I/O
	1. Input Devices
	2. Output Devices


![[co-01.png]]

### Registers

1. PC
	Stands for program counter. it holds the ==starting address== of the ==next instruction== to be fetch (Execute).
2. MAR / AR
	Memory Address register / Address register. Contains the address or memory locations used for either read or write operation. It's connected to address system bus.
3. MBR / DR
	Memory Buffer Register / Data register. Contains Instruction or Data. It's connected to data system bus.
4. IR
	Instruction register, that contains the instruction which is currently being executed by CPU
5. AC
	Accumulator, It holds temporary result or the first operand of ALU operation


![[co-02.png]]

6. SP
	Stack pointer, points to the address in top of stack
7. PSW
	Program Status Register / Flag Register. Contains Status of ALU result
	1. carry
	2. parity
	3. sign
	4. zero flag
	5. auxilliary flag
	6. overflow flag
8. GPR
	General Purpose Registers. Used for data process.

![[co-03.png]]

### Instruction Cycle

1. Fetch Cycle
	To fetch the instruction from memory to CPU (IR). ==At the end of fetch cycle, PC is incremented and it point to the starting address of next instruction==. 
	Process: $PC -> MAR -> Memory -> MBR -> IR; PC++;$
2. Execute Cycle
	1. Decode
	2. Execute
3. Interrupt Cycle


![[co-04.png]]

![[co-05.png]]

![[co-06.png]]

![[co-07.png]]

If an interrupt occurs when Instruction "A" was being executed / about to execute, then Fetch cycle for "A" will be completed, then the starting address of next instruction, Let's assume "B" will be pointed by PC and will be pushed to the stack as return address, so that after interrupt completion, CPU can again start from "B".


### Memory

Memory can be classified into two types

1. ==Word Addressable==
	Each cell size is one word. 
1. ==Byte Addressable==
	Each cell size is one byte. Cell size of this memory is $8$ $bits$

$1  Word = 32  bits = 4  bytes$ (Generally assumed)

---

## Numericals


1. ![[co-08.png]]


#### Solution:

I1 : 1000 - 1007
I2 : 1008 - 1011
....
I7 : ==1040== - 1043 ||  **NOTE:**  *Program Counter always holds starting address of next instruction* 

So, $Ans = 1040$.

2. ![[co-09.png]]

#### Solution:

I1 : 1000 - 1001
I2 : 1002
....
I6 : ==1008== - 1009 ||  **NOTE:**  *Program Counter always holds starting address of next instruction* 

So, $Ans = 1008$.


3. ![[co-11.png]]

#### Solution:

I1 : 1000 - 1001
I2 : 1002
....
I4 : ==1004== - 1005 ||  **NOTE:**  *Program Counter always holds starting address of next instruction* 

So, $Ans = 1004$.


4. ![[co-10.png]]


#### Solution:

- Each and every instruction needs to be fetched and decoded, so all Instruction size $*$ 3
- Multiplication will need additional 6 cycles
- Register to/from memory will need extra 4 cycles

So, 

$(3*3+4) + (3*3+4) + (1*3+6) + (3*3+4) + (1*3) = 51$ Cycles


5. ![[co-12.png]]

#### Solution:

- Each and every instruction needs to be fetched and decoded, so all Instruction size $*$ 2
- Addition will need additional 1 cycles
- Register to/from memory will need extra 3 cycles

So, 

$(2*2+3) + (1*2+3) + (1*2+1) + (2*2+3) + (1*2) = 24$ Cycles