## Content:

1) Basics
2) Positional Numbering Systems
	- Decimal System
	- Binary System
	- Octal System
	- Hexadecimal System
3) General Case
4) Binary Addition 
5) Binary Multiplication


## -- Positional Numbering Systems --

 Positional numbering systems are systems in which the placement of a digit in connection to its value determines the actual meaning in a numeral string 

There are several numbering systems:

- **Decimal**
- **Binary**
- **Octal**
- **Hexadecimal**

Each numbering system can be provided as a subscript, for example (10<sub>2</sub>  10<sub>8</sub>     10<sub>10</sub>  10<sub>16</sub> )



## -- Decimal System --

The ***Binary System*** is base-10 which means it has digits 0-9, this is the common numbering system as we have ten fingers, allowing us to easily work with this system. 

Decimal values are represented by a subscript of 10.

177<sub>10</sub>      


### **To Another Base**:

To convert decimal to another numbering base, you can follow the same procedure (binary is a little different compared to others). The steps are simple, first divide your decimal value by the base subscript. The remainder of the dibvision is your result and the whole number is then divided again until you reach 0. If you are converting to binary, the remainder is always 1, but if you are converting to another base like hex, you would multiply the remainder by its subscript, so for hex it would be 16. The result will be all the remainders in reverse order. 


### To Binary:

524 / 2 = 262  *remainder*  **0**
262 / 2 = 131  *remainder*  **0**
131 / 2 = 65    *remainder*  **1**
65  /  2 = 32    *remainder*  **1**
32  /  2 = 16    *remainder*  **0**
16  /  2 = 8      *remainder*  **0**
8    /  2 = 4      *remainder*  **0**
4   /   2 = 2      *remainder*  **0**
2   /   2 = 1      *remainder*  **0**
1   /   2 = 0      *remainder*  **1**

**1000001100**<sub>2</sub>


### To Octal:

524 / 8 = 65     *remainder*  0.5x8     = **4**
65   / 8 = 8       *remainder*  0.125x8 = **1**
8     / 8 = 1       *remainder*                    **0**
1     / 8 = 0       *remainder*  0.125x8 = **1**

**1014**<sub>8</sub>


### To Hexadecimal:

524 / 16 = 32  *remainder* 0.75x16   = **12** = **C**
32   / 16 = 2    *remainder*                       **0**
2     / 16 = 0    *remainder*  0.125x16 =  **2**
 
**20C**<sub>16</sub>




## -- Binary System --

The ***Binary System*** is base-2 which means it can have only two possible values (1, 0).

Binary values are represented by a subscript of 2.

256 | 128 | 64 | 32 | 16 | 8 | 4 | 2 | 1 
	
  0         1       0       1      1     0    0    0    1      =      177<sub>10</sub>      


### **To Decimal**:

To convert binary values to decimal, you would start from the far left digit and multiply each digit by 2 shifting to the right. For each multiplication 2 is exponent by its index and each shift decreases the exponent. This same concept applies to any base value, being divised by its subscript constantly and shifting.


5   4   3   2   1   0    -1  -2  -3  -4
1 0 1 1 0 1 . 0 1 0 1
= 

1x2<sup>5</sup> + 0x2<sup>4</sup> +  1x2<sup>3</sup> +  1x2<sup>2</sup> +  0x2<sup>1</sup> +  1x2<sup>0</sup> +  0x2<sup>-1</sup> +  1x2<sup>-2</sup> +  0x2<sup>-3</sup> +  1x2<sup>-4</sup>

 32    +   0     +     8    +    4     +     0    +     1    +    0      +    .25   +   .0  +  .0625 

**45.3125**<sub>10</sub>



### **To Hexadecimal:**

To convert binary to hexadecimal, you group the binary signals into groups of four (4-bits) starting from the right -- this is because 4-bits can represent 0-15 digits. Then you convert one group at a time to its hex value, to do this you can represent the binary value in decimal first and then represent it in the hex value. 

Hexadecimal is easily mapped to binary allowing a human-readable format, whilst still being easy to translate with the least amount of mathematics.

**10011011001** 
=

0100 1101 1001

   4       13      9

As we know 13 in hex is represented as 'D'.

**4D9**<sub>16</sub>



### **To Octal:**

To convert binary to octal, you group the binary signals into groups of 3 (3-bits) starting from the far right (just like for hexadecimal) -- this is because 3-bits can represent 0-7 digits.  
**10011011001** 
=

010 011 011 001

  2      3     3     1 

**2331**<sub>8</sub>

As we know 13 in hex is represented as 'D'.

**4D9**<sub>16</sub>





## -- Octal System --

The ***Octal System*** is represented using base-8, this means its possible digits are 0-7.

### **To Decimal:**

450.72<sub>8</sub>  
=

4x8<sup>2</sub> + 5x8<sup>1</sub> + 0x8<sup>0</sub> + 7x8<sup>-1</sub> + 2x8<sup>-2</sub>

256   +  40    +   0     + .875  + .03125

**296.90625**<sub>10</sub>



### **To Binary:**


This is just the opposite process from octal to binary. Seperate each digit and represent as a 3-bit binary value.

450.72<sub>8</sub>  
=

4x8<sup>2</sub> + 5x8<sup>1</sub> + 0x8<sup>0</sub> + 7x8<sup>-1</sub> + 2x8<sup>-2</sub>

256   +  40    +   0     + .875  + .03125

**296.90625**<sub>10</sub>






## -- Hexadecimal System --

The ***Hexadecimal System*** is a base-16, this means it has 16 possible digits 0-F. Instead of using 10-15, they are represented by letters A-F. This is more efficient to read allowing it to be compact with one digit instead of multiple like '25'.

**A :** 10 
**B :** 11
**C :** 12
**D :** 13
**E :** 14
**F :** 15

### **To Decimal:**

A2C.F2<sub>16</sub>  
=

10x16<sup>2</sub> + 2x16<sup>1</sub> + 12x16<sup>0</sub> + 15x16<sup>-1</sub> + 2x16<sup>-2</sub>

2560     +    32    +     12     +   .9375   + .0078125

**2604.9453125**<sub>10</sub>


