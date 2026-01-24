# python_tutorial
*This introduction to python 3.10+ for beginners has been created by FALAMLIH*

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

`python basic sytax` : https://www.tutorialspoint.com/python/python_basic_syntax.htm
https://www.tutorialspoint.com/python/python_variables.htm

# the Python keywords

and as	assert break class continue def	del	elif else except False finally for from global if import in is lambda None nonlocal not or pass raise return True try while with yield

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

A Python variable refers to the object and not the memory location.

An object is stored in memory only once.

private variables are defined by adding a double underscore (__) and can't acess without using a method or Name Mangling(we'll see this in OOP).


 
