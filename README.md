*This introduction to python 3.10+ for beginners has been created by FALAMLIH*

# Unicode System

universal character encoding standard that assigns a unique numeric value (code point) to every character, symbol, and emoji across all writing systems ,  The default encoding for Python source code is UTF-8.

# PYTHON

#!/usr/bin/python3

general-purpose interpreted, interactive, object-oriented, and high-level programming language. Python is dynamically-typed and garbage-collected programming language.

 Python is processed at runtime by the interpreter. You do not need to compile your program before executing it, also Python is a completely object-oriented language. Everything in a Python program is an object.

 iterpreter component:
| Parser                     |
| Compiler                   |
| Bytecode Generator         |
| Python Virtual Machine     |
| Garbage Collector          |
| Memory Manager             |
| Standard Library           |


The Python interpreter is the complete program you install and run (python or python3).
The Python Virtual Machine (PVM) is a component inside the interpreter that executes Python bytecode.
Python source code is first compiled to bytecode, then the PVM interprets that bytecode.
The CPU never executes Python bytecode directly; it executes the compiled machine code of the interpreter, which in turn carries out the bytecode's instructions.

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
    this is how to initialise an empty dictionnaty :
        keys = ['A', 'B', 'C', 'D']
        graph = dict.fromkeys(keys, [])

set : an unordered collection of unique elements, Duplicate items are not allowed

Boolean : True / False

None : the null type of values or absence of a valuel

# Some methods Python

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


# Python errors

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

`the with statement` is a control flow structure that ensures a setup action is performed when a block of code is entered and a corresponding cleanup action is performed when the block is exited, even if errors occur. This mechanism is known as a context manager.
it Replaces long try-except–finally blocks with cleaner syntax.
    If a file isn’t closed properly, you may get:
        resource leaks
        corrupted or incomplete data
        locked files
        crashes in long-running programs

# Python modules

A `module` is a file containing definition of functions, classes, variables, constants or any other Python object
Python has the import keyword for this purpose
    `SYS` :This module provides access to some variables used or maintained by the interpreter and to functions that interact strongly with the interpreter
    the sys module provides a variable called sys.argv. It's main purpose are:
    It is a list of command-line arguments.
    len(sys.argv) provides the number of command-line arguments.
    sys is a built-in Python module that gives your program direct access to the Python runtime and the operating system interface
The ____init__.py file in Python serves two primary purposes: it marks a directory as a regular Python package, and it provides a place for initialization code when that package is importe

# Python data types

`lists[]` :A List is a collection of ordered, mutable (Elements can be modified after creation) elements that can hold a variety of data types
    Example: [1, 2, 3, 4, 5]
we don't put values in list with index, we use append()

`sets{}` :A Set is an unordered collection of unique elements, Duplicate values are automatically removed, does not Support indexing and slicing
    Example: {1, 2, 3, 4, 5}
    `intersection`: used to see common data
    `union`: to union data
    `difference`: to see the unique data between datas

`Tuples()` :A Tuple is an ordered, immutable collection of elements, Once created, elements cannot be modified
Tuples are hashable and can be used as dictionary keys, unlike lists.
Hashable = something Python can lock in a box and trust it will never change
    Example: (1, 2, 3, 4, 5)
tuples protect the structure of your data
Tuples can be dictionary keys
    `Unpacking` means:
    Taking a collection (tuple, list, etc.) and assigning its elements to multiple variables in one line.

`Dictionaries{}` :A dictionary (dic()) is also a non-homogeneous data structure that stores key-value pairs, The dictionary doesn't allow duplicate keys
    Example: {1: "a", 2: "b", 3: "c", 4: "d", 5: "e"}
    ->keys() : gives you only the names
    ->values() : gives you only the values or numbers
    ->items() : name + number together as tuples
        You can loop like this:
            for item, quantity in bag.items():
                print(item, quantity)
    ->get() : Safely gets a value without crashing
        get(key, default)
            Means:
            “If the key exists → give me its value
            If it doesn’t exist → give me this default”
    ->update() : Adds or changes many things at once /ex:bag.update({"apple": 5, "pear": 2})
    !!!important: if you have nested dictionnaries, you can use ft.items() to get nested dictionnaries, and if there is another nested dict, use the key of each or loop to get values like that :
         print(players.items())
        print(players["alice"].items())
        print(players["bob"]["items"].items())

    
# Python generators && comprehension

`generator` is a function that acts as an iterator to produce a sequence of values one at a time, and only when requested. They are memory efficient because they don't store the entire sequence in memory at once; instead, they pause their execution with the `yield` keyword and resume when the next value is needed.

`comprehension`:


# python I/O

`open`:Python's built-in open() function is used to open files in various modes, such as reading, writing, and appending
    file = open("filename", "mode")
    Where, filename is the name of the file to open and mode is the mode in which the file is opened (e.g., 'r' for reading, 'w' for writing, 'a' for appending)
`r`:
Opens a file for reading only. The file pointer is placed at the beginning of the file. This is the default mode of open
`w`:
Opens a file for writing only. Overwrites the file if the file exists. If the file does not exist, creates a new file for writing

`CONTEXT MANAGERS`

`WITH STATEMENT`

`RAII`

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

__init__ is a special function inside a class (called constructor)
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

# POLYMORPHISM AND ABSTRACTION
    Polymorphism means "many forms". In programming it means "many types" and refers to the possibility that a single object may have multiple types.
    
`ABSTRACT CLASSES`:
    A class that cannot be instantiated directly; it defines a template for its subclasses
    it Forces all subclasses to implement certain methods
[text](https://www.cs.sjsu.edu/faculty/pearce/modules/lectures/ood3/concepts/polymorphism.htm)

`protocol`:


# venv
A separate Python workspace with its own packages and Python interpreter
to creat a virtual env:
    python -m venv matrix_env

to activate it:
    source matrix_env/bin/activate
if sys.base_prefix != sys.prefix: you are in the venv
base_prefix is the name of the envirenement of the user

there is a private data that we need to protect and don't put directly in our code, so we use :
   load_dotenv() method to load them from .env to memory to use them
   to check if the variable we need exist, we do : os.getenv("var_name")
   to check if .env file exist: os.path.exists("filename")

`.toml` is a configuration file format, It only stores structured data

`Poetry` reads and uses pyproject.toml
It uses it to:
    *create virtual environment
    *install dependencies
    *manage project

Poetry creates a virtual environment for your project automatically in:
    * ~/.cache/pypoetry/virtualenvs/
    (poetry env info)

# pydantic (BaseModel)
`BaseModel` tells that the data will entrer must have a defined form

`Field` is a function used to define validation rules, default values, and metadata for attributes in a BaseModel

`model validator` is logic that checks or modifies the entire model’s data to ensure it is valid.
Model validator modes:
1. mode="before"
    Runs before validation of field
    Receives raw input (dict)
2. mode="after"
    Runs after validation of field
    Works with the final model instance
str : min_length, max_length, pattern, strip_whitespace, to_lower, to_upper
int, float : gt (>), ge(>=), lt(<), le(<=), multiple_of
bool: default, description, alias
list: min_length, max_length
`Enum` lets you create a variable that can only take predefined values.

# Lambda

`lambda` is a small anonymous function written in one line, used for simple operations without defining a full function.
        Exs: add = lambda x, y: x + y
            (lambda x: x + 1)(5)
            list(map(lambda x: x * 2, nums))
# Functions

`Callables` in Python are anything you can “call” using parentheses () like a function
`*args` → many positional arguments → tuple
`**kwargs` → many keyword arguments → dict
`nonlocal` -> a keyword that lets a function modify a variable from its outer (enclosing) function.
    nonlocal only works if the variable already exists in an outer function
    It does NOT work for global variables
    It MUST be declared before using the variable

In Python, a first-class citizen (or first-class object) is an entity that is treated like any other value in the language. This means it can be manipulated, passed around, and used without restrictions. 
While many programming languages treat basic data types (like integers and strings) as first-class citizens, Python is notable for treating functions and classes as first-class citizens as well.

# TYPES OF METHODS

                    User class
                       │
          ┌────────────┼────────────┐
          ↓            ↓            ↓
     Instance       Class        Static
      method        method        method
          │            │            │
        self          cls          nothing
          │            │            │
       object        class       independent

                              PYTHON METHODS
                                    │
              ┌─────────────────────┼─────────────────────┐
              ↓                     ↓                     ↓
       INSTANCE METHOD         CLASS METHOD         STATIC METHOD
              │                     │                     │
            self                   cls                 nothing
              │                     │                     │
           object                 class             independent
              │                     │                     │
      ┌───────┼───────┐             │             ┌──────┴──────┐
      ↓       ↓       ↓             ↓             ↓             ↓
    object   object   object     class state     utility      helper
    state    methods  attrs      /constructor   function     logic

                              SPECIAL METHODS
                                    │
                           "__" + name + "__"
                                    │
                    ┌───────────────┼───────────────┐
                    ↓               ↓               ↓
                 __init__        __str__         __len__
                    │               │               │
                 creation        print()          len()
                    │               │               │
                  object          object          object


                              OPERATOR METHODS
                                    │
                 ┌──────────────────┼──────────────────┐
                 ↓                  ↓                  ↓
              __add__            __eq__             __lt__
                 │                  │                  │
                +                  ==                  <
                 │                  │                  │
             a + b              a == b              a < b


                              ABSTRACT METHODS
                                    │
                            @abstractmethod
                                    │
                              ┌─────┴─────┐
                              ↓           ↓
                          interface   requirement
                              │           │
                              └─────┬─────┘
                                    ↓
                              subclass MUST
                              implement it


                               PROPERTY
                                  │
                             @property
                                  │
                    ┌─────────────┼─────────────┐
                    ↓             ↓             ↓
                  getter        setter        deleter
                    │             │             │
                  read          modify        delete
                    │             │             │
               object.attr   object.attr = x   del object.attr
