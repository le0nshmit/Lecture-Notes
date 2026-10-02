

## -- Program Functionality   (Input, Process, Output) --

**1- Input:** Accepts data user or source
**2-Process:** Performs operations on the data
**3-Output**: Produces results based on operations


## -- Variables --

Variables stores a value of various types (int, float, char, etc)

A constant is a variable that has a fixed value using the kword `const`

### **DataTypes:**

**Int:** an integer value (25) - 2 or 4-byte
**Float:** a decimal value (3.5f) - 4-byte | 7 decimals
**Double:** a more precise decimal value (3.5f)  - 8-byte | 15 decimals
**Char:** a character value ('A') - 1-byte
**String:** a sequence of characters ('POO') 
**Bool:** an 'on'/'off' value (True, False) - 1-byte

### Variable Scope:

- **Local:** declared inside function or block, removed from stack when not used
- **Global:** declared outside functions and accessible across program
- **Static:** persisted value throughout program but with local scope

### Variable Naming:

**1**- Use meaningful names 
**2**- Follow naming conventions (camelCase)
**3**- Avoid reserved keywords (e.g  break)
**4**- Keep names concise

You can assign multiple variables to the same starting value:

	int a = b = c = 5;


### Type Casting:

**Implicit Casting:** compiler automatically converts data types

	int x = 10
	float y = x;

**Explicit Casting:** manually  converting data type

	float result = static_cast<float>(x) / 3;




## -- Input & Output --

Input and Output requires the iostream library `#include <iostream>`

**Output:** cout (character output)

**Input:** cin (character input)



## -- Operators --

**Bitwise Operators:** binary value operations

`&`: bitwise AND
`|`: bitwise OR
`^`: bitwise XOR
`<< >>`: shift operators

- AND (&)
- OR (|)
- XOR (^)
- Shift Operators (<<, >>)

**Mathmatic Operators:**

`%`  : modulus operator returns remainder





## -- Stack vs Heap --

**Stack:**

- Static 
- Automatically handled
- Faster but limited

**Heap**:

- Dynamic
- Manually handled
- Slower but more flexible

