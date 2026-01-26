*This introduction to python 3.10+ for beginners has been created by FALAMLIH*

# Unicode System

universal character encoding standard that assigns a unique numeric value (code point) to every character, symbol, and emoji across all writing systems ,  The default encoding for Python source code is UTF-8.

# PYTHON

general-purpose interpreted, interactive, object-oriented, and high-level programming language. Python is dynamically-typed and garbage-collected programming language.

 Python is processed at runtime by the interpreter. You do not need to compile your program before executing it, also Python is a completely object-oriented language. Everything in a Python program is an object.

Using Python, we can perform:
*Web development*
*Data analysis and machine learning*
*Automation and scripting*
*Software testing and many more*

Python virtual environment is a self-contained, isolated directory tree that contains a specific Python installation and a separate set of installed packages. It allows developers to manage project-specific dependencies without interfering with other projects or the system-wide Python installation

# FROM CODE TO RESULT (Python Interpreter)

code in python go across 3 steps :
    `code.py`: file that contain the python source code.
    `Python Interpreter`: where the source code translate to   byte code not machine code (byte code is processed by a virtual machine, while machine code is processed by the CPU).
    `PVM`:python virtual machine reads and interprets this bytecode through an interpreter loop. The interpreter executes the instructions on the host machine, converting them into machine-level instructions that the computer's processor can understand and carry out.
    The Python VM maintains a Python object model to represent data types, such as integers, strings, lists, and custom objects. It manages the creation, manipulation, and destruction of these objects during execution.
    The Python VM handles memory allocation and garbage collection to manage the memory used by Python objects dynamically.


# print ("Hello, World!")

to write code in python, we don't have to use brackets{}, we've just to respect the (TAB) under kywords

`python basic sytax` : https://www.tutorialspoint.com/python/python_basic_syntax.htm
https://www.tutorialspoint.com/python/python_variables.htm

# the Python keywords

and as	assert break class continue def	del	elif else except False finally for from global if import in is lambda None nonlocal not or pass raise return True try while with yield

(#)single line comments

("" or """ """)multilines comments

# Data types

int (signed integers)

float (floating point real values)

complex (complex numbers)

string (non-numeric data type)

List Data Type : [2023, "hi", 3.11, 5+6j, 1.23E]

Tuple Data Type : (2023, "hi", 3.11, 5+6j, 1.23E) read-only lists

Range Data Type : range(start, stop, step)

bytes :  bytes() function or by prefixing a sequence of numbers with b

bytearray : you can modify the values stored in it after it is created (bytearray() function)

memoryview :  view into the memory of the original object ( memoryview())

Dictionary :  Data is stored as key: value pairs within curly braces {}
    Using curly braces
        my_dict = {"name": "Jake", "age": 22, "city": "London"}
    Using the dict() constructor
        another_dict = dict(brand="Ford", model="Mustang", year=1964)

set : an unordered collection of unique elements, Duplicate items are not allowed

Boolean : True / False

None : the null type of values or absence of a valuel

# Functions && Variables in Python

to get from the standard input we use:`input()`

to write to the standard output we use:`print()`

to get the adress of somthing:`id(something)`

to delete a variable:`del varible_name`

to know the type of varible:`type(varibal_name)`

we can declre multiple variables at once :`a,b,c = 1,2,"fatyzaa"`

type casting in python: `a = 3 --> a = str(3) --> a = '3'`

A variable name must start with a letter or the underscore character.

Python Local Variables are defined inside a function.

Python doesn't have any formally defined constants.

A Python variable refers to the object and not the memory 
location.
An object is stored in memory only once.

private variables are defined by adding a double underscore (__) and can't acess without using a method or Name Mangling(we'll see this in OOP).

Type casting :  the process of converting a value from one data type to another to ensure compatibility and perform specific operations

if, elif, else

match-case has been introduced, which is similar to the switch-case construct available in C/C++/Java etc.
    EXAMPLE :
        match variable_name:
            case 'pattern 1' : statement 1
            case 'pattern 2' : statement 2

The for loop in Python provides the ability to loop over the items of any sequence --> for num in numbers:
                                                                                            total += num


# Python Operators

Addition(+), Subtraction(-), Multiplication(*), Division(/), Modulus(%), Exponent(**), floor division(// -> (9//2 = 4)), Equal(==), Not equal(!=), Greater/less than(> / <), Greater than or equal to(>=), Less than or equal to(<=), "and", "or" and "not"
for more : https://www.w3schools.com/python/python_operators.asp
