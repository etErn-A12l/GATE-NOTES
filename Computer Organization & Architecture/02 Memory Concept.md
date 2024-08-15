
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




