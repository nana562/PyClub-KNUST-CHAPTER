# Syntax

### Quickstart

Python is an interpreted programming language, this means that as a developer you write Python (.py) files in a text editor and then put those files into the python interpreter to be executed.

The way to run a python file is like this on the command line:

**`C:\Users\pyclubKNUST>python helloworld.py`**

Where "helloworld.py" is the name of your python file.

Let's write our first Python file, called _**helloworld.py**_, which can be done in any text editor.

<mark style="background-color:green;">**helloworld.py**</mark>

`print("Hello, World!")`

Save your file. Open your command line, navigate to the directory where you saved your file, and run:&#x20;

**`C:\Users\pyclubKNUST>python helloworld.py`**

<mark style="background-color:green;">**The output:**</mark>

`Hello, World!`



### The Command-line

To test a short amount of code in python sometimes it is quickest and easiest not to write the code in a file. This is made possible because Python can be run as a command line itself.

Type the following on the Windows, Mac or Linux command line:

_**`"python"`**_ command did not work, you can try _**`"py":`**_

Type `print("Hello, World!")`

Whenever you are done in the python command line, you can simply type the following to quit the python command line interface:

_**exit()**_

Congratulations, you have written and executed your first Python program.

### **Python Identifiers**

A Python identifier is a name used to identify a variable, function, class, module or other object. An identifier starts with a letter A to Z or a to z or an underscore (\_) followed by zero or more letters, underscores and digits (0 to 9).

Python does not allow punctuation characters such as @, $, and % within identifiers. Python is a case sensitive programming language. Thus, **Manpower** and **manpower** are two different identifiers in Python.

Here are naming conventions for Python identifiers-

* Class names start with an uppercase letter. All other identifiers start with a lowercase letter.
* Starting an identifier with a single leading underscore indicates that the identifier is private.
* &#x20;Starting an identifier with two leading underscores indicates a strong private identifier.
* If the identifier also ends with two trailing underscores, the identifier is a language`-`defined special name.

### &#x20;**Reserved Words**

The following list shows the Python keywords. These are reserved words and you cannot use them as constants or variables or any other identifier names. All the Python keywords contain lowercase letters only.

| and      | exec    | Not    |
| -------- | ------- | ------ |
| as       | finally | or     |
| assert   | for     | pass   |
| break    | from    | print  |
| class    | global  | raise  |
| continue | if      | return |
| def      | import  | try    |
| del      | in      | while  |
| elif     | is      | with   |
| else     | lambda  | yield  |
| except   |         |        |

**Lines and Indentation**

Python does not use braces({}) to indicate blocks of code for class and function definitions or flow control. Blocks of code are denoted by line indentation, which is rigidly enforced.

The number of spaces in the indentation is variable, but all statements within the block must be indented the same amount. For example-

&#x20;

{% hint style="success" %}
**Good to know:** Spaces or Tabs?&#x20;

The recommended indentation is 4 spaces but tabs or spaces can be used so long as they are consistent. The spacing should be even and uniform throughout.
{% endhint %}

{% hint style="danger" %}
Do not mix tabs and spaces in Python as this will cause an error in Python 3 and can cause errors in Python 2.

Improper indentation can cause an IndentationError or cause the program to do something unexpected.
{% endhint %}

