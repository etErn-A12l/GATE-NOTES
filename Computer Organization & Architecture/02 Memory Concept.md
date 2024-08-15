
##### Main Memory is represented in the form of $2^{n}$ x m

Where, 
n = Number of Address line ( A.L )
m = Number of Address line ( D.L )

- A.L => Address Line denotes the capacity of Memory
- D.L => Data Lines denotes the capacity of Data ( cell size )

**NOTE**: *n bit address line can represent $2^{n}$ memory cells* ( 0 to $2^{n}$ -1) .

Refer to [[General]]

![[co-13.png]]

So, for **1K Byte** Memory : 
	$2^{10}$ x 8 bit => 10 address lines, 8 data lines
Similarly, for **16 Byte** Memory :
	$2^{4}$ x 8 bit => 4 address lines, 8 data lines
	=> A.L is 0000 to 1111 in binary

**64 K Byte** Memory ( **64 KB** ) :
	$2^{16}$ x 8 bit
	=> 16 bit A.L ( $0000$ to $FFFF$ in hex )
	=> 8 bit D.L
	=> $2^{16}$ memory cells
	=> each cell is 8 bits

**1 M Byte** Memory ( **1 MB** ) :
	$2^{20}$ x 8 bit
	=> 20 bit A.L ( $00000$ to $FFFFF$ in hex )
	=> 8 bit D.L
	=> $2^{20}$ memory cells
	=> each cell is 8 bits



**NOTE**: *When memory is byte addressable, then the data line will always be $8$ $bit$. But if it is word addressable, then the data line depends on the word length of a processor. Example: a $64$ $bit$ processor has a data line of $64$ $bit$. Default Memory configuration is byte addressable.*

---


### Numericals

1. The capacity of a memory unit is defined by the number of word multiplied by the number of bits/word. How many separate address and data lines are needed for a memory of $64K$ $*$ $16$ ?

#Solution:

$64K$= $2^{6}$ * $1K$ = $2^{6}$ * $2^{10}$ = $2^{16}$

So, address line = $16 bit$ and also, data line = $16 bit$

2. Consider a system which has 1024 k words. Each word has the size of 32 bits then what is the capacity of memory in MB (MegaByte) ?

#Solution:

32 bits = 4 bytes. 
1024 K words = 1024 * 4 K bytes = 4096 KB = 4 MB. 


3. A processor can support a maximum memory of 4GB, where the memory is word-addressable ( a word consists of two bytes ). The size of the address bus of the processor is at least how many bits ?

#Solution:

one word = 2 bytes

4 GB = 2 Bytes * 2 GB = 2 * 2 * $2^{30}$ Bytes = $2^{31}$ $*$ 2 bytes. = $2^{31}$ words ( 1 word = 2 Bytes )

Ans = 31 address lines, minimum 31 bits.


4. The capacity of a memory unit is defined by the number of word multiplied by the number of bits/word. How many separate address and data lines are needed for a memory of 4K x 16 ?

#Solution: 

4 K = $2^{2}$ * $2^{10}$ = $2^{12}$

So, 12 Address , 16 Data line

5. Consider a 32 bit Hypothetical processor which support 128 MByte memory. System is enhanced with a new word addressable memory. Now how many address lines are required in the new system ?


#Solution 

1 word = 32 bits = 4 bytes.
128 MB = ( 128 MB / 4 B ) M words = 32 M Words = $2^{5}$ * $2^{20}$ words = $2^{25}$ words

Address = 25 bit