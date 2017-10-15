## bit.dc, v1.1
### Bitwise operations for `dc`

#### Operators
This section lists the operators. These are persistent macros intended to be called by the user.

| Register | Function       |    I    |    O    | Comment
|:--------:|:---------------|:-------:|:-------:|:--------
| &        | Bitwise AND    |    2    |    1    |
|\|        | Bitwise OR     |    2    |    1    |
| ^        | Bitwise XOR    |    2    |    1    |
| \        | Bitwise NOT    |    1    |    1    | This function flips the bits of the top number
| ~        | Bitwise NOT    |    2    |    1    | This function flips the bits of the top two numbers, using the longer number's length in bits

#### Helper Functions
This section lists the helper functions. These are persistent macros intended to be called by the operators and each other.

| Register | Function       |    I    |    O    | Comment
|:--------:|:---------------|:-------:|:-------:|:--------
| ?        | Error message  |    0    |    0    | This function displays a message indicating that there are not enough values on the stack
| #        | Array to int   |   A[]   |    1    | This function converts the boolean array A[] to a number and pushes that number on the stack
| B        | Run-once code  |    2    |    1    | This function contains code that is used once by multiple functions

#### Temporary Registers
This section lists the temporary registers. These registers hold transient values or code and are left unchanged at the end of an operation.

| Register | Function       |    I    |    O    | Comment
|:--------:|:---------------|:-------:|:-------:|:--------
| $        | Int to array   |    1    | a[],b[] | This function splits the top of stack to either a[] or b[]
| a,b      | Input parsing  |    -    |    -    | These registers and their arrays hold input while an operation is taking place
| A        | Output storage |    -    |    -    | This register and its array hold output while an operation is taking place
| I        | Conditional    |    -    |    -    | This register contains code that is to be executed in an if-then-else structure
| L        | Loop code      | a[],b[] |   A[]   | This function contains code that is used in a do-while manner
| O        | Operator code  |    2    |    1    | This register contains code that is different for each operator
| Z        | max(a,b)       |   a,b   |    Z    | This register contains the maximum of a and b, which represent the lengths of the input




<hr />
<br>Author:     Joseph Reed
