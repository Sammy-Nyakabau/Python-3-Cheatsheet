![Python Logo](https://i.ibb.co/VMcNQpQ/Python-logo.png)

# :computer: Python-3-Cheatsheet :snake:
Code snippets which detail the fundamental syntax and concepts introduced in [Python 3](https://docs.python.org/3/contents.html)


## Table of Contents

1. [Introduction](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#introduction)
2. [Variables](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#variables)
3. [Strings](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#strings)
4. [Type Conversion](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#type-conversion)
5. [Falsy Values](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#falsy-values)
6. [Conditional Statements](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#conditional-statements)
7. [Loops](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#loops)
8. [Functions](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#functions)
9. [Lists](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#lists)
10. [Tuples](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#tuples)
11. [Arrays](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#arrays)
12. [Sets](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#sets)
13. [Dictionaries](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#dictionaries)
14. [Generator Expressions](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#generator-expressions)
15. [Unpacking Operator](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#unpacking-operator)
16. [Exceptions](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#exceptions)
17. [Classes](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#classes)

---

### Introduction

>Python is a general-purpose interpreted, interactive, object-oriented, and high-level programming language. It was created by Guido van Rossum during 1985- 1990. Like Perl, Python source code is also available under the GNU General Public License (GPL). Python is named after a TV Show called ëMonty Pythonís Flying Circusí and not after Python-the snake.

>Python 3.0 was released in 2008. Although this version is supposed to be backward incompatibles, later on many of its important features have been backported to be compatible with version 2.7. This cheatsheet gives enough understanding on Python 3 version programming language.
---

### Variables :pushpin:

- Variables are nothing but reserved memory locations to store values. It means that when you create a variable, you reserve some space in the memory.
- Based on the data type of a variable, the interpreter allocates memory and decides what can be stored in the reserved memory. Therefore, by assigning different data types to the variables, you can store integers, decimals or characters in these variables.

```python
a = 1       # integer
b = 1.1     # float
c = 1 + 2j  # complex number (a + bi)
d = “a”     # string
e = True    # boolean (True / False)
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---
### Strings :pushpin:

- Strings are amongst the most popular types in Python. We can create them simply by enclosing characters in quotes. Python treats single quotes the same as double quotes.

```python
x = “Python”
len(x)
x[0]
x[-1]
x[0:3]
 
# Formatted strings
name = f”{first} {last}”
 
# Escape sequences
\” \’ \\ \n
 
# String methods
x.upper()
x.lower()
x.title()
x.strip()
x.find(“p”)
x.replace(“a”, “b”)
“a” in x
```
---
### Type Conversion :pushpin:

- Sometimes, you may need to perform conversions between the built-in types. To convert between types, you simply use the type-names as a function.

- There are several built-in functions to perform conversion from one data type to another. These functions return a new object representing the converted value.

```python
int(x)  
float(x) 
bool(x) 
string(x)
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---
### Falsy Values :pushpin:

- A falsy (sometimes written falsey) value is a value that is considered false when encountered in a Boolean context.

```python
0
“”
[]
()
{}
set()
range(0)
None
False
```
---
### Conditional Statements :pushpin:

- Decision-making is the anticipation of conditions occurring during the execution of a program and specified actions taken according to the conditions.
- Decision structures evaluate multiple expressions, which produce TRUE or FALSE as the outcome. You need to determine which action to take and which statements to execute if the outcome is TRUE or FALSE otherwise.
- Python programming language assumes any **non-zero** and **non-null** values as TRUE, and any **zero** or **null** values as FALSE value

```python
if x == 1:  
    print(“a”)
elif x == 2:  
    print(“b”)
else:   
    print(“c”)
 
# Ternary operator 
x = “a” if n > 1 else “b”
 
# Chaining comparison operators
if 18 <= age < 65:
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---
### Loops :pushpin:

- In general, statements are executed sequentially − The first statement in a function is executed first, followed by the second, and so on. There may be a situation when you need to execute a block of code several number of times.
- Programming languages provide various control structures that allow more complicated execution paths.
- A loop statement allows us to execute a statement or group of statements multiple times. 

```python
for n in range(1, 10): 
    print(n)
 
while n < 10: 
    print(n)
    n += 1
```
---
### Functions :pushpin:

- A function is a block of organized, reusable code that is used to perform a single, related action. Functions provide better modularity for your application and a high degree of code reusing.
- As you already know, Python gives you many built-in functions like print(), etc. but you can also create your own functions. These functions are called user-defined functions.

```python
def increment(number, by=1):   
    return number + by
 
# Keyword arguments 
increment(2, by=1)
 
# Variable number of arguments 
def multiply(*numbers): 
    for number in numbers: 
        print number 
 
 
multiply(1, 2, 3, 4)
 
# Variable number of keyword arguments 
def save_user(**user):  
    ...
 
 
save_user(id=1, name="Sam")
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---

### Lists :pushpin:

- The most basic data structure in Python is the sequence. Each element of a sequence is assigned a number - its position or index. The first index is zero, the second index is one, and so forth.
- There are certain things you can do with all the sequence types. These operations include indexing, slicing, adding, multiplying, and checking for membership. In addition, Python has built-in functions for finding the length of a sequence and for finding its largest and smallest elements.
- The list is the most versatile datatype available in Python, which can be written as a list of comma-separated values (items) between square brackets. Important thing about a list is that the items in a list need not be of the same type

```python
# Creating lists
letters = ["a", "b", "c"]     
matrix = [[0, 1], [1, 2]]
zeros = [0] * 5
combined = zeros + letters
numbers = list(range(20))
 
# Accessing items
letters = ["a", "b", "c", "d"]
letters[0]  # "a"
letters[-1] # "d"
 
# Slicing lists 
letters[0:3]   # "a", "b", "c"
letters[:3]    # "a", "b", "c"
letters[0:]    # "a", "b", "c", "d"
letters[:]     # "a", "b", "c", "d"
letters[::2]   # "a", "c"
letters[::-1]  # "d", "c", "b", "a" 
 
# Unpacking 
first, second, *other = letters 
 
# Looping over lists 
for letter in letters: 
    ... 
 
for index, letter in enumerate(letters): 
    ... 
 
# Adding items 
letters.append("e")
letters.insert(0, "-")
 
# Removing items 
letters.pop()
letters.pop(0)
letters.remove("b")
del letters[0:3]
 
# Finding items 
if "f" in letters: 
    letters.index("f")
 
# Sorting lists 
letters.sort()
letters.sort(reverse=True) 
 
# Custom sorting 
items = [
    ("Product1", 10),
    ("Product2", 9),
    ("Product3", 11)
]
 
items.sort(key=lambda item: item[1])
 
# Map and filter 
prices = list(map(lambda item: item[1], items))
expensive_items = list(filter(lambda item: item[1] >= 10, items))
 
# List comprehensions 
prices = [item[1] for item in items]
expensive_items = [item for item in items if item[1] >= 10]
 
# Zip function 
list1 = [1, 2, 3]
list2 = [10, 20, 30]
combined = list(zip(list1, list2))    # [(1, 10), (2, 20)...]
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---

### Tuples :pushpin:
- A tuple is a collection of objects which ordered and immutable. Tuples are sequences, just like lists. The main difference between the tuples and the lists is that the tuples cannot be changed unlike lists. Tuples use parentheses, whereas lists use square brackets.
- Creating a tuple is as simple as putting different comma-separated values. Optionally, you can put these comma-separated values between parentheses also.

```python
point = (1, 2, 3)
point(0:2)     # (1, 2)
x, y, z = point 
if 10 in point: 
    ... 
 
# Swapping variables 
x = 10
y = 11
x, y = y, x 
```
---
### Arrays :pushpin:

- Array is a container which can hold a fix number of items and these items should be of the same type. Most of the data structures make use of arrays to implement their algorithms.

```python
from array import *

arrayName = array(typecode, [Initializers])

# Typecode are the codes that are used to define the type of value the array will hold.

# Example
from array import array 
 
numbers = array("i", [1, 2, 3])
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---

### Sets :pushpin:

- Mathematically, a set is a collection of items not in any particular order. A Python set is similar to this mathematical definition with below additional conditions.
    - The elements in the set cannot be duplicates.
    - The elements in the set are immutable(cannot be modified) but the set as a whole is mutable.
    - There is no index attached to any element in a python set. So they do not support any indexing or slicing operation.

```python
first = {1, 2, 3, 4}
second = {1, 5}
 
first | second  # {1, 2, 3, 4, 5}
first & second  # {1}
first - second  # {2, 3, 4}
first ^ second  # {2, 3, 4, 5}
 
if 1 in first: 
    ... 
```
---

### Dictionaries :pushpin:

- Each key is separated from its value by a colon `:`, the items are separated by commas, and the whole thing is enclosed in curly braces. An empty dictionary without any items is written with just two curly braces, like this: `{}`.
- Keys are unique within a dictionary while values may not be. The values of a dictionary can be of any type, but the keys must be of an immutable data type such as strings, numbers, or tuples.

```python
point = {"x": 1, "y": 2}
point = dict(x=1, y=2)
point["z"] = 3
if "a" in point: 
    ... 
point.get("a", 0)   # 0
del point["x"]
for key, value in point.items(): 
   ... 
 
# Dictionary comprehensions 
values = {x: x * 2 for x in range(5)}
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---

### Generator Expressions :pushpin:

- Generators in python are a special routine that can be used to control the iteration behaviour of a loop. A generator is similar to a function returning an array. A generator has parameter, which we can call and it generates a sequence of numbers. But unlike functions, which return a whole array, a generator yields one value at a time which requires less memory.
- There are various other expressions that can be simply coded similar to list comprehensions but instead of brackets we use parenthesis. These expressions are designed for situations where the generator is used right away by an enclosing function. Generator expression allows creating a generator without a yield keyword. However, it doesn’t share the whole power of generator created with a yield function

```python
values = (x * 2 for x in range(10000))
len(values)  # Error
for x in values:
    print(x)
```
---

### Unpacking Operator :pushpin:

- We use two operators `*` (for tuples) and `**` (for dictionaries)
- We can use `*` or `**` to unpack the list so that all elements of it can be passed as sinlge elements in the combined list/dictionary.

```python
first = [1, 2, 3]
second = [4, 5, 6]
combined = [*first, "a", *second]
 
first = {"x": 1}
second = {"y": 2}
combined = {**first, **second}
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---

### Exceptions :pushpin:

- Python has many built-in exceptions that are raised when your program encounters an error (something in the program goes wrong).
- When these exceptions occur, the Python interpreter stops the current process and passes it to the calling process until it is handled. If not handled, the program will crash.

```python
# Handling Exceptions 
try: 
  …
except (ValueError, ZeroDivisionError):
  …
else: 
  # no exceptions raised
finally:
  # cleanup code 
 
# Raising exceptions 
if x < 1:     
    raise ValueError(“…”)
 
# The with statement 
with open(“file.txt”) as file
```

---

### Classes :pushpin:

- Python has been an object-oriented language since the time it existed. Due to this, creating and using classes and objects are downright easy.

```python
# Creating classes
class Point: 
    def __init__(self, x, y):         
        self.x = x
        self.y = y 
 
    def draw(self):         
        …
 
# Instance vs class attributes
class Point: 
    default_color = “red”
 
    def __init__(self, x, y):         
        self.x = x
 
# Instance vs class methods
class Point: 
    def draw(self):        
        …
     
    @classmethod
    def zero(cls):         
        return cls(0, 0)
 
 
# Magic methods
__str__()
__eq__()
__cmp__()
... 
 
# Private members 
class Point: 
    def __init__(self, x):         
        self.__x = x
 
 
# Properties 
class Point: 
    def __init__(self, x):         
        self.__x = x
 
    @property
    def x(self):    
        return self.__x     
 
    @property.setter:
    def x.setter(self, value): 
        self.__x = value 
 
# Inheritance
class FileStream(Stream): 
    def open(self):        
         super().open()
         … 
 
# Multiple inheritance 
class FlyingFish(Flyer, Swimmer): 
    … 
 
# Abstract base classes
from abc import ABC, abstractmethod
 
class Stream(ABC): 
    @abstractmethod
    def read(self): 
        pass 
 
# Named tuples 
from collections import namedtuple
 
Point = namedtuple(“Point”, [“x”, “y”])
point = Point(x=1, y=2)
```
##### **[Back To Top :arrow_up:](https://github.com/Sammy-Nyakabau/Python-3-Cheatsheet#table-of-contents)**
---
