# CPU scratch pad instruction codes:

# Bus_Read_Write:
*Used to read from or write to the CPU bus* | **INPUT IS INVERTED (active while low)**
## Bus in/out:

### High Order bit:
	0. out
	1. in
## Register numbers:
0. B
1. C
2. D
3. E
4. H
5. L
6. W (TMP)
7. Z (TMP)

# register ops:

## Increment/Decrement (8 or 16 bit)

### I_D (Increment/Decrement):
*Specifies whether to increment or decrement |*
*Tri-state input (Z for disable)*

0. Decrement
1. Increment

## Transfers
**INPUT IS INVERTED (active while low)**

### Read_Select & Write_Select:
*Used to select which input/output register should be used*

#### High Order bit:
0. select 16 bit
1. select 8 bit

| Input 	| 8-bit 	| 16-bit 		|
|-----------|-----------|-----------	|
| 		0  	|Register B	|BC Pair		|
| 		1  	|Register C	|Program Coutner|
|		2	|Register D	|DE Pair		|
| 		3  	|Register E	|Stack Pointer	|
| 		4  	|Register H	|HL Pair		|
| 		5  	|Register L	|Address read/load|
| 		6  	|Register W	|WZ Pair		|
| 		7  	|Register Z	|N/A			|
