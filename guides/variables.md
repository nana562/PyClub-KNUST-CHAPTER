# Variables

Variable is a name that is used to refer to memory location. Python variable is also known as an identifier and used to hold value.

In Python, we don't need to specify the type of variable because Python is a infer language and smart enough to get variable type.

```
// Example code
number = 5
name = "John"
print(number)
print(name)
```

### Identifier Naming

Variables are the example of identifiers. An Identifier is used to identify the literals used in the program. The rules to name an identifier are given below.

Declaring Variable and Assigning Values

Python does not bind us to declare a variable before using it in the application. It allows us to create a variable at the required time.

We don't need to declare explicitly variable in Python. When we assign any value to the variable, that variable is declared automatically.

The equal (=) operator is used to assign a value to a variable.

### Variable Names

We have already discussed how to declare the valid variable. Variable names can be any length can have uppercase, lowercase (A to Z, a to z), the digit (0-9), and underscore character(\_). Consider the following example of valid variables names.

The variable name should be descriptive to make code more readable.

The multi-word keywords can be created by the following method.

* **Camel Case -** In the camel case, each word or abbreviation in the middle of begins with a capital letter. There is no intervention of whitespace. For example - nameOfStudent, valueOfVaraible, etc.
* **Pascal Case -** It is the same as the Camel Case, but here the first word is also capital. For example - NameOfStudent, etc.
* **Snake Case -** In the snake case, Words are separated by the underscore. For example - name\_of\_student, etc.

### Multiple Assignment

Python allows us to assign a value to multiple variables in a single statement, which is also known as multiple assignments.

We can apply multiple assignments in two ways, either by assigning a single value to multiple variables or assigning multiple values to multiple variables. Consider the following example.

**1. Assigning single value to multiple variables**

```
// Example code
x=y=z=50    
print(x)    
print(y)    
print(z)    
```

**2. Assigning multiple values to multiple variables:**

```
// Some code
a,b,c=5,10,15    
print a    
print b    
print c    
```

### Python Variable Types

There are two types of variables in Python - Local variable and Global variable. Let's understand the following variables.

#### Local Variable

Local variables are the variables that declared inside the function and have scope within the function. Let's understand the following example.\


```
// Example code
# Declaring a function  
def add():  
    # Defining local variables. They has scope only within a function  
    a = 20  
    b = 30  
    c = a + b  
    print("The sum is:", c)  
  
# Calling a function  
add()  
```

**Explanation:**

In the above code, we declared a function named **add()** and assigned a few variables within the function. These variables will be referred to as the **local variables** which have scope only inside the function. If we try to use them outside the function, we get a following error.

```
// Example code
add()  
# Accessing local variable outside the function   
print(a)  
```

We tried to use local variable outside their scope; it threw the **NameError.**

#### Global Variables

Global variables can be used throughout the program, and its scope is in the entire program. We can use global variables inside or outside the function.

A variable declared outside the function is the global variable by default. Python provides the **global** keyword to use global variable inside the function. If we don't use the **global** keyword, the function treats it as a local variable. Let's understand the following example.

```
// Example code
# Declare a variable and initialize it  
x = 101  
  
# Global variable in function  
def mainFunction():  
    # printing a global variable  
    global x  
    print(x)  
    # modifying a global variable  
    x = 'Welcome To Javatpoint'  
    print(x)  
  
mainFunction()  
print(x)  
```

**Explanation:**

In the above code, we declare a global variable **x** and assign a value to it. Next, we defined a function and accessed the declared variable using the **global** keyword inside the function. Now we can modify its value. Then, we assigned a new string value to the variable x.

Now, we called the function and proceeded to print **x**. It printed the as newly assigned value of x.

### Delete a variable

We can delete the variable using the **del** keyword. The syntax is given below.

**Syntax -**

`del <variable_name`>

In the following example, we create a variable x and assign value to it. We deleted variable x, and print it, we get the error **"variable x is not defined"**. The variable x will no longer use in future.

**Example -**

```
// Example code
# Assigning a value to x  
x = 6  
print(x)  
# deleting a variable.   
del x  
print(x)  
```

### Maximum Possible Value of an Integer in Python

Unlike the other programming languages, Python doesn't have long int or float data types. It treats all integer values as an **int** data type. Here, the question arises. What is the maximum possible value can hold by the variable in Python? Consider the following example.

**Example -**

```
// Some code
# A Python program to display that we can store  
# large numbers in Python  
  
a = 10000000000000000000000000000000000000000000  
a = a + 1  
print(type(a))  
print (a)  
```

As we can see in the above example, we assigned a large integer value to variable **x** and checked its type. It printed **class \<int>** not long int. Hence, there is no limitation number by bits and we can expand to the limit of our memory.

Python doesn't have any special data type to store larger numbers.

#### Print Single and Multiple Variables in Python

We can print multiple variables within the single print statement. Below are the example of single and multiple printing values.

**Example - 1 (Printing Single Variable)**

```
// Some code
# printing single value   
a = 5  
print(a)  
print((a))  
```



**Example - 2 (Printing Multiple Variables)**

```
// Some code
a = 5
b -t
# printing multiple variables  
print(a,b)  
# separate the variables by the comma  
Print(1, 2, 3, 4, 5, 6, 7, 8)   
```

