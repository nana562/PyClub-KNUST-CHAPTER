# Strings

### Python Strings

Strings in Python are identified as a contiguous set of characters represented in the quotation marks. Python allows either pair of single or double quotes. Subsets of strings can be taken using the slice operator (\[ ] and \[:] ) with indexes starting at 0 in the beginning of the string and working their way from -1 to the end.

The plus (+) sign is the string concatenation operator and the asterisk (\*) is the repetition operator. For example-

```
// Example code
 str = 'Hello World!'
print (str)          # Prints complete string
print (str[0])       # Prints first character of the string
print (str[2:5])     # Prints characters starting from 3rd to 5th
print (str[2:])      # Prints string starting from 3rd character
print (str * 2)      # Prints string two times
print (str + "TEST") # Prints concatenated string
```



### Creating String in Python

We can create a string by enclosing the characters in single-quotes or double- quotes. Python also provides triple-quotes to represent the string, but it is generally used for multiline string or **docstrings**.

```
// Example code
#Using single quotes  
str1 = 'Hello Python'  
print(str1)  
#Using double quotes  
str2 = "Hello Python"  
print(str2)  
  
#Using triple quotes  
str3 = '''''Triple quotes are generally used for  
    represent the multiline or 
    docstring'''   
print(str3)  
```

### Strings indexing and splitting

Like other languages, the indexing of the Python strings starts from 0. For example, The string "HELLO" is indexed as given in the below figure.

Consider the following example:

```
str = "HELLO"  
print(str[0])  
print(str[1])  
print(str[2])  
print(str[3])  
print(str[4])  
# It returns the IndexError because 6th index doesn't exist  
print(str[6])  
```

Here, we must notice that the upper range given in the slice operator is always exclusive i.e., if str = 'HELLO' is given, then str\[1:3] will always include str\[1] = 'E', str\[2] = 'L' and nothing else.

Consider the following example:

```
// Example code
# Given String  
str = "JAVATPOINT"  
# Start Oth index to end  
print(str[0:])  
# Starts 1th index to 4th index  
print(str[1:5])  
# Starts 2nd index to 3rd index  
print(str[2:4])  
# Starts 0th to 2nd index  
print(str[:3])  
#Starts 4th to 6th index  
print(str[4:7])  
```

### Deleting the String

As we know that strings are immutable. We cannot delete or remove the characters from the string.  But we can delete the entire string using the **del** keyword.

`str = "JAVATPOINT"` &#x20;

`del str[1]` &#x20;

Now we are deleting entire string.

```
// Some code
str1 = "JAVATPOINT"  
del str1  
print(str1)  
```

### String Operators

| Operator | Description                                                                                                                                                                                                                                        |
| -------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| +        | It is known as concatenation operator used to join the strings given either side of the operator.                                                                                                                                                  |
| \*       | It is known as repetition operator. It concatenates the multiple copies of the same string.                                                                                                                                                        |
| \[]      | It is known as slice operator. It is used to access the sub-strings of a particular string.                                                                                                                                                        |
| \[:]     | It is known as range slice operator. It is used to access the characters from the specified range.                                                                                                                                                 |
| in       | It is known as membership operator. It returns if a particular sub-string is present in the specified string.                                                                                                                                      |
| not in   | It is also a membership operator and does the exact reverse of in. It returns true if a particular substring is not present in the specified string.                                                                                               |
| r/R      | It is used to specify the raw string. Raw strings are used in the cases where we need to print the actual meaning of escape characters such as "C://python". To define any string as a raw string, the character r or R is followed by the string. |
| %        | It is used to perform string formatting. It makes use of the format specifiers used in C programming like %d or %f to map their values in python. We will discuss how formatting is done in python.                                                |

#### Example

Consider the following example to understand the real use of Python operators.

```
// Some code
str = "Hello"     
str1 = " world"    
print(str*3) # prints HelloHelloHello    
print(str+str1)# prints Hello world     
print(str[4]) # prints o                
print(str[2:4]); # prints ll                    
print('w' in str) # prints false as w is not present in str    
print('wo' not in str1) # prints false as wo is present in str1.     
print(r'C://python37') # prints C://python37 as it is written    
print("The string str : %s"%(str)) # prints The string str : Hello    
```

### Python String Formatting

#### Escape Sequence

Let's suppose we need to write the text as - They said, "Hello what's going on?"- the given statement can be written in single quotes or double quotes but it will raise the **SyntaxError** as it contains both single and double-quotes.

### Example

Consider the following example to understand the real use of Python operators.

```
// Example code
str = "They said, "Hello what's going on?""  
print(str)  
```

We can use the triple quotes to accomplish this problem but Python provides the escape sequence.

The backslash(/) symbol denotes the escape sequence. The backslash can be followed by a special character and it interpreted differently. The single quotes inside the string must be escaped. We can apply the same as in the double quotes.

#### Example -

```
// Example code
# using triple quotes  
print('''''They said, "What's there?"''')  
  
# escaping single quotes  
print('They said, "What\'s going on?"')  
  
# escaping double quotes  
print("They said, \"What's going on?\"")  
```



| Escape Sequence | Description                | Example                                                                                                                                    |
| --------------- | -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| \newline        | It ignores the new line.   | <pre><code>print("Python1 \
Python2 \
Python3")</code></pre><p><strong>Output:</strong></p><pre><code>Python1 Python2 Python3</code></pre> |
| \\\\            | Backslash                  | <pre><code>print("\\")</code></pre><p><strong>Output:</strong></p><pre><code>\</code></pre>                                                |
| \\'             | Single Quotes              | <pre><code>print('\'')</code></pre><p><strong>Output:</strong></p><pre><code>'</code></pre>                                                |
| \\\\''          | Double Quotes              | <pre><code>print("\"")</code></pre><p><strong>Output:</strong></p><pre><code>"</code></pre>                                                |
| \a              | ASCII Bell                 | <pre><code>print("\a")</code></pre>                                                                                                        |
| \b              | ASCII Backspace(BS)        | <pre><code>print("Hello \b World")</code></pre><p><strong>Output:</strong></p><pre><code>Hello World</code></pre>                          |
| \f              | ASCII Formfeed             | <pre><code>print("Hello \f World!")
Hello  World!</code></pre>                                                                             |
|                 | ASCII Linefeed             | <pre><code>print("Hello \n World!")</code></pre><p><strong>Output:</strong></p><pre><code>Hello
 World!</code></pre>                       |
|                 | ASCII Carriege Return(CR)  | <pre><code>print("Hello \r World!")</code></pre><p><strong>Output:</strong></p><pre><code>World!</code></pre>                              |
|                 | ASCII Horizontal Tab       | <pre><code>print("Hello \t World!")</code></pre><p><strong>Output:</strong></p><pre><code>Hello 	 World!</code></pre>                      |
| \v              | ASCII Vertical Tab         | <pre><code>print("Hello \v World!")</code></pre><p><strong>Output:</strong></p><pre><code>Hello 
 World!</code></pre>                      |
| \ooo            | Character with octal value | <pre><code>print("\110\145\154\154\157")Output:
Hello</code></pre>                                                                         |
| \xHH            | Character with hex value.  | <pre><code>print("\x48\x65\x6c\x6c\x6f")</code></pre><p><strong>Output:</strong></p><pre><code>Hello</code></pre>                          |

Here is the simple example of escape sequence.

```
// Some code
print("C:\\Users\\DEVANSH SHARMA\\Python32\\Lib")  
print("This is the \n multiline quotes")  
print("This is \x48\x45\x58 representation") 
```



We can ignore the escape sequence from the given string by using the raw string. We can do this by writing **r** or **R** in front of the string. Consider the following example.

`print(r"C:\\Users\\DEVANSH SHARMA\\Python32")` &#x20;

### The format() method

The **format()** method is the most flexible and useful method in formatting strings. The curly braces {} are used as the placeholder in the string and replaced by the **format()** method argument. Let's have a look at the given an example:

```
// Example code
# Using Curly braces  
print("{} and {} both are the best friend".format("Devansh","Abhishek"))  
  
#Positional Argument  
print("{1} and {0} best players ".format("Virat","Rohit"))  
  
#Keyword Argument  
print("{a},{b},{c}".format(a = "James", b = "Peter", c = "Ricky"))  
```

### Python String Formatting Using % Operator

Python allows us to use the format specifiers used in C's printf statement. The format specifiers in Python are treated in the same way as they are treated in C. However, Python provides an additional operator %, which is used as an interface between the format specifiers and their values. In other words, we can say that it binds the format specifiers to the values.

Consider the following example.

```
// Some code
Integer = 10;    
Float = 1.290    
String = "Devansh"    
print("Hi I am Integer ... My value is %d\nHi I am float ... My value is %f\nHi I am string ... My value is %s"%(Integer,Float,String))    
```

### String Length

To get the length of a string, use the `len()` function.

```
// Example code
#The len() function returns the length of a string:

a = "Hello, World!"
print(len(a))

```

### Python String functions

Python provides various in-built functions that are used for string handling. Many String fun

| Method                                                                                                | Description                                                                                                                                                                                                   |
| ----------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [capitalize()](https://www.javatpoint.com/python-string-capitalize-method)                            | It capitalizes the first character of the String. This function is deprecated in python3                                                                                                                      |
| [casefold()](https://www.javatpoint.com/python-string-casefold-method)                                | It returns a version of s suitable for case-less comparisons.                                                                                                                                                 |
| [center(width ,fillchar)](https://www.javatpoint.com/python-string-center-method)                     | It returns a space padded string with the original string centred with equal number of left and right spaces.                                                                                                 |
| [count(string,begin,end)](https://www.javatpoint.com/python-string-count-method)                      | It counts the number of occurrences of a substring in a String between begin and end index.                                                                                                                   |
| decode(encoding = 'UTF8', errors = 'strict')                                                          | Decodes the string using codec registered for encoding.                                                                                                                                                       |
| [encode()](https://www.javatpoint.com/python-string-encode-method)                                    | Encode S using the codec registered for encoding. Default encoding is 'utf-8'.                                                                                                                                |
| [endswith(suffix ,begin=0,end=len(string))](https://www.javatpoint.com/python-string-endswith-method) | It returns a Boolean value if the string terminates with given suffix between begin and end.                                                                                                                  |
| [expandtabs(tabsize = 8)](https://www.javatpoint.com/python-string-expandtabs-method)                 | It defines tabs in string to multiple spaces. The default space value is 8.                                                                                                                                   |
| [find(substring ,beginIndex, endIndex)](https://www.javatpoint.com/python-string-find-method)         | It returns the index value of the string where substring is found between begin index and end index.                                                                                                          |
| [format(value)](https://www.javatpoint.com/python-string-format-method)                               | It returns a formatted version of S, using the passed value.                                                                                                                                                  |
| [index(subsring, beginIndex, endIndex)](https://www.javatpoint.com/python-string-index-method)        | It throws an exception if string is not found. It works same as find() method.                                                                                                                                |
| [isalnum()](https://www.javatpoint.com/python-string-isalnum-method)                                  | It returns true if the characters in the string are alphanumeric i.e., alphabets or numbers and there is at least 1 character. Otherwise, it returns false.                                                   |
| [isalpha()](https://www.javatpoint.com/python-string-isalpha-method)                                  | It returns true if all the characters are alphabets and there is at least one character, otherwise False.                                                                                                     |
| [isdecimal()](https://www.javatpoint.com/python-string-isdecimal-method)                              | It returns true if all the characters of the string are decimals.                                                                                                                                             |
| [isdigit()](https://www.javatpoint.com/python-string-isdigit-method)                                  | It returns true if all the characters are digits and there is at least one character, otherwise False.                                                                                                        |
| [isidentifier()](https://www.javatpoint.com/python-string-isidentifier-method)                        | It returns true if the string is the valid identifier.                                                                                                                                                        |
| [islower()](https://www.javatpoint.com/python-string-islower-method)                                  | It returns true if the characters of a string are in lower case, otherwise false.                                                                                                                             |
| [isnumeric()](https://www.javatpoint.com/python-string-isnumeric-method)                              | It returns true if the string contains only numeric characters.                                                                                                                                               |
| [isprintable()](https://www.javatpoint.com/python-string-isprintable-method)                          | It returns true if all the characters of s are printable or s is empty, false otherwise.                                                                                                                      |
| [isupper()](https://www.javatpoint.com/python-string-isupper-method)                                  | It returns false if characters of a string are in Upper case, otherwise False.                                                                                                                                |
| [isspace()](https://www.javatpoint.com/python-string-isspace-method)                                  | It returns true if the characters of a string are white-space, otherwise false.                                                                                                                               |
| [istitle()](https://www.javatpoint.com/python-string-istitle-method)                                  | It returns true if the string is titled properly and false otherwise. A title string is the one in which the first character is upper-case whereas the other characters are lower-case.                       |
| [isupper()](https://www.javatpoint.com/python-string-isupper-method)                                  | It returns true if all the characters of the string(if exists) is true otherwise it returns false.                                                                                                            |
| [join(seq)](https://www.javatpoint.com/python-string-join-method)                                     | It merges the strings representation of the given sequence.                                                                                                                                                   |
| len(string)                                                                                           | It returns the length of a string.                                                                                                                                                                            |
| [ljust(width\[,fillchar\])](https://www.javatpoint.com/python-string-ljust-method)                    | It returns the space padded strings with the original string left justified to the given width.                                                                                                               |
| [lower()](https://www.javatpoint.com/python-string-lower-method)                                      | It converts all the characters of a string to Lower case.                                                                                                                                                     |
| [lstrip()](https://www.javatpoint.com/python-string-lstrip-method)                                    | It removes all leading whitespaces of a string and can also be used to remove particular character from leading.                                                                                              |
| [partition()](https://www.javatpoint.com/python-string-partition-method)                              | It searches for the separator sep in S, and returns the part before it, the separator itself, and the part after it. If the separator is not found, return S and two empty strings.                           |
| maketrans()                                                                                           | It returns a translation table to be used in translate function.                                                                                                                                              |
| [replace(old,new\[,count\])](https://www.javatpoint.com/python-string-replace-method)                 | It replaces the old sequence of characters with the new sequence. The max characters are replaced if max is given.                                                                                            |
| [rfind(str,beg=0,end=len(str))](https://www.javatpoint.com/python-string-rfind-method)                | It is similar to find but it traverses the string in backward direction.                                                                                                                                      |
| [rindex(str,beg=0,end=len(str))](https://www.javatpoint.com/python-string-rindex-method)              | It is same as index but it traverses the string in backward direction.                                                                                                                                        |
| [rjust(width,\[,fillchar\])](https://www.javatpoint.com/python-string-rjust-method)                   | Returns a space padded string having original string right justified to the number of characters specified.                                                                                                   |
| [rstrip()](https://www.javatpoint.com/python-string-rstrip-method)                                    | It removes all trailing whitespace of a string and can also be used to remove particular character from trailing.                                                                                             |
| [rsplit(sep=None, maxsplit = -1)](https://www.javatpoint.com/python-string-rsplit-method)             | It is same as split() but it processes the string from the backward direction. It returns the list of words in the string. If Separator is not specified then the string splits according to the white-space. |
| [split(str,num=string.count(str))](https://www.javatpoint.com/python-string-split-method)             | Splits the string according to the delimiter str. The string splits according to the space if the delimiter is not provided. It returns the list of substring concatenated with the delimiter.                |
| [splitlines(num=string.count('\n'))](https://www.javatpoint.com/python-string-splitlines-method)      | It returns the list of strings at each line with newline removed.                                                                                                                                             |
| [startswith(str,beg=0,end=len(str))](https://www.javatpoint.com/python-string-startswith-method)      | It returns a Boolean value if the string starts with given str between begin and end.                                                                                                                         |
| strip(\[chars])                                                                                       | It is used to perform lstrip() and rstrip() on the string.                                                                                                                                                    |
| [swapcase()](https://www.javatpoint.com/python-string-swapcase-method)                                | It inverts case of all characters in a string.                                                                                                                                                                |
| title()                                                                                               | It is used to convert the string into the title-case i.e., The string **meEruT** will be converted to Meerut.                                                                                                 |
| [translate(table,deletechars = '')](https://www.javatpoint.com/python-string-translate-method)        | It translates the string according to the translation table passed in the function .                                                                                                                          |
| [upper()](https://www.javatpoint.com/python-string-upper-method)                                      | It converts all the characters of a string to Upper Case.                                                                                                                                                     |
| [zfill(width)](https://www.javatpoint.com/python-string-zfill-method)                                 | Returns original string leftpadded with zeros to a total of width characters; intended for numbers, zfill() retains any sign given (less one zero).                                                           |
