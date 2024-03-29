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
1. Built-in Data Types

      In programming, data type is an important concept.

      Variables can store data of different types, and different types can do different things.
      
      Python has the following data types built-in by default, in these categories:
      
      Text Type:	str
      Numeric Types:	int, float, complex
      Sequence Types:	list, tuple, range
      Mapping Type:	dict
      Set Types:	set, frozenset
      Boolean Type:	bool
      Binary Types:	bytes, bytearray, memoryview
      None Type:	NoneType

2. Getting the Data Type
      You can get the data type of any object by using the type() function:
      
      Example
      Print the data type of the variable x:
      
      x = 5
      print(type(x))

3. Setting the Data Type
      In Python, the data type is set when you assign a value to a variable:

      Example	                                Data Type	
      x = "Hello World"	                             str	
      x = 20	                                   int	
      x = 20.5	                                    float	
      x = 1j	                                    complex	
      x = ["apple", "banana", "cherry"]	            list	
      x = ("apple", "banana", "cherry")	            tuple	
      x = range(6)	                              range	
      x = {"name" : "John", "age" : 36}	            dict	
      x = {"apple", "banana", "cherry"}	            set	
      x = frozenset({"apple", "banana", "cherry"})	frozenset	
      x = True	                                    bool	
      x = b"Hello"	                              bytes	
      x = bytearray(5)	                              bytearray	
      x = memoryview(bytes(5))	                  memoryview	
      x = None	                                    NoneType

4. Setting the Specific Data Type
      In Python, the data type is set when you assign a value to a variable:
      Example	                                  Data Type	
      x = str("Hello World")	                        str	
      x = int(20)	                                    int	
      x = float(20.5)	                              float	
      x = complex(1j)	                              complex	
      x = list(("apple", "banana", "cherry"))	      list	
      x = tuple(("apple", "banana", "cherry"))	      tuple	
      x = range(6)	                              range	
      x = dict(name="John", age=36)	                  dict	
      x = set(("apple", "banana", "cherry"))	      set	
      x = frozenset(("apple", "banana", "cherry"))	frozenset	
      x = bool(5)	                                    bool	
      x = bytes(5)	                              bytes	
      x = bytearray(5)	                              bytearray	
      x = memoryview(bytes(5))	                  memoryview
````

## Python Numbers
```
      There are three numeric types in Python:
      
      int
      float
      complex
      Variables of numeric types are created when you assign a value to them:
      
      ExampleGet your own Python Server
      x = 1    # int
      y = 2.8  # float
      z = 1j   # complex

      To verify the type of any object in Python, use the type() function:
      
      Example
      print(type(x))
      print(type(y))
      print(type(z))
      
1. Int
      Int, or integer, is a whole number, positive or negative, without decimals, of unlimited length.
      
      Example
      Integers:
      
      x = 1
      y = 35656222554887711
      z = -3255522
      
      print(type(x))
      print(type(y))
      print(type(z))

      o/p:
      <class 'int'>
      <class 'int'>
      <class 'int'>

2. Float
      Float, or "floating point number" is a number, positive or negative, containing one or more decimals.
      
      Example
      Floats:
      
      x = 1.10
      y = 1.0
      z = -35.59
      
      print(type(x))
      print(type(y))
      print(type(z))

      Float can also be scientific numbers with an "e" to indicate the power of 10.
      
      Example
      Floats:
      
            x = 35e3
            y = 12E4
            z = -87.7e100
            
            print(type(x))
            print(type(y))
            print(type(z))

3. Complex
      Complex numbers are written with a "j" as the imaginary part:
      
      Example
      Complex:
      
      x = 3+5j
      y = 5j
      z = -5j
      
      print(type(x))
      print(type(y))
      print(type(z))

4. Type Conversion
      You can convert from one type to another with the int(), float(), and complex() methods:
      Example
      Convert from one type to another:
      
      x = 1    # int
      y = 2.8  # float
      z = 1j   # complex
      
      #convert from int to float:
      a = float(x)
      
      #convert from float to int:
      b = int(y)
      
      #convert from int to complex:
      c = complex(x)
      
      print(a)
      print(b)
      print(c)
      
      print(type(a))
      print(type(b))
      print(type(c))
      
      output:
      1.0
      2
      (1+0j)
      <class 'float'>
      <class 'int'>
      <class 'complex'>

5. Random Number
      Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers:
      
      Example
      Import the random module, and display a random number between 1 and 9:
      
      import random
      
      print(random.randrange(1, 10))

      o/p: 5
```

## Python Casting
```
1. Specify a Variable Type
      There may be times when you want to specify a type on to a variable. This can be done with casting. Python is an object-orientated language, and as such it uses classes to define          data types, including its primitive types.
      
      Casting in python is therefore done using constructor functions:
      
      int() - constructs an integer number from an integer literal, a float literal (by removing all decimals), or a string literal (providing the string represents a whole number)
      float() - constructs a float number from an integer literal, a float literal or a string literal (providing the string represents a float or an integer)
      str() - constructs a string from a wide variety of data types, including strings, integer literals and float literals

      Example 1:
      Integers:
      
            x = int(1)   # x will be 1
            y = int(2.8) # y will be 2
            z = int("3") # z will be 3
            print(x)
            print(y)
            print(z)
            o/p:
            1
            2
            3

      Example 2:
      Floats:
      
            x = float(1)     # x will be 1.0
            y = float(2.8)   # y will be 2.8
            z = float("3")   # z will be 3.0
            w = float("4.2") # w will be 4.2

      Example 3:
      Strings:
      
            x = str("s1") # x will be 's1'
            y = str(2)    # y will be '2'
            z = str(3.0)  # z will be '3.0'
```

## Python Strings
```
1. Strings
      Strings in python are surrounded by either single quotation marks, or double quotation marks.
      
      'hello' is the same as "hello".
      
      You can display a string literal with the print() function:
      
      Example
      print("Hello")
      print('Hello')

2. Assign String to a Variable
      Assigning a string to a variable is done with the variable name followed by an equal sign and the string:
      
      Example
      a = "Hello"
      print(a)

3.Multiline Strings
      You can assign a multiline string to a variable by using three quotes:
      
      Example
      You can use three double quotes:
      
      a = """Lorem ipsum dolor sit amet,
      consectetur adipiscing elit,
      sed do eiusmod tempor incididunt
      ut labore et dolore magna aliqua."""
      print(a)

4. Strings are Arrays
      Like many other popular programming languages, strings in Python are arrays of bytes representing unicode characters.
      
      However, Python does not have a character data type, a single character is simply a string with a length of 1.
      
      Square brackets can be used to access elements of the string.
      
      Example
      Get the character at position 1 (remember that the first character has the position 0):
      
      a = "Hello, World!"
      print(a[1])

      o/p: e

5. Looping Through a String
      Since strings are arrays, we can loop through the characters in a string, with a for loop.
      
      Example
      Loop through the letters in the word "banana":
      
      for x in "banana":
        print(x)
      o/p:
      b
      a
      n
      a
      n
      a

6. String Length
      To get the length of a string, use the len() function.
      
      Example
      The len() function returns the length of a string:
      
      a = "Hello, World!"
      print(len(a))

      o/p: 13

7. Check String
      To check if a certain phrase or character is present in a string, we can use the keyword in.
      
      Example
      Check if "free" is present in the following text:
      
      txt = "The best things in life are free!"
      print("free" in txt)
      o/p: True

      Use it in an if statement:
      
      Example
      Print only if "free" is present:
      
      txt = "The best things in life are free!"
      if "free" in txt:
        print("Yes, 'free' is present.")

8. Check if NOT
      To check if a certain phrase or character is NOT present in a string, we can use the keyword not in.
      
      Example
      Check if "expensive" is NOT present in the following text:
      
      txt = "The best things in life are free!"
      print("expensive" not in txt)
      o/p: True

      Use it in an if statement:
      
      Example
      print only if "expensive" is NOT present:
      
      txt = "The best things in life are free!"
      if "expensive" not in txt:
        print("No, 'expensive' is NOT present.")
```

## Python - Slicing Strings
```
1. Slicing
      You can return a range of characters by using the slice syntax.
      
      Specify the start index and the end index, separated by a colon, to return a part of the string.
      
      ExampleGet your own Python Server
      Get the characters from position 2 to position 5 (not included):
      
      b = "Hello, World!"
      print(b[2:5])
      o/p: llo

2.Slice From the Start
      By leaving out the start index, the range will start at the first character:
      
      Example
      Get the characters from the start to position 5 (not included):
      
      b = "Hello, World!"
      print(b[:5])

      o/p: Hello

3. Slice To the End
      By leaving out the end index, the range will go to the end:
      
      Example
      Get the characters from position 2, and all the way to the end:
      
      b = "Hello, World!"
      print(b[2:])
      o/p: llo, World!

4. Negative Indexing
      Use negative indexes to start the slice from the end of the string:

      Example
      Get the characters:
      From: "o" in "World!" (position -5)
      To, but not included: "d" in "World!" (position -2):
      
      b = "Hello, World!"
      print(b[-5:-2])

      o/p: orl
```

## Python - Modify Strings
```
Python has a set of built-in methods that you can use on strings.

1. Upper Case
      Example
      The upper() method returns the string in upper case:
      
      a = "Hello, World!"
      print(a.upper())

      o/p: HELLO, WORLD!

2. Lower Case
      Example
      The lower() method returns the string in lower case:
      
      a = "Hello, World!"
      print(a.lower())

3. Remove Whitespace
      Whitespace is the space before and/or after the actual text, and very often you want to remove this space.
      
      Example
      The strip() method removes any whitespace from the beginning or the end:
      
      a = " Hello, World! "
      print(a.strip()) # returns "Hello, World!"

      o/p: Hello, World!

4. Replace String
      Example
      The replace() method replaces a string with another string:
      
      a = "Hello, World!"
      print(a.replace("H", "J"))
      o/p: Jello World

5. Split String
      The split() method returns a list where the text between the specified separator becomes the list items.
      
      Example
      The split() method splits the string into substrings if it finds instances of the separator:
      
      a = "Hello, World!"
      print(a.split(",")) # returns ['Hello', ' World!']

      o/p: ['Hello', ' World!']

````

## Python - String Concatenation
```
1. String Concatenation
      To concatenate, or combine, two strings you can use the + operator.
      
      Example 1:
      Merge variable a with variable b into variable c:
      
      a = "Hello"
      b = "World"
      c = a + b
      print(c)
      o/p: HelloWorld

Example 2:
      To add a space between them, add a " ":
      
      a = "Hello"
      b = "World"
      c = a + " " + b
      print(c)

      o/p: Hello World

```

## Python - Format - Strings
```
1. String Format
      As we learned in the Python Variables chapter, we cannot combine strings and numbers like this:
      
      Example 1:
      age = 36
      txt = "My name is John, I am " + age
      print(txt)
      
      But we can combine strings and numbers by using the format() method!
      
      The format() method takes the passed arguments, formats them, and places them in the string where the placeholders {} are:
      
      Example 2:
      Use the format() method to insert numbers into strings:
      
      age = 36
      txt = "My name is John, and I am {}"
      print(txt.format(age))
      
      o/p: My name is John, and I am 36

      The format() method takes unlimited number of arguments, and are placed into the respective placeholders:

      Example 3:
            quantity = 3
            itemno = 567
            price = 49.95
            myorder = "I want {} pieces of item {} for {} dollars."
            print(myorder.format(quantity, itemno, price))
            
            o/p: I want 3 pieces of item 567 for 49.95 dollars.
      
      You can use index numbers {0} to be sure the arguments are placed in the correct placeholders:
      
      Example 4:
            quantity = 3
            itemno = 567
            price = 49.95
            myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
            print(myorder.format(quantity, itemno, price))

            o/p: I want to pay 49.95 dollars for 3 pieces of item 567

```


## Python - Escape Characters
```
1. Escape Character
      To insert characters that are illegal in a string, use an escape character.
      
      An escape character is a backslash \ followed by the character you want to insert.
      
      An example of an illegal character is a double quote inside a string that is surrounded by double quotes:
      
      Example 1:
      You will get an error if you use double quotes inside a string that is surrounded by double quotes:
      
      txt = "We are the so-called "Vikings" from the north."
      
      
      To fix this problem, use the escape character \":

      Example 2:
      The escape character allows you to use double quotes when you normally would not be allowed:
      
      txt = "We are the so-called \"Vikings\" from the north."
      
      o/p: We are the so-called "Vikings" from the north.

      Escape Characters
      Other escape characters used in Python:
      
      Code	Result	
      \'	Single Quote	
      \\	Backslash	
      \n	New Line	
      \r	Carriage Return	
      \t	Tab	
      \b	Backspace	
      \f	Form Feed	
      \ooo	Octal value	
      \xhh	Hex value

```


## Python - String Methods
```
Python has a set of built-in methods that you can use on strings.

Note: All string methods return new values. They do not change the original string.

Method	Description
capitalize()	Converts the first character to upper case
casefold()	Converts string into lower case
center()	Returns a centered string
count()	Returns the number of times a specified value occurs in a string
encode()	Returns an encoded version of the string
endswith()	Returns true if the string ends with the specified value
expandtabs()	Sets the tab size of the string
find()	Searches the string for a specified value and returns the position of where it was found
format()	Formats specified values in a string
format_map()	Formats specified values in a string
index()	Searches the string for a specified value and returns the position of where it was found
isalnum()	Returns True if all characters in the string are alphanumeric
isalpha()	Returns True if all characters in the string are in the alphabet
isascii()	Returns True if all characters in the string are ascii characters
isdecimal()	Returns True if all characters in the string are decimals
isdigit()	Returns True if all characters in the string are digits
isidentifier()	Returns True if the string is an identifier
islower()	Returns True if all characters in the string are lower case
isnumeric()	Returns True if all characters in the string are numeric
isprintable()	Returns True if all characters in the string are printable
isspace()	Returns True if all characters in the string are whitespaces
istitle()	Returns True if the string follows the rules of a title
isupper()	Returns True if all characters in the string are upper case
join()	Joins the elements of an iterable to the end of the string
ljust()	Returns a left justified version of the string
lower()	Converts a string into lower case
lstrip()	Returns a left trim version of the string
maketrans()	Returns a translation table to be used in translations
partition()	Returns a tuple where the string is parted into three parts
replace()	Returns a string where a specified value is replaced with a specified value
rfind()	Searches the string for a specified value and returns the last position of where it was found
rindex()	Searches the string for a specified value and returns the last position of where it was found
rjust()	Returns a right justified version of the string
rpartition()	Returns a tuple where the string is parted into three parts
rsplit()	Splits the string at the specified separator, and returns a list
rstrip()	Returns a right trim version of the string
split()	Splits the string at the specified separator, and returns a list
splitlines()	Splits the string at line breaks and returns a list
startswith()	Returns true if the string starts with the specified value
strip()	Returns a trimmed version of the string
swapcase()	Swaps cases, lower case becomes upper case and vice versa
title()	Converts the first character of each word to upper case
translate()	Returns a translated string
upper()	Converts a string into upper case
zfill()	Fills the string with a specified number of 0 values at the beginning

```

## Python Booleans
```
Booleans represent one of two values: True or False.

1. Boolean Values
      In programming you often need to know if an expression is True or False.
      
      You can evaluate any expression in Python, and get one of two answers, True or False.
      
      When you compare two values, the expression is evaluated and Python returns the Boolean answer:
      
      Example 1:
            print(10 > 9)
            print(10 == 9)
            print(10 < 9)
      
      When you run a condition in an if statement, Python returns True or False:
      
      Example 2:
      Print a message based on whether the condition is True or False:
      
            a = 200
            b = 33
            
            if b > a:
              print("b is greater than a")
            else:
              print("b is not greater than a")


2. Evaluate Values and Variables
      The bool() function allows you to evaluate any value, and give you True or False in return,

      Example
      Evaluate a string and a number:
      
      print(bool("Hello"))
      print(bool(15))
      
      o/p:
      True
      True

3. Most Values are True
      Almost any value is evaluated to True if it has some sort of content.
      
      Any string is True, except empty strings.
      
      Any number is True, except 0.
      
      Any list, tuple, set, and dictionary are True, except empty ones.
      
      Example
      The following will return True:
      
      bool("abc")
      bool(123)
      bool(["apple", "cherry", "banana"])
      
      o/p:
      True
      True
      True

4. Some Values are False
      In fact, there are not many values that evaluate to False, except empty values, such as (), [], {}, "", the number 0, and the value None. And of course the value False evaluates to       False.
      
      Example 1:
      The following will return False:
      
      bool(False)
      bool(None)
      bool(0)
      bool("")
      bool(())
      bool([])
      bool({})

      o/p:
      False
      False
      False
      False
      False
      False
      False
      
      One more value, or object in this case, evaluates to False, and that is if you have an object that is made from a class with a __len__ function that returns 0 or False:
      
      Example 2:
            class myclass():
              def __len__(self):
                return 0
            
            myobj = myclass()
            print(bool(myobj))

      o/p: False


5. Functions can Return a Boolean
      You can create functions that returns a Boolean Value:
      
      Example
            Print the answer of a function:
            
            def myFunction() :
              return True
            
            print(myFunction())

      o/p: True

      You can execute code based on the Boolean answer of a function:
      
      Example
      Print "YES!" if the function returns True, otherwise print "NO!":
      
            def myFunction() :
              return True
            
            if myFunction():
              print("YES!")
            else:
              print("NO!")


      Python also has many built-in functions that return a boolean value, like the isinstance() function, which can be used to determine if an object is of a certain data type:
      
      Example
      Check if an object is an integer or not:
      
            x = 200
            print(isinstance(x, int))
      
      o/p: True

```


## Python Operators
```
Operators are used to perform operations on variables and values.

In the example below, we use the + operator to add together two values:

Example
      print(10 + 5)

Python divides the operators in the following groups:

Arithmetic operators
Assignment operators
Comparison operators
Logical operators
Identity operators
Membership operators
Bitwise operators


1.Python Arithmetic Operators
      Arithmetic operators are used with numeric values to perform common mathematical operations:
      
      Operator	Name	            Example	
      +	      Addition	      x + y	
      -	      Subtraction	      x - y	
      *	      Multiplication	x * y	
      /	      Division	      x / y	
      %	      Modulus	      x % y	
      **	      Exponentiation	x ** y	
      //	      Floor division	x // y	

2. Python Assignment Operators
      Assignment operators are used to assign values to variables:

      Operator	Example	Same As	
      =	      x = 5	      x = 5	
      +=	      x += 3	x = x + 3	
      -=	      x -= 3	x = x - 3	
      *=	      x *= 3	x = x * 3	
      /=	      x /= 3	x = x / 3	
      %=	      x %= 3	x = x % 3	
      //=	      x //= 3	x = x // 3	
      **=	      x **= 3	x = x ** 3	
      &=	      x &= 3	x = x & 3	
      |=	      x |= 3	x = x | 3	
      ^=	      x ^= 3	x = x ^ 3	
      >>=	      x >>= 3	x = x >> 3	---> bitwise operator, right shift
      Eg:
      x = 5
      x >>= 3
      print(x)
      
      o/p: 0
      Here x=5, 5>>3
      here 5 in binary code is 101, so we need to shift right by 3 bits, so result is 0, since we have only 3 digits.

      <<=	      x <<= 3	x = x << 3	---> bitwise operator, left shift

      Eg:
      x = 5
      x <<= 3
      print(x)
      
      
      o/p: 40
      5<<3, 5 in binary is 101, we need to shift 3 bits left, 101000 which is 40 in decimal.


3. Python Comparison Operators
      Comparison operators are used to compare two values:
      
      Operator	Name	                        Example	
      ==	      Equal	                        x == y	
      !=	      Not equal	                  x != y	
      >	      Greater than	            x > y	
      <	      Less than	                  x < y	
      >=	      Greater than or equal to	x >= y	
      <=	      Less than or equal to	      x <= y
      
      
4. Python Logical Operators
      Logical operators are used to combine conditional statements:
      
      Operator	Description	                                                Example	
      and 	      Returns True if both statements are true	                  x < 5 and  x < 10	
      or	      Returns True if one of the statements is true	            x < 5 or x < 4	
      not	      Reverse the result, returns False if the result is true	not(x < 5 and x < 10)

5.Python Identity Operators
      Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object, with the same memory location:
      
      Operator	            Description	                                    Example	
      is 	      Returns True if both variables are the same object	      x is y	
      is not	Returns True if both variables are not the same object	x is not y

6. Python Membership Operators
      Membership operators are used to test if a sequence is presented in an object:
      
      Operator	      Description	                                                                        Example	
      in 	            Returns True if a sequence with the specified value is present in the object	      x in y	
      not in	      Returns True if a sequence with the specified value is not present in the object	x not in y


7. Python Bitwise Operators
      Bitwise operators are used to compare (binary) numbers:
      
      Operator	      Name	                              Description	                                                                                                Example	
      & 	            AND	                              Sets each bit to 1 if both bits are 1	                                                                  x & y	
      |	            OR	                              Sets each bit to 1 if one of two bits is 1	                                                            x | y	
      ^	            XOR	                              Sets each bit to 1 if only one of two bits is 1	                                                            x ^ y	
      ~	            NOT	                              Inverts all the bits	                                                                                      ~x	
      <<	            Zero fill left shift	            Shift left by pushing zeros in from the right and let the leftmost bits fall off	                        x << 2	
      >>	            Signed right shift	            Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off	x >> 2


8. Operator Precedence
      Operator precedence describes the order in which operations are performed.
      
      Example 1:
      Parentheses has the highest precedence, meaning that expressions inside parentheses must be evaluated first:
      
            print((6 + 3) - (6 + 3))
      
            o/p: 0

      Example 2:
      Multiplication * has higher precedence than addition +, and therefor multiplications are evaluated before additions:
      
            print(100 + 5 * 3)
      
            o/p: 115

      The precedence order is described in the table below, starting with the highest precedence at the top:
      
      Operator	                                    Description	t
      ()	                                          Parentheses	
      **	                                          Exponentiation	
      +x  -x  ~x	                                    Unary plus, unary minus, and bitwise NOT	
      *  /  //  %	                                    Multiplication, division, floor division, and modulus	
      +  -	                                          Addition and subtraction	
      <<  >>	                                    Bitwise left and right shifts	
      &	                                          Bitwise AND	
      ^	                                          Bitwise XOR	
      |	                                          Bitwise OR	
      ==  !=  >  >=  <  <=  is  is not  in  not in 	Comparisons, identity, and membership operators	
      not	                                          Logical NOT	
      and	                                          AND	
      or	                                          OR


      NOTE: If two operators have the same precedence, the expression is evaluated from left to right.
      
      Example
      Addition + and subtraction - has the same precedence, and therefor we evaluate the expression from left to right:
      
            print(5 + 4 - 7 + 3)
            o/p: 5

```

## Python Lists
```
1. List
      Lists are used to store multiple items in a single variable.
      
      Lists are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary, all with different qualities and usage.
      
      Lists are created using square brackets:
      
      Example:
      Create a List:
      
            thislist = ["apple", "banana", "cherry"]
            print(thislist)

2. List Items
      List items are ordered, changeable, and allow duplicate values.
      
      List items are indexed, the first item has index [0], the second item has index [1] etc.

      a) Ordered
            When we say that lists are ordered, it means that the items have a defined order, and that order will not change.
            
            If you add new items to a list, the new items will be placed at the end of the list.
            
            Note: There are some list methods that will change the order, but in general: the order of the items will not change.
      
      b) Changeable
            The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.
      
      c) Allow Duplicates
            Since lists are indexed, lists can have items with the same value:
      
            Example
            Lists allow duplicate values:
            
            thislist = ["apple", "banana", "cherry", "apple", "cherry"]
            print(thislist)

3. List Length
      To determine how many items a list has, use the len() function:
      
      Example
      Print the number of items in the list:
      
      thislist = ["apple", "banana", "cherry"]
      print(len(thislist))

4. List Items - Data Types
      List items can be of any data type:
      
      Example
      String, int and boolean data types:
      
      list1 = ["apple", "banana", "cherry"]
      list2 = [1, 5, 7, 9, 3]
      list3 = [True, False, False]

      A list can contain different data types:
      
      Example
      A list with strings, integers and boolean values:
      
      list1 = ["abc", 34, True, 40, "male"]
      o/p: ['abc', 34, True, 40, 'male']

5. type()
      From Python's perspective, lists are defined as objects with the data type 'list':
      
      <class 'list'>
      
      Example
      What is the data type of a list?
      
      mylist = ["apple", "banana", "cherry"]
      print(type(mylist))

      o/p: <class 'list'>

6. The list() Constructor
      It is also possible to use the list() constructor when creating a new list.
      
      Example
      Using the list() constructor to make a List:
      
      thislist = list(("apple", "banana", "cherry")) # note the double round-brackets
      print(thislist)
      
      o/p: ['apple', 'banana', 'cherry']

7. Python Collections (Arrays)
      There are four collection data types in the Python programming language:
      
      List is a collection which is ordered and changeable. Allows duplicate members.
      Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
      Set is a collection which is unordered, unchangeable*, and unindexed. No duplicate members.
      Dictionary is a collection which is ordered** and changeable. No duplicate members.
      
      Note: When choosing a collection type, it is useful to understand the properties of that type. Choosing the right type for a particular data set could mean retention of meaning,          and, it could mean an increase in efficiency or security.

```

## Python - Access List Items
```
1. Access Items
      List items are indexed and you can access them by referring to the index number:
      
      Example
      Print the second item of the list:
      
      thislist = ["apple", "banana", "cherry"]
      print(thislist[1])
      Note: The first item has index 0.

2. Negative Indexing
      Negative indexing means start from the end
      
      -1 refers to the last item, -2 refers to the second last item etc.
      
      Example
      Print the last item of the list:
      
      thislist = ["apple", "banana", "cherry"]
      print(thislist[-1])

3. Range of Indexes
      You can specify a range of indexes by specifying where to start and where to end the range.
      
      When specifying a range, the return value will be a new list with the specified items.
      
      Example 1:
            Return the third, fourth, and fifth item:
            
            thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
            print(thislist[2:5])
            Note: The search will start at index 2 (included) and end at index 5 (not included).
            
            Remember that the first item has index 0.
            
            By leaving out the start value, the range will start at the first item:
            
      Example 2:
            This example returns the items from the beginning to, but NOT including, "kiwi":
            
            thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
            print(thislist[:4])
            By leaving out the end value, the range will go on to the end of the list:
      
      Example 3:
            This example returns the items from "cherry" to the end:
            
            thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
            print(thislist[2:])

4. Range of Negative Indexes
      Specify negative indexes if you want to start the search from the end of the list:
      
      Example
      This example returns the items from "orange" (-4) to, but NOT including "mango" (-1):
      
      thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
      print(thislist[-4:-1])
      
      o/p: ['orange', 'kiwi', 'melon']


5. Check if Item Exists
      To determine if a specified item is present in a list use the in keyword:
      
      Example
      Check if "apple" is present in the list:
      
      thislist = ["apple", "banana", "cherry"]
      if "apple" in thislist:
        print("Yes, 'apple' is in the fruits list")

```

## Python - Change List Items
```
1. Change Item Value
      To change the value of a specific item, refer to the index number:
      
      Example
      Change the second item:
      
      thislist = ["apple", "banana", "cherry"]
      thislist[1] = "blackcurrant"
      print(thislist)
      o/p: ['apple', 'blackcurrant', 'cherry']

2. Change a Range of Item Values
      To change the value of items within a specific range, define a list with the new values, and refer to the range of index numbers where you want to insert the new values:
      
      Example 1:
      Change the values "banana" and "cherry" with the values "blackcurrant" and "watermelon":
      
      thislist = ["apple", "banana", "cherry", "orange", "kiwi", "mango"]
      thislist[1:3] = ["blackcurrant", "watermelon"]
      print(thislist)
      If you insert more items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:

      Example 2:
      Change the second value by replacing it with two new values:
      
      thislist = ["apple", "banana", "cherry"]
      thislist[1:2] = ["blackcurrant", "watermelon"]
      print(thislist)
      Note: The length of the list will change when the number of items inserted does not match the number of items replaced.
      
      If you insert less items than you replace, the new items will be inserted where you specified, and the remaining items will move accordingly:

      Example 3:
      Change the second and third value by replacing it with one value:
      
      thislist = ["apple", "banana", "cherry"]
      thislist[1:3] = ["watermelon"]
      print(thislist)

3. Insert Items
      To insert a new list item, without replacing any of the existing values, we can use the insert() method.
      
      The insert() method inserts an item at the specified index:
      
      Example
      Insert "watermelon" as the third item:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.insert(2, "watermelon")
      print(thislist)
      o/p: ['apple', 'banana', 'watermelon', 'cherry']
```

## Python - Add List Items
```
1. Append Items
      To add an item to the end of the list, use the append() method:
      
      Example
      Using the append() method to append an item:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.append("orange")
      print(thislist)
      
2. Insert Items
      To insert a list item at a specified index, use the insert() method.
      
      The insert() method inserts an item at the specified index:
      
      Example
      Insert an item as the second position:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.insert(1, "orange")
      print(thislist)
      Note: As a result of the examples above, the lists will now contain 4 items.

3. Extend List
      To append elements from another list to the current list, use the extend() method.
      
      Example
      Add the elements of tropical to thislist:
      
      thislist = ["apple", "banana", "cherry"]
      tropical = ["mango", "pineapple", "papaya"]
      thislist.extend(tropical)
      print(thislist)
      The elements will be added to the end of the list.

4. Add Any Iterable
      The extend() method does not have to append lists, you can add any iterable object (tuples, sets, dictionaries etc.).
      
      Example
      Add elements of a tuple to a list:
      
      thislist = ["apple", "banana", "cherry"]
      thistuple = ("kiwi", "orange")
      thislist.extend(thistuple)
      print(thislist)
      o/p: ['apple', 'banana', 'cherry', 'kiwi', 'orange']
```

## Python - Remove List Items
```
1. Remove Specified Item
      The remove() method removes the specified item.
      
      Example
      Remove "banana":
      
      thislist = ["apple", "banana", "cherry"]
      thislist.remove("banana")
      print(thislist)

      If there are more than one item with the specified value, the remove() method removes the first occurance:
      
      Example
      Remove the first occurance of "banana":
      
      thislist = ["apple", "banana", "cherry", "banana", "kiwi"]
      thislist.remove("banana")
      print(thislist)

2.Remove Specified Index
      The pop() method removes the specified index.
      
      Example 1:
      Remove the second item:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.pop(1)
      print(thislist)

      If you do not specify the index, the pop() method removes the last item.
      
      Example 2;
      Remove the last item:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.pop()
      print(thislist)
      The del keyword also removes the specified index:
      
      Example 3:
      Remove the first item:
      
      thislist = ["apple", "banana", "cherry"]
      del thislist[0]
      print(thislist)
      The del keyword can also delete the list completely.
      
      Example 4:
      Delete the entire list:
      
      thislist = ["apple", "banana", "cherry"]
      del thislist

      o/p:
      Traceback (most recent call last):
        File "demo_list_del2.py", line 3, in <module>
          print(thislist) #this will cause an error because you have succsesfully deleted "thislist".
      NameError: name 'thislist' is not defined

3.Clear the List
      The clear() method empties the list.
      
      The list still remains, but it has no content.
      
      Example
      Clear the list content:
      
      thislist = ["apple", "banana", "cherry"]
      thislist.clear()
      print(thislist)

      o/p: []
      
      
```

## Python - Loop Lists
```
1. Loop Through a List
      You can loop through the list items by using a for loop:
      
      Example
      Print all items in the list, one by one:
      
      thislist = ["apple", "banana", "cherry"]
      for x in thislist:
        print(x)
      
      o/p:
      apple
      banana
      cherry

2. Loop Through the Index Numbers
      You can also loop through the list items by referring to their index number.
      
      Use the range() and len() functions to create a suitable iterable.
      
      Example
      Print all items by referring to their index number:
      
      thislist = ["apple", "banana", "cherry"]
      for i in range(len(thislist)):
        print(thislist[i])
      
      Note: The iterable created in the example above is [0, 1, 2].

3. Using a While Loop
      You can loop through the list items by using a while loop.
      
      Use the len() function to determine the length of the list, then start at 0 and loop your way through the list items by referring to their indexes.
      
      Remember to increase the index by 1 after each iteration.
      
      Example
      Print all items, using a while loop to go through all the index numbers
      
      thislist = ["apple", "banana", "cherry"]
      i = 0
      while i < len(thislist):
        print(thislist[i])
        i = i + 1

      o/p:
       apple
       banana
       cherry

4. Looping Using List Comprehension
      List Comprehension offers the shortest syntax for looping through lists:
      
      Example
      A short hand for loop that will print all items in a list:
      
      thislist = ["apple", "banana", "cherry"]
      [print(x) for x in thislist]
      
```

## Python - List Comprehension
```
1. List Comprehension
      List comprehension offers a shorter syntax when you want to create a new list based on the values of an existing list.
      
      Example:
      
      Based on a list of fruits, you want a new list, containing only the fruits with the letter "a" in the name.
      
      Without list comprehension you will have to write a for statement with a conditional test inside:
      
      Example
      fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
      newlist = []
      
      for x in fruits:
        if "a" in x:
          newlist.append(x)
      
      print(newlist)

      o/p: ['apple', 'banana', 'mango']

      With list comprehension you can do all that with only one line of code:
      
      Example
      fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
      
      newlist = [x for x in fruits if "a" in x]
      
      print(newlist)

2. The Syntax
      newlist = [expression for item in iterable if condition == True]
      The return value is a new list, leaving the old list unchanged.
      
      a) Condition
            The condition is like a filter that only accepts the items that valuate to True.
            
            Example
            Only accept items that are not "apple":
            
            newlist = [x for x in fruits if x != "apple"]
      
            The condition if x != "apple"  will return True for all elements other than "apple", making the new list contain all fruits except "apple".
            
            The condition is optional and can be omitted:
            
            Example
            With no if statement:
            
            newlist = [x for x in fruits]

      b) Iterable
            The iterable can be any iterable object, like a list, tuple, set etc.
            
            Example 1:
            You can use the range() function to create an iterable:
            
            newlist = [x for x in range(10)]
            
            Same example, but with a condition:
            
            Example 2:
            Accept only numbers lower than 5:
            
            newlist = [x for x in range(10) if x < 5]

      c) Expression
            The expression is the current item in the iteration, but it is also the outcome, which you can manipulate before it ends up like a list item in the new list:
            
            Example 1:
            Set the values in the new list to upper case:
            
            newlist = [x.upper() for x in fruits]
            o/p: ['APPLE', 'BANANA', 'CHERRY', 'KIWI', 'MANGO']
            
            You can set the outcome to whatever you like:
            
            Example 2:
            Set all values in the new list to 'hello':
            
            newlist = ['hello' for x in fruits]
            o/p: ['hello', 'hello', 'hello', 'hello', 'hello']
            
            The expression can also contain conditions, not like a filter, but as a way to manipulate the outcome:
            
            Example 3:
            Return "orange" instead of "banana":
            
            fruits = ["apple", "banana", "cherry", "kiwi", "mango"]
            newlist = [x if x != "banana" else "orange" for x in fruits]
            print(newlist)
            
            o/p:
            ['apple', 'orange', 'cherry', 'kiwi', 'mango']

```

## Python - Sort Lists
```
1. Sort List Alphanumerically
      List objects have a sort() method that will sort the list alphanumerically, ascending, by default:
      
      Example  1:
      Sort the list alphabetically:
      
      thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
      thislist.sort()
      print(thislist)

      o/p: ['banana', 'kiwi', 'mango', 'orange', 'pineapple']

      Example 2:
      Sort the list numerically:
      
      thislist = [100, 50, 65, 82, 23]
      thislist.sort()
      print(thislist)


2. Sort Descending
      To sort descending, use the keyword argument reverse = True:
      
      Example
      Sort the list descending:
      
      thislist = ["orange", "mango", "kiwi", "pineapple", "banana"]
      thislist.sort(reverse = True)
      print(thislist)
      
      
      o/p: ['pineapple', 'orange', 'mango', 'kiwi', 'banana']

3. Customize Sort Function
      You can also customize your own function by using the keyword argument key = function.
      
      The function will return a number that will be used to sort the list (the lowest number first):
      
      Example
      Sort the list based on how close the number is to 50:
      
      def myfunc(n):
        return abs(n - 50)
      
      thislist = [100, 50, 65, 82, 23]
      thislist.sort(key = myfunc)
      print(thislist)

      o/p:[50, 65, 23, 82, 100]

4. Case Insensitive Sort
      By default the sort() method is case sensitive, resulting in all capital letters being sorted before lower case letters:
      
      Example 1;
      Case sensitive sorting can give an unexpected result:
      
      thislist = ["banana", "Orange", "Kiwi", "cherry"]
      thislist.sort()
      print(thislist)
      
      o/p: ['Kiwi', 'Orange', 'banana', 'cherry']
      
      Luckily we can use built-in functions as key functions when sorting a list.
      
      So if you want a case-insensitive sort function, use str.lower as a key function:
      
      Example 2:
      Perform a case-insensitive sort of the list:
      
      thislist = ["banana", "Orange", "Kiwi", "cherry"]
      thislist.sort(key = str.lower)
      print(thislist)
      
      o/p: ['banana', 'cherry', 'Kiwi', 'Orange']

5. Reverse Order
      What if you want to reverse the order of a list, regardless of the alphabet?
      
      The reverse() method reverses the current sorting order of the elements.
      
      Example
      Reverse the order of the list items:
      
      thislist = ["banana", "Orange", "Kiwi", "cherry"]
      thislist.reverse()
      print(thislist)

```

## Python - Copy Lists
```
1. Copy a List
      You cannot copy a list simply by typing list2 = list1, because: list2 will only be a reference to list1, and changes made in list1 will automatically also be made in list2.
      
      There are ways to make a copy, one way is to use the built-in List method copy().
      
      Example 1:
      Make a copy of a list with the copy() method:
      
      thislist = ["apple", "banana", "cherry"]
      mylist = thislist.copy()
      print(mylist)
      
      Another way to make a copy is to use the built-in method list().
      
      Example 2:
      Make a copy of a list with the list() method:
      
      thislist = ["apple", "banana", "cherry"]
      mylist = list(thislist)
      print(mylist)
```

## Python - Join Lists
```
1. Join Two Lists
      There are several ways to join, or concatenate, two or more lists in Python.
      
      One of the easiest ways are by using the + operator.
      
      Example 1:
      Join two list:
      
      list1 = ["a", "b", "c"]
      list2 = [1, 2, 3]
      
      list3 = list1 + list2
      print(list3)
      
      o/p: ['a', 'b', 'c', 1, 2, 3]
      
      Another way to join two lists is by appending all the items from list2 into list1, one by one:
      
      Example 2:
      Append list2 into list1:
      
      list1 = ["a", "b" , "c"]
      list2 = [1, 2, 3]
      
      for x in list2:
        list1.append(x)
      
      print(list1)

      Or you can use the extend() method, where the purpose is to add elements from one list to another list:
      
      Example 3:
      Use the extend() method to add list2 at the end of list1:
      
      list1 = ["a", "b" , "c"]
      list2 = [1, 2, 3]
      
      list1.extend(list2)
      print(list1)

````

## Python - List Methods
```
1. List Methods
      Python has a set of built-in methods that you can use on lists.
      
      Method	Description
      append()	Adds an element at the end of the list
      clear()	Removes all the elements from the list
      copy()	Returns a copy of the list
      count()	Returns the number of elements with the specified value
      extend()	Add the elements of a list (or any iterable), to the end of the current list
      index()	Returns the index of the first element with the specified value
      insert()	Adds an element at the specified position
      pop()	Removes the element at the specified position
      remove()	Removes the item with the specified value
      reverse()	Reverses the order of the list
      sort()	Sorts the list

````

## Python Tuples
```
mytuple = ("apple", "banana", "cherry")

1. Tuple
      Tuples are used to store multiple items in a single variable.
      
      Tuple is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Set, and Dictionary, all with different qualities and usage.
      
      A tuple is a collection which is ordered and unchangeable.
      
      Tuples are written with round brackets.
      
      ExampleGet your own Python Server
      Create a Tuple:
      
      thistuple = ("apple", "banana", "cherry")
      print(thistuple)

2. Tuple Items
      Tuple items are ordered, unchangeable, and allow duplicate values.
      
      Tuple items are indexed, the first item has index [0], the second item has index [1] etc.

3. Ordered
      When we say that tuples are ordered, it means that the items have a defined order, and that order will not change.

4. Unchangeable
      Tuples are unchangeable, meaning that we cannot change, add or remove items after the tuple has been created.

5. Allow Duplicates
      Since tuples are indexed, they can have items with the same value:

      Example
      Tuples allow duplicate values:
      
      thistuple = ("apple", "banana", "cherry", "apple", "cherry")
      print(thistuple)

6.Tuple Length
      To determine how many items a tuple has, use the len() function:
      
      Example
      Print the number of items in the tuple:
      
      thistuple = ("apple", "banana", "cherry")
      print(len(thistuple))

7.Create Tuple With One Item
      To create a tuple with only one item, you have to add a comma after the item, otherwise Python will not recognize it as a tuple.
      
      Example
      One item tuple, remember the comma:
      
      thistuple = ("apple",)
      print(type(thistuple))
      
      #NOT a tuple
      thistuple = ("apple")
      print(type(thistuple))

      o/p:
      <class 'tuple'>
      <class 'str'>

8. Tuple Items - Data Types
      Tuple items can be of any data type:
      
      Example
      String, int and boolean data types:
      
      tuple1 = ("apple", "banana", "cherry")
      tuple2 = (1, 5, 7, 9, 3)
      tuple3 = (True, False, False)
      print(tuple1)
      print(tuple2)
      print(tuple3)
      
      A tuple can contain different data types:
      
      Example
      A tuple with strings, integers and boolean values:
      
      tuple1 = ("abc", 34, True, 40, "male")
      o/p: ('abc', 34, True, 40, 'male')
      
9. type()
      From Python's perspective, tuples are defined as objects with the data type 'tuple':
      
      <class 'tuple'>
      Example
      What is the data type of a tuple?
      
      mytuple = ("apple", "banana", "cherry")
      print(type(mytuple))
      
      o/p: <class 'tuple'>

10. The tuple() Constructor
      It is also possible to use the tuple() constructor to make a tuple.
      
      Example
      Using the tuple() method to make a tuple:
      
      thistuple = tuple(("apple", "banana", "cherry")) # note the double round-brackets
      print(thistuple)

11. Python Collections (Arrays)
      There are four collection data types in the Python programming language:
      
      List is a collection which is ordered and changeable. Allows duplicate members.
      Tuple is a collection which is ordered and unchangeable. Allows duplicate members.
      Set is a collection which is unordered, unchangeable*, and unindexed. No duplicate members.
      Dictionary is a collection which is ordered** and changeable. No duplicate members.
```







