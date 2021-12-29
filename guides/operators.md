# Operators

### Python Operators

The operator can be defined as a symbol which is responsible for a particular operation between two operands. Operators are the pillars of a program on which the logic is built in a specific programming language. Python provides a variety of operators, which are described as follows.

* Arithmetic operators
* Comparison operators
* Assignment Operators
* Logical Operators
* Bitwise Operators
* Membership Operators
* Identity Operators

### Arithmetic Operators

Arithmetic operators are used to perform arithmetic operations between two operands. It includes + (addition), - (subtraction), \*(multiplication), /(divide), %(reminder), //(floor division), and exponent (\*\*) operators.



| **Operator**      | **Description**                                                                                                                     | **Example**                              |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------- |
| + Addition        | Adds values on either side of the operator.                                                                                         | a + b = 31                               |
| - Subtraction     | Subtracts right hand operand from left hand operand.                                                                                | a – b = -11                              |
| \* Multiplication | Multiplies values on either side of the operator                                                                                    | a \* b = 210                             |
| / Division        | Divides left hand operand by right hand operand                                                                                     | b / a = 2.1                              |
| % Modulus         | Divides left hand operand by right hand operand and returns remainder                                                               | b % a = 1                                |
| \*\* Exponent     | Performs exponential (power) calculation on operators                                                                               | a\*\*b =10 to the power 20               |
| //                | Floor Division - The division of operands where the result is the quotient in which the digits after the decimal point are removed. | <p>9//2 = 4 and</p><p>9.0//2.0 = 4.0</p> |

### Comparison Operators

These operators compare the values on either side of them and decide the relation among them. They are also called Relational operators.

Assume variable a holds the value 10 and variable b holds the value 20, then-

| **Operator** | **Description**                                                                                                   | **Example**           |
| ------------ | ----------------------------------------------------------------------------------------------------------------- | --------------------- |
| ==           | If the values of two operands are equal, then the condition becomes true.                                         | (a == b) is not true. |
| !=           | If values of two operands are not equal, then condition becomes true.                                             | (a!= b) is true.      |
| >            | If the value of left operand is greater than the value of right operand, then condition becomes true.             | (a > b) is not true.  |
| <            | If the value of left operand is less than the value of right operand, then condition becomes true.                | (a < b) is true.      |
| >=           | If the value of left operand is greater than or equal to the value of right operand, then condition becomes true. | (a >= b) is not true. |
| <=           | If the value of left operand is less than or equal to the value of right operand, then condition becomes true.    | (a <= b) is true.     |

### Assignment Operators



| **Operator**       | **Description**                                                                            | **Example**                                                        |
| ------------------ | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------ |
| =                  | Assigns values from right side operands to left side operand                               | c = a + b assigns value of a + b into c                            |
| += Add AND         | It adds right operand to the left operand and assign the result to left operand            | c += a is equivalent to c = c + a                                  |
| -= Subtract AND    | It subtracts right operand from the left operand and assign the result to left operand     | c -= a is equivalent to c = c - a                                  |
| \*= Multiply AND   | It multiplies right operand with the left operand and assign the result to left operand    | c \*= a is equivalent to c = c \* a                                |
| /= Divide AND      | It divides left operand with the right operand and assign the result to left operand       | c /= a is equivalent to c = c / ac /= a is equivalent to c = c / a |
| %= Modulus AND     | It takes modulus using two operands and assign the result to left operand                  | c %= a is equivalent to c = c % a                                  |
| \*\*= Exponent AND | Performs exponential (power) calculation on operators and assign value to the left operand | <p>c **= a is equivalent to c = c</p><p>** a</p>                   |
| //= Floor Division | It performs floor division on operators and assign value to the left operand               | c //= a is equivalent to c = c // a                                |

### Logical Operators

The following logical operators are supported by Python language. Assume variable a holds True and variable b holds False then-

| **Operator**    | **Description**                                                      | **Example**           |
| --------------- | -------------------------------------------------------------------- | --------------------- |
| and Logical AND | If both the operands are true then condition becomes true.           | (a and b) is False.   |
| or Logical OR   | If any of the two operands are non-zero then condition becomes true. | (a or b) is True.     |
| not Logical NOT | Used to reverse the logical state of its operand.                    | Not(a and b) is True. |

### Bitwise Operators

Bitwise operator works on bits and performs bit-by-bit operation. Assume if a = 60; and b = 13; Now in binary format they will be as follows- a = 0011 1100 b = 0000 1101

a\&b = 0000 1100

a|b = 0011 1101 a^b = 0011 0001

\~a  = 1100 0011

Pyhton's built-in function bin() can be used to obtain binary representation of an integer number.

&#x20;

The following Bitwise operators are supported by Python language-

| **Operator**                                   | **Description**                                                                               | **Example**                                                                         |
| ---------------------------------------------- | --------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------- |
| & Binary AND                                   | Operator copies a bit to the result, if it exists in both operands                            | <p>(a &#x26; b) (means 0000</p><p>1100)</p>                                         |
| \| Binary OR                                   | It copies a bit, if it exists in either operand.                                              | <p>(a | b) = 61 (means</p><p>0011 1101)</p>                                         |
| ^ Binary XOR                                   | It copies the bit, if it is set in one operand but not both.                                  | <p>(a ^ b) = 49 (means</p><p>0011 0001)</p>                                         |
| <p>~     Binary      Ones</p><p>Complement</p> | It is unary and has the effect of 'flipping' bits.                                            | (\~a ) = -61 (means 1100 0011 in 2's complement form due to a signed binary number. |
| << Binary Left Shift                           | The left operand’s value is moved left by the number of bits specified by the right operand.  | <p>a &#x3C;&#x3C; = 240 (means</p><p>1111 0000)</p>                                 |
| >> Binary Right Shift                          | The left operand’s value is moved right by the number of bits specified by the right operand. | <p>a >> = 15 (means</p><p>0000 1111)</p>                                            |

### Membership Operators

Python’s membership operators test for membership in a sequence, such as strings, lists, or tuples. There are two membership operators as explained below-

| **Operator** | **Description**                                                                                  | **Example**                                                                             |
| ------------ | ------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| in           | Evaluates to true, if it finds a variable in the specified sequence and false otherwise.         | x in y, here in results in a 1 if x is a member of sequence y.                          |
| not in       | Evaluates to true, if it does not find a variable in the specified sequence and false otherwise. | <p>x not in y, here not in results in a 1 if x is not a member of sequence</p><p>y.</p> |

### Identity Operators

Identity operators compare the memory locations of two objects. There are two Identity operators as explained below:

| **Operator** | **Description**                                                                                                 | **Example**                                                          |
| ------------ | --------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------- |
| is           | Evaluates to true if the variables on either side of the operator point to the same object and false otherwise. | x is y, here is results in 1 if id(x) equals id(y).                  |
| is not       | Evaluates to false if the variables on either side of the operator point to the same object and true otherwise. | x is not y, here is not results in 1 if id(x) is not equal to id(y). |

### Operator Precedence

The precedence of the operators is essential to find out since it enables us to know which operator should be evaluated first. The precedence table of the operators in Python is given below.

| Operator                           | Description                                                                                |
| ---------------------------------- | ------------------------------------------------------------------------------------------ |
| \*\*                               | The exponent operator is given priority over all the others used in the expression.        |
| \~ + -                             | The negation, unary plus, and minus.                                                       |
| \* / % //                          | The multiplication, divide, modules, reminder, and floor division.                         |
| + -                                | Binary plus, and minus                                                                     |
| >> <<                              | Left shift. and right shift                                                                |
| &                                  | Binary and.                                                                                |
| ^ \|                               | Binary xor, and or                                                                         |
| <= < > >=                          | Comparison operators (less than, less than equal to, greater than, greater then equal to). |
| <> == !=                           | Equality operators.                                                                        |
| <p>= %= /= //= -= +=<br>*= **=</p> | Assignment operators                                                                       |
| is is not                          | Identity operators                                                                         |
| in not in                          | Membership operators                                                                       |
| not or and                         | Logical operators                                                                          |
