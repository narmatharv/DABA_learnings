## What is Python?
```
Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

It is used for:

web development (server-side),
software development,
mathematics,
system scripting.
```

## What can Python do?
```
Python can be used on a server to create web applications.
Python can be used alongside software to create workflows.
Python can connect to database systems. It can also read and modify files.
Python can be used to handle big data and perform complex mathematics.
Python can be used for rapid prototyping, or for production-ready software development.
```

## Why Python?
```
Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
Python has a simple syntax similar to the English language.
Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.
Python can be treated in a procedural way, an object-oriented way or a functional way.

```

## Good to know
```
The most recent major version of Python is Python 3, which we shall be using in this tutorial. However, Python 2, although not being updated with anything other than security updates, is still quite popular.
In this tutorial Python will be written in a text editor. It is possible to write Python in an Integrated Development Environment, such as Thonny, Pycharm, Netbeans or Eclipse which are particularly useful when managing larger collections of Python files.
```

## Python Syntax compared to other programming languages

```
Python was designed for readability, and has some similarities to the English language with influence from mathematics.
Python uses new lines to complete a command, as opposed to other programming languages which often use semicolons or parentheses.
Python relies on indentation, using whitespace, to define scope; such as the scope of loops, functions and classes. Other programming languages often use curly-brackets for this purpose.

```

# CREATE A NEW PYTHON PROJECT
```
1. To check python version on your mac
      python --version

2. Create a new folder using terminal
      mkdir Python

3. Go to folder
      cd Python

4. Create a new file with .py extension
      touch helloworld.py

5. To start writing code, directly run the command
      python3

6. Type print("Hello World") and enter
   output: Hello World

Note: you can also open the IDLE, right click on the file name(helloworld.py) and open with IDLE and enter the above code.

```

## Python Indentation
```
Indentation refers to the spaces at the beginning of a code line.

Where in other programming languages the indentation in code is for readability only, the indentation in Python is very important.

Python uses indentation to indicate a block of code.

Eg:
      if 5 > 2:
        print("Five is greater than two!")

Python will give you an error if you skip the indentation:

Example
Syntax Error:

if 5 > 2:
print("Five is greater than two!")

The number of spaces is up to you as a programmer, the most common use is four, but it has to be at least one.

Example
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 

You have to use the same number of spaces in the same block of code, otherwise Python will give you an error:

Example
Syntax Error:

if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!")
```

## Python Variables
```
Variables are containers for storing data values.

1. Creating Variables
      Python has no command for declaring a variable.
      
      In Python, variables are created when you assign a value to it:
      
      Example
      Variables in Python:
      
      x = 5
      y = "Hello, World!"
      
      print(x)
      print(y)
      
      Variables do not need to be declared with any particular type, and can even change type after they have been set.
      
      Example
      x = 4       # x is of type int
      x = "Sally" # x is now of type str
      print(x)
      
      o/p: Sally

2. Casting
      If you want to specify the data type of a variable, this can be done with casting.
      
      Example
      x = str(3)    # x will be '3'
      y = int(3)    # y will be 3
      z = float(3)  # z will be 3.0

      print(x)
      print(y)
      print(z)
      
      o/p:
      3
      3
      3.0

3. Get the Type
      You can get the data type of a variable with the type() function.
      Example
      x = 5
      y = "John"
      print(type(x))
      print(type(y))
      
      o/p:
      <class 'int'>
      <class 'str'>

4. Single or Double Quotes?
      String variables can be declared either by using single or double quotes:
      
      Example
      x = "John"
      # is the same as
      x = 'John'

5. Case-Sensitive
      Variable names are case-sensitive.
      
      Example
      This will create two variables:
      
      a = 4
      A = "Sally"
      #A will not overwrite a

```

## Variable Names
```
Variable Names
      A variable can have a short name (like x and y) or a more descriptive name (age, carname, total_volume). Rules for Python variables:
      A variable name must start with a letter or the underscore character
      A variable name cannot start with a number
      A variable name can only contain alpha-numeric characters and underscores (A-z, 0-9, and _ )
      Variable names are case-sensitive (age, Age and AGE are three different variables)
      A variable name cannot be any of the Python keywords.

Example
      Legal variable names:
      
      myvar = "John"
      my_var = "John"
      _my_var = "John"
      myVar = "John"
      MYVAR = "John"
      myvar2 = "John"

Multi Words Variable Names
      Variable names with more than one word can be difficult to read.
      
      There are several techniques you can use to make them more readable:

1. Camel Case
      Each word, except the first, starts with a capital letter:
      
      myVariableName = "John"

2. Pascal Case
      Each word starts with a capital letter:

      MyVariableName = "John"

3. Snake Case
      Each word is separated by an underscore character:

      my_variable_name = "John"

```

## Assign Multiple Values
```
Many Values to Multiple Variables
Python allows you to assign values to multiple variables in one line:

Example
x, y, z = "Orange", "Banana", "Cherry"
print(x)
print(y)
print(z)

1. One Value to Multiple Variables
      And you can assign the same value to multiple variables in one line:
      
      Example
      x = y = z = "Orange"
      print(x)
      print(y)
      print(z)

2. Unpack a Collection
      If you have a collection of values in a list, tuple etc. Python allows you to extract the values into variables. This is called unpacking.
      
      Example
      Unpack a list:
      
      fruits = ["apple", "banana", "cherry"]
      x, y, z = fruits
      print(x)
      print(y)
      print(z)

      o/p:
            apple
            banana
            cherry
```

## Output Variables
```
The Python print() function is often used to output variables.

Example
x = "Python is awesome"
print(x)

In the print() function, you output multiple variables, separated by a comma:

Example
x = "Python"
y = "is"
z = "awesome"
print(x, y, z)
Output : Python is awesome

You can also use the + operator to output multiple variables:

Example
x = "Python "
y = "is "
z = "awesome"
print(x + y + z)

For numbers, the + character works as a mathematical operator:

Example
x = 5
y = 10
print(x + y)
o/p: 15

In the print() function, when you try to combine a string and a number with the + operator, Python will give you an error:

Example
x = 5
y = "John"
print(x + y)

The best way to output multiple variables in the print() function is to separate them with commas, which even support different data types:

Example
x = 5
y = "John"
print(x, y)
o/p: 5 John

```

## Global Variables
```
Variables that are created outside of a function (as in all of the examples above) are known as global variables.
Global variables can be used by everyone, both inside of functions and outside.

Example
Create a variable outside of a function, and use it inside the function

      x = "awesome"
      
      def myfunc():
        print("Python is " + x)
      
      myfunc()

If you create a variable with the same name inside a function, this variable will be local, and can only be used inside the function. The global variable with the same name will remain as it was, global and with the original value.

Example
Create a variable inside a function, with the same name as the global variable

      x = "awesome"
      
      def myfunc():
        x = "fantastic"
        print("Python is " + x)
      
      myfunc()
      
      print("Python is " + x)

1. The global Keyword
      Normally, when you create a variable inside a function, that variable is local, and can only be used inside that function.
      
      To create a global variable inside a function, you can use the global keyword.
      
      Example
      If you use the global keyword, the variable belongs to the global scope:
      
      def myfunc():
        global x
        x = "fantastic"
      
      myfunc()
      
      print("Python is " + x)

i) Also, use the global keyword if you want to change a global variable inside a function.

      Example
      To change the value of a global variable inside a function, refer to the variable by using the global keyword:
      
      x = "awesome"
      
      def myfunc():
        global x
        x = "fantastic"
      
      myfunc()
      
      print("Python is " + x)

      output: Python is fantastic

```

 ## Python Keywords
 ```
      Refer this: https://www.w3schools.com/python/python_ref_keywords.asp
 ```

## Data Types
```


