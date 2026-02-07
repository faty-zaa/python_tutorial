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

conditions : if, elif, else, for else, while, while else, break, continue, pass

pass : Does nothing; a null operation.

break : Terminates the loop entirely.

continue : Skips the rest of the code inside the loop for the current iteration and proceeds to the next iteration.

return : Exits the current function and optionally returns a value

match-case has been introduced, which is similar to the switch-case construct available in C/C++/Java etc.
    EXAMPLE :
        match variable_name:
            case 'pattern 1' : statement 1
            case 'pattern 2' : statement 2

The for loop in Python provides the ability to loop over the items of any sequence --> for num in numbers:
                 total += num

# Data types

int (signed integers)

float (floating point real values)

complex (complex numbers)

string (non-numeric data type)

raw string is a string literal created by prefixing the string with the letter r or R. This tells the Python interpreter to treat backslashes (\) as literal characters, rather than as special escape characters. (raw_string = r"This is a newline:\n" --> This is a newline:\n)

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
we can cast a string to a list, modify the list using methods like insert(), append(), or remove() and then convert the list back to a string to obtain a modified version.

Defining a Python Function --> def function_name( parameters ):

Lambda forms can take any number of arguments but return just one value in the form of an expression --> sum = lambda arg1, arg2: arg1 + arg2; print ("Value of total : ", sum( 10, 20 ))

for more details (positional, arbitary, kyword & default arguments ...): https://www.tutorialspoint.com/python/python_functions.htm

# Python Operators

Addition(+), Subtraction(-), Multiplication(*), Division(/), Modulus(%), Exponent(**), floor division(// -> (9//2 = 4)), Equal(==), Not equal(!=), Greater/less than(> / <), Greater than or equal to(>=), Less than or equal to(<=), "and", "or" and "not"
for more : https://www.w3schools.com/python/python_operators.asp

# OOP (Object-oriented programming)

is defined as a programming model that uses the concept of objects which refers to real-world entities with state and behavior

Class → blueprint

Object → real thing

__init__ → setup function

self → the object itself

__main__
(if __name__ == "__main__") :
    Every Python file has a built-in variable called __name__.
    If you run the file directly, Python sets __name__ to "__main__".
    If the file is imported into another file, __name__ is set to the filename instead.

`Class attributes` are those variables that belong to a class and whose value is shared among all the instances of that class

`Built-In Class Attributes`:
__dict__ − Dictionary containing the class's namespace.

__doc__ − Class documentation string or none, if undefined.

__name__ − Class name.

__module__ − Module name in which the class is defined. This attribute is "__main__" in interactive mode.

__bases__ − A possibly empty tuple containing the base classes, in the order of their occurrence in the base class list.

`instance attribute` in Python is a variable that is specific to an individual object of a class. It is defined inside the __init__() method.

__init__ is a special function inside a class
p = Plant("Rose", 10, 3)
Python automatically calls:
Plant.__init__(p, "Rose", 10, 3)

We need __init__ to:

Give the object starting values

Make sure the object is ready to use

Avoid creating empty objects with no data
 ft_command_quest.py
`Encapsulation` = keeping data and the code that uses it together, and protecting it from misuse, it hide internal data & control how it is accessed or modified by using private attributes, setters and gtters

`Public Variables`: Public variables are accessible from anywhere, both inside and outside the class. In the image, a public place is considered as an analogy for public variables as they can be accessed by anyone.

`Protected Variables`: Protected variable can be accessed within the class and its subclasses. In the image, a private domicile is considered as an analogy for protected variables as they can be accessed by family members (subclasses) but not by outsiders.

`Private Variables`: Private variables are only accessible  within the class they are defined in. In the image, a vault is considered as an analogy for private variables as they can only be accessed by the owner (the class itself) and not by anyone else.

you can access the private variable using name mangling

`Name mangling` is:
    Python’s automatic renaming of class attributes that start with double underscores (__) to include the class name, in order to avoid name conflicts and accidental overrides, especially in subclasses.
        __name → _ClassName__name

`Inheritance` is:
    An OOP mechanism where a class derives from another class, reusing its behavior and state while guaranteeing that the derived class can be used anywhere the base class is expected without breaking program correctness.
    *super() function allows you to access methods and attributes of the parent class from within a child class.



`pass` is a do-nothing statement.
It tells Python:
“There must be a statement here, but I intentionally want nothing to happen.”

`raising error` :
    “This situation is invalid. Stop normal execution”
    *raise stops normal execution and signals that an error has occurred
    *Looks for the nearest matching except
    *If none is found → program crashes

`Exception` is the base class for almost  all runtime errors in Python
 you can defend your program by placing the suspicious code in a try: block. After the try: block, include an except: statement, followed by a block of code which handles the problem as elegantly as possible

 An `exception class` is a specialized class in object-oriented programming that serves as a blueprint for creating exception objects, which represent runtime errors or unusual conditions encountered during program execution
 
`The finally block` in Python is used within a try statement to define a section of code that will always execute, regardless of whether an exception was raised, handled, or not
The primary purpose of the finally block is to ensure that essential cleanup actions are performed in all circumstances
