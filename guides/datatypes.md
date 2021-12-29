# Datatypes

## Python Data Types

Variables can hold values, and every value has a data-type. Python is a dynamically typed language; hence we do not need to define the type of the variable while declaring it. The interpreter implicitly binds the value with its type.

`a = 5`&#x20;

The variable **a** holds integer value five and we did not define its type. Python interpreter will automatically interpret variables **a** as an integer type.

Python enables us to check the type of the variable used in the program. Python provides us the **type()** function, which returns the type of the variable passed.

Consider the following example to define the values of different data types and checking its type.

```
// Some code
a=10  
b="Hi Python"  
c = 10.5  
print(type(a))  
print(type(b))  
print(type(c))  
```

Python has the following data types built-in by default, in these categories:

| Text Type:      | `str`                              |
| --------------- | ---------------------------------- |
| Numeric Types:  | `int`, `float`, `complex`          |
| Sequence Types: | `list`, `tuple`, `range`           |
| Mapping Type:   | `dict`                             |
| Set Types:      | `set`, `frozenset`                 |
| Boolean Type:   | `bool`                             |
| Binary Types:   | `bytes`, `bytearray`, `memoryview` |

### Getting the Data Type

You can get the data type of any object by using the `type()` function:

#### Example

Print the data type of the variable x:

`x = 5`\
`print(type(x))`

### Setting the Specific Data Type

If you want to specify the data type, you can use the following constructor functions:

### Setting the Specific Data Type

If you want to specify the data type, you can use the following constructor functions:

| Example                                      | Data Type  |   | Try it |
| -------------------------------------------- | ---------- | - | ------ |
| x = str("Hello World")                       | str        |   |        |
| x = int(20)                                  | int        |   |        |
| x = float(20.5)                              | float      |   |        |
| x = complex(1j)                              | complex    |   |        |
| x = list(("apple", "banana", "cherry"))      | list       |   |        |
| x = tuple(("apple", "banana", "cherry"))     | tuple      |   |        |
| x = range(6)                                 | range      |   |        |
| x = dict(name="John", age=36)                | dict       |   |        |
| x = set(("apple", "banana", "cherry"))       | set        |   |        |
| x = frozenset(("apple", "banana", "cherry")) | frozense   |   |        |
| x = bool(5)                                  | bool       |   |        |
| x = bytes(5)                                 | bytes      |   |        |
| x = bytearray(5)                             | bytearray  |   |        |
| x = memoryview(bytes(5))                     | memoryview |   |        |
