
## Content:

1) **[[#-- How Computers Are Made --|How Computers Are Made]]**
2) **[[#-- Digital Computing -- |Digital Computing]]**
3) **[[#-- Truth Tables --|Truth Tables]]**
4) **[[#-- Logical Gates --|Logical Gates]]**
5) **[[#-- Boolean Axioms and Theorems --|Boolean Axioms and Theorems]]**
6) **[[#-- Half Adder (2-digit) --|Half Adder]]**


## -- How Computers Are Made --

1)  It all starts with commond sand, which consists mostly of silicon dioxide (*quarts*)

2)  Using chemical methods such as **Carbothermic Reduction** to achieve **metallurgical-grade silicon** (approximately 99% pure), to achieve **electronic-grade purity** (99.999999% or higher) it will undergo a chemical purification, typically via the **Siemens Process**

3)  Silicon is a semi-conductor
	- It can conduct or stop conducting electricity
	- We can switch electrical current in silicon on/off very fast (nano seconds)

4)  From silicon we can make very fast switches, a bunch of these together make a chip which is put inside a plastic cover 


- This is called *Switch Logic*, or *Boolean Logic*, after **George Boole** who was the first to think of it

- A switch has two values (on/off) using two possible voltage values known as *logic 0* and *logic 1* -- hence why True or False values are called Booleans

- For **CMOS** (Complementary Metal-Oxide Semiconductor) logic gates, *logic 1* is any voltage greater than 70% of the supply voltage whilst *logic 0* is less than 30% of supply voltage

- Switches are referred to as ***Transistors***



## -- Digital Computing --

Digital computers use **digital logic** by converting *binary signals* (0s and 1s) and processing them through *logic gates*

Digital logic can be split into two layers:

- **Physical:**  transistors wired together to form logic gates

- **Logical:** rules (Boolean algebra) that dictate how gates are combined to perform useful operations



## -- Truth Tables --

A truth table is a mathematical table that listed every combination of values for the component prepositions and shows the resulting truth value of the statement.

Truth tables use five standard connectives in statements:


#### **Boolean Algebra:**

|      Connective       | Symbol |       English        |  Alternatives  |
| :-------------------: | :----: | :------------------: | :------------: |
|       Negation        |   ¬p   |       *not* p        | ~p  p'  p̄  !p |
|      Conjuction       | p ∧ q  |      p *and* q       |   p&q   p.q    |
|      Disjunction      | p ∨ q  |       p *or* q       |   p+q  p\|q    |
| Exclusive Disjunction | p ⊕ q  |       p xor q        |      p⊻q       |
|      Implication      | p → q  |   *if* p *then* q    |    p⊃q  p⇒q    |
|     Biconditional     | p ↔ q  | p *if and only if* q |    p≡q  p⇔q    |



## -- Logical Gates --

### **NOT Gate:**

![[Not-Gate.webp|79]]

Whatever is input, the opposite state will output, the NOT function is denoted by a horizontal bar over the value or in some cases a single quote mark (')






*Truth table of NOT gate:*

| **A** | **¬A** |
| :---: | :----: |
|   0   |   1    |
|   1   |   0    |


### AND Gate:

![[And-Gate.webp|88]]

Both input values must be 1 in order for the output to be 1


*Truth table of AND gate:*

| **A** | **B** | Z=A ∧ B |
| :---: | :---: | :-----: |
|   0   |   0   |    0    |
|   0   |   1   |    0    |
|   1   |   0   |    0    |
|   1   |   1   |    1    |


### OR Gate:

![[Or-Gate.webp|87]]

Output will be True if one or more value is true

*Truth table of OR gate:*

| **A** | **B** | Z=A ∨ B |
| :---: | :---: | :-----: |
|   0   |   0   |    0    |
|   0   |   1   |    1    |
|   1   |   0   |    1    |
|   1   |   1   |    1    |


### XOR Gate:

![[Xor-Gate.webp|69]]

Outputs true if the values input are different

*Truth table of AND gate:*

| **A** | **B** | Z=A ⊕ B |
| :---: | :---: | :-----: |
|   0   |   0   |    0    |
|   0   |   1   |    1    |
|   1   |   0   |    1    |
|   1   |   1   |    0    |


### NAND Gate:

![[Nand-Gate.webp|80]]

Combines the use of AND gate and NOT gate. 

*Truth table of NAND gate:*

| **A** | **B** | A ∧ B | ¬(A ∧ B) |
| :---: | :---: | :---: | :------: |
|   0   |   0   |   0   |    1     |
|   0   |   1   |   0   |    1     |
|   1   |   0   |   0   |    1     |
|   1   |   1   |   1   |    0     |

The output is the opposite of the AND result



### NOR Gate:

![[Nor-Gate.webp|80]]

Combines the use of OR gate and NOT gate. 

*Truth table of NOR gate:*

| **A** | **B** | A ∨ B | ¬(A ∨ B) |
| :---: | :---: | :---: | :------: |
|   0   |   0   |   0   |    1     |
|   0   |   1   |   1   |    0     |
|   1   |   0   |   1   |    0     |
|   1   |   1   |   1   |    0     |

The output is the opposite of the OR result




## -- Boolean Axioms and Theorems --

Axioms or Postulates of Boolean Algebra are just definitions of three basic logic operations (AND, OR and NOT). Boolean Theorems are extra rules that are derived from the axioms.


## Boolean Axioms:


1)  **Identity Property**
2)  **Complement Property**
3)  **Involution Property**
4)  **Commutative Property**
5)  **Associative Property**


### 1. Identity Property

These four rules tell you what happens when you combine a variable with two constans 0 and 1. Combining 0 or 1 either leaves the variable unchanged or forces the result to 0 or 1.

- x + 0 = x    
	`ORing anything with 0 leaves it unchanged`

- x . 1 = x
	`ANDing anything with 1 leaves it unchanged`

- x + 1 = 1
	`ORing anything with 1 always produces 1`

- x . 0 = 0
	`ANDing anything with 0 always produces 0`


### 2. Complement Property

These two rules define what the NOT operation does in relation to AND or OR operations.

- x + x' = 1
	`A signal ORed with its own inverse is always 1`

- x . x' = 0
	`A signal ANDed with its own inverse is always 0`


### 3. Involution Property

Applying NOT twice brings back the original value, allowing for the simplification of the logic circuit

- (x')' = x


### 4. Commutative Property

The order of inputs does not matter. The OR and AND are symmetric meaning swapping the inputs never change the output.

- x + y = y + x
- x . y = y . x


### 5. Associative Property

The way you group (multiple OR operations) or (multiple AND operations) does not matter. 

- x + (y + z) = (x + y) + z
- x . (y . z) = (x . y) . z




## Boolean Theorems:

1) **Indempotent Laws**
2) **Absorption Laws**
3) **Distributive Laws**
4) **De Morgan's Law**



### 1. Indempotent Law

Doing the same operation twice with the same variable does nothing, it will just output the original signal

- x + x = x
- x . x = x


### 2. Absorption Law

A smaller term can "absorb" a larger term that already contains it. This means that the extra part becomes redundant. The signal that appears in both logic operations is the remaining output

- x + x.y = x
- x . x+y = x



### 3. Distributive Law

AND distributes over OR and vice versa, OR distributes over AND (just like multiplication `3 x (4+5) = (3x4) + (3x5)` )

- x . (y + z) = (x . y) + (x . z)
- x + (y . z) = (x + y) . (x + z)


### 4. De Morgan's Law

When you invert an OR operation it will become AND with inverted signals, this will apply vice versa with an invert AND operation becoming OR with inverted signals.

- (x . y)' = x' + y'
- (x + y)' = x' . y'




## -- Half Adder (2-digit) --

A ***Half Adder*** is a logical circuit that carries addition of binary signals. It is the simplest adder using two logic gates (XOR, AND). The half adder can only handle two 1-bit numbers allowing a total value of 2 -- a full adder would allow a maximum value of 3.


*Circuit Diagram:                                       Logic Diagram:*

![[Half-Adder-Circuit.png|147]]                               ![[Half-Adder-Logic.png|250]]


*Truth Table:*


| *INPUT* | *INPUT* | *OUTPUT* | *OUTPUT* |
| :-----: | :-----: | :------: | :------: |
|  **A**  |  **B**  |  **S**   |  **C**   |
|    0    |    0    |    0     |    0     |
|    0    |    1    |    1     |    0     |
|    1    |    0    |    1     |    0     |
|    1    |    1    |    0     |    1     |

Carry represents the value for the next digit placeholder whilst sum is the actual result, just like in binary addition, for example:

![[Binary-Addition-Example.png|269]]  

Here we have the small (1's) that represent the carry for the next digit placeholder and the sum would be 0, and if it was three (1's) the sum would be 1 with a carry of 1.



## -- Full Adder (2-digit) --

A ***Full Adder*** can be thought of as two ***Half Adders*** connected together, with the first half adder passing it's carry to the second half adder. This means the full adder can take 3 inputs, this allows it to be chained to make ***Ripple Carry Adders***.

