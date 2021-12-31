# Python Basics
Most of these notes are built in Jupyter Notebook. So let's do a quick review of how to install Jupyter Notebook first. 

Jupyter Notebook is an open source web application that allows us to create and share code and documents. It is an interactive computing environment, which allows users to experiment with code and share it.

![jupyter](https://miro.medium.com/max/756/0*AqFDoe9TNQQLmrl1.png)

Take a close look from their web page: [https://jupyter.org/](https://jupyter.org/)

Jupyter is the acronym for Julia, Python and R, the three programming languages Jupyter started with, although today it supports a large number of languages.
It is widely used to create and share documents containing code. This is very useful in teaching, since we can show with examples how a script, a language works or ask students to propose and validate their own code.

## Advantages of using Jupyter Notebook

Provides an environment where you can log code, execute code, view results, visualize data, and view output results. These features make it a convenient tool for performing end-to-end data science workflows, which can be used for data cleansing, statistical modeling, creating and training machine learning models, data visualization, and many other purposes. When you are still prototyping a project, Jupyter Notebooks is really useful, because your code is written in a separate unit and runs separately. This allows users to test specific code blocks in the project without having to run the code from the beginning of the script. Jupyter Notebook is a web application that facilitates the creation and sharing of literary program documents. It supports real-time code, mathematical equations, visualization and Markdown. Its uses include data cleaning and conversion, numerical simulation, statistical modeling and machines. Studying and so on. Currently, the data in Kaggle, the most popular data mining competition, is in Jupyter format. For machine learning beginners, learning to use Jupyter Notebook is very important.

## Jupyter Notebook vs Jupyter Lab

Jupyter Notebook is an interactive web-based computational environment for creating Jupyter notebook documents. It supports several languages such as Python (IPython), Julia, R, etc. and is mainly used for data analysis, data visualization and more interactive exploratory computing. JupyterLab is the next generation user interface including laptops. It has a modular structure, where you can open multiple notebooks or files (e.g. HTML, text, Markdowns, etc.) as tabs in the same window. It offers a more IDE-like experience. For a beginner, it is advisable to start with Jupyter Notebook, as it only consists of a file explorer and an editor (notebook) view. It might be easier to use. If you want more features, switch to JupyterLab. JupyterLab offers many more features and an improved interface, which can be extended through extensions.

To install Jupyter Notebook, please keep forward the next link: [https://docs.jupyter.org/en/latest/install/notebook-classic.html](https://docs.jupyter.org/en/latest/install/notebook-classic.html)

Once JupyterLab is installed in our computer we can make use of it and exploit all the possibilities to write code and visualize at the same time what we are doing. It is a good starting point. Usually what I do is that I start writing code in JupyterLab and then, if necessary, I convert this notebook into a Python executable for speed and versatility.

In data science, usually, we use libraries or write code to download, extract, consolidate, organize, optimize, analyze and visualize data and data manipulation results.  Let's start then with some basic notions and syntax of how to use Python for our purposes and also in general tasks. Python provides a good foundation for all our data science tasks.

**_Let's do it!_**

## What is Python?

Python is a popular programming language. It was created by Guido van Rossum, and released in 1991.

It is used for:
- web development (server-side),
- software development,
- mathematics,
- system scripting.

## What can Python do?
- Python can be used on a server to create web applications.
- Python can be used alongside software to create workflows.
- Python can connect to database systems. It can also read and modify files.
- Python can be used to handle big data and perform complex mathematics.
- Python can be used for rapid prototyping, or for production-ready software development.

## Why Python?
- Python works on different platforms (Windows, Mac, Linux, Raspberry Pi, etc).
- Python has a simple syntax similar to the English language.
- Python has syntax that allows developers to write programs with fewer lines than some other programming languages.
- Python runs on an interpreter system, meaning that code can be executed as soon as it is written. This means that prototyping can be very quick.
- Python can be treated in a procedural way, an object-oriented way or a functional way.


Python syntax can be executed by writing directly in the Command Line:


```python
## Example: Try out yourself your first task, print "Hello, World!"
print("Hello, World!")
```

    Hello, World!


## Creating a Comment
Comments starts with a #, and Python will ignore them: 


```python
#This is a comment
print("Hello, World!")
```

    Hello, World!


Comments can be placed at the end of a line, and Python will ignore the rest of the line:


```python
print("Hello, World!") #This is a comment
```

    Hello, World!


A comment does not have to be text that explains the code, it can also be used to prevent Python from executing code:


```python
#print("Hello, World!")
print("Cheers, Beer!") 
```

    Cheers, Beer!


### Multi Line Comments

Python does not really have a syntax for multi line comments.

To add a multiline comment you could insert a # for each line:


```python
#This is a comment
#written in
#more than just one line
print("Hello, World!")
```

    Hello, World!


Or, not quite as intended, you can use a multiline string.

Since Python will ignore string literals that are not assigned to a variable, you can add a multiline string (triple quotes) in your code, and place your comment inside it:


```python
"""
This is a comment written in more than just one line
"""
print("Hello, World!") 
```

    Hello, World!


## Python Variables
Variables are containers for storing data values.

### Creating Variables
Python has no command for declaring a variable. A variable is created the moment you first assign a value to it.


```python
x = 562
y = "David"
print(x)
print(y)
```

    562
    David


Variables do not need to be declared with any particular type, and can even change type after they have been set.


```python
x = 3467       # x is of type int
x = "Sierra" # x is now of type str
print(x)
```

    Sierra


If you want to specify the data type of a variable, this can be done with casting.


```python
x = str(3465)    # x will be '3'
y = int(8783)    # y will be 3
z = float(3389)  # z will be 3.0 
print("x =",x, "y =",y, "z =",z)
```

    x = 3465 y = 8783 z = 3389.0


Or, you could directly print the variable trought the name without the command "print"


```python
x
```




    '3465'



- Many Values to Multiple Variables: Python allows you to assign values to multiple variables in one line:
    - Note: Make sure the number of variables matches the number of values, or else you will get an error.
- One Value to Multiple Variables: And you can assign the same value to multiple variables in one line.
- Unpack a Collection: If you have a collection of values in a list, tuple etc. Python allows you extract the values into variables. This is called unpacking.


```python
# Example 1
x1, y1, z1 = "Orange", "Banana", "Cherry"
print("x1 =",x1)
print("z1 =",y1)
print("z1 =",z1)

# Example 2
x2 = y2 = z2 = "Orange"
print("x2 =",x2)
print("y2 =",y2)
print("z2 =",z2)

# Example 3
fruits = ["apple", "banana", "cherry"]
x3, y3, z3 = fruits
print("x3 =",x3)
print("y3 =",y3)
print("z3 =",z3)
```

    x1 = Orange
    z1 = Banana
    z1 = Cherry
    x2 = Orange
    y2 = Orange
    z2 = Orange
    x3 = apple
    y3 = banana
    z3 = cherry


- You can also use the + character to add a variable to another variable.
- For numbers, the + character works as a mathematical operator.
- If you try to combine a string and a number, Python will give you an error.


```python
#Example
x = "Python is "
y = "awesome"
z =  x + y
print(z)
```

    Python is awesome



```python
#Example
x = 5
y = 10
print(x + y)
```

    15



```python
#Example
x = 5
y = "John"
print(x + y)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-14-6c53d93dc73b> in <module>
          2 x = 5
          3 y = "John"
    ----> 4 print(x + y)
    

    TypeError: unsupported operand type(s) for +: 'int' and 'str'


## Built-in Data Types

In programming, data type is an important concept. Variables can store data of different types, and different types can do different things. Python has the following data types built-in by default, in these categories:
- Text Type: |str
- Numeric Types: |int, float, complex
- Sequence Types: |list, tuple, range
- Mapping Type: |dict
- Set Types: |set, frozenset
- Boolean Type: |bool
- Binary Types: |bytes, bytearray, memoryview

You can get the data type of any object by using the type() function:


```python
#Example
x1, y1, z1, u1, v1, w1, t1 = 583783, 0.0776, 4j+2, "Some thing", ["one", "two", "three"], ("one", "two", "three"), {"one", "two", "three"}
x2, y2, z2, u2, v2, w2, t2 = True, False, dict(name="David", age=43), {"David":43}, bytearray(5), memoryview(bytes(5)), int(20.5)
for i in [x1, y1, z1, u1, w1, t1]:
    print("Variable", i, "is type", type(i))
print("---------------")
for j in [x2, y2, z2, u2, v2, w2, t2]:
    print("Variable", j, "is type", type(j))
```

    Variable 583783 is type <class 'int'>
    Variable 0.0776 is type <class 'float'>
    Variable (2+4j) is type <class 'complex'>
    Variable Some thing is type <class 'str'>
    Variable ('one', 'two', 'three') is type <class 'tuple'>
    Variable {'one', 'two', 'three'} is type <class 'set'>
    ---------------
    Variable True is type <class 'bool'>
    Variable False is type <class 'bool'>
    Variable {'name': 'David', 'age': 43} is type <class 'dict'>
    Variable {'David': 43} is type <class 'dict'>
    Variable bytearray(b'\x00\x00\x00\x00\x00') is type <class 'bytearray'>
    Variable <memory at 0x7f64531d4b80> is type <class 'memoryview'>
    Variable 20 is type <class 'int'>


## Boolean Values

In programming you often need to know if an expression is True or False. You can evaluate any expression in Python, and get one of two answers, True or False. When you compare two values, the expression is evaluated and Python returns the Boolean answer.


```python
#Example
print("10 > 9:", 10 > 9)
print("10 == 9:", 10 == 9)
print("10 < 9:", 10 < 9) 
u, v, w, x = "one", "two", "three", "Three"
print("one == two:", u == v) 
print("three == three:", w == w) 
print("three == Three:", w == x) 
```

    10 > 9: True
    10 == 9: False
    10 < 9: False
    one == two: False
    three == three: True
    three == Three: False


# Python Arithmetic Operators

- Arithmetic operators are used with numeric values to perform common mathematical operations:

| Operator | Name | Example || Operator | Name | Example | 
| --- | --- | --- || --- | --- | --- |
| + | Addition | x + y || - | Subtraction | x - y |
| * | Multiplication | x * y || / | Division | x / y |
| ** | Exponentiation | x ** y || // | Floor division | x // y |
| % | Modulus | x % y |

- Python Assignment Operators. Assignment operators are used to assign values to variables:

| Operator | Example | Same As || Operator | Example | Same As |
| --- | --- | --- || --- | --- | --- |
| = | x = 5 | x = 5 || += | x += 3 | x = x + 3 |
| -= | x -= 3 | x = x - 3 || *= | x *= 3 | x = x * 3 |
| /= | x /= 3 | x = x / 3 || %= | x %= 3 | x = x % 3 |
| //= | x //= 3 | x = x // 3 || **= | x **= 3 | x = x ** 3 |
| &= | x &= 3 | x = x & 3 || \|= | x \|= 3 | x = x \| 3 |
| ^= | x ^= 3 | x = x ^ 3 || >>= | x >>= 3 | x = x >> 3 |
| <<= | x <<= 3 | x = x << 3 |

- Python Comparison Operators. Comparison operators are used to compare two values.

| Operator | Name | Example |
| --- | --- | --- |
| == |Equal | x == y |
| != |Not equal | x != y |
| > |Greater than | x > y |
| < |Less than | x < y |
| >= |Greater than or equal to | x >= y |
| <= |Less than or equal to | x <= y |

- Python Logical Operators. Logical operators are used to combine conditional statements. 

| Operator | Description | Example |
| --- | --- | --- |
| and  | Returns True if both statements are true | x < 5 and  x < 10 |
| or | Returns True if one of the statements is true | x < 5 or x < 4 |
| not | Reverse the result, returns False if the result is true | not(x < 5 and x < 10) |

- Python Identity Operators. Identity operators are used to compare the objects, not if they are equal, but if they are actually the same object, with the same memory location.

| Operator | Description | Example |
| --- | --- | --- |
| is  | Returns True if both variables are the same object | x is y |
| is not | Returns True if both variables are not the same object | x is not y |

- Python Membership Operators. Membership operators are used to test if a sequence is presented in an object.

| Operator | Description | Example |
| --- | --- | --- |
| in  | Returns True if a sequence with the specified value is present in the object | x in y |
| not in | Returns True if a sequence with the specified value is not present in the object | x not in y |

- Python Bitwise Operators. Bitwise operators are used to compare (binary) numbers.

| Operator | Name | Description |
| --- | --- | --- |
| &  | AND | Sets each bit to 1 if both bits are 1 |
| \| | OR | Sets each bit to 1 if one of two bits is 1 |
| ^ | XOR | Sets each bit to 1 if only one of two bits is 1 |
| ~  | NOT | Inverts all the bits |
| << | Zero fill left shift | Shift left by pushing zeros in from the right and let the leftmost bits fall off |
| >> | Signed right shift | Shift right by pushing copies of the leftmost bit in from the left, and let the rightmost bits fall off |


```python
#Example

```
