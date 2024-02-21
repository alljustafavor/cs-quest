Variables and Data Types

Variables are containers for storing data values.

Creating Variables: Python has no command for declaring a variable. A variable is created the moment you first assign a value to it.

```python
  x = 5      # output: 5
  y = "John" # output: "John"
```
variavles so not need to be declared with any type, and can even change type after they have been set.

```python
  x = 5      # x: int
  x = "John" # x: str
```

Casting: if you want to specify the data type of a variable, this can be done with casting.

```python
  x = str(3)   # output: '3'
  y = int(3)   # output: 3
  z = float(3) # output: 3.0
```

Assign multiple values: Python allows you to assign values to multiple variables in one line.



Data Types
In programming, data type is an important concept.
Variables can store data of different types, and different types can do different things.
Python has the following data types built-in by default, in these vategories:

* Text Type:	str
* Numeric Types:	int, float, complex
* Sequence Types:	list, tuple, range
* Mapping Type:	dict
* Set Types:	set, frozenset
* Boolean Type:	bool
* Binary Types:	bytes, bytearray, memoryview
* None Type:	NoneType

```python
x = "Hello World"                            # type: str
x = 20                                       # type: int
x = 20.5                                     # type: float
x = 1j                                       # type: complex
x = ["apple", "banana", "cherry"]            # type: list
x = ("apple", "banana", "cherry")            # type: tuple
x = range(6)                                 # type: range
x = {"name" : "John", "age" : 36}            # type: dict
x = {"apple", "banana", "cherry"}            # type: set
x = frozenset({"apple", "banana", "cherry"}) # type: int
x = True                                     # type: bool
x = b"Hello"                                 # type: bytes
x = bytearray(5)                             # type: bytearray
x = memoryview(bytes(5))                     # type: memoryview
x = none                                     # type: NoneType 
```
Setting the Specific Data Type:

```python
x = str("Hello World")	                      # type: str
x = int(20)	                                  # type: int
x = float(20.5)	                              # type: float
x = complex(1j)	                              # type: complex
x = list(("apple", "banana", "cherry"))	      # type: list
x = tuple(("apple", "banana", "cherry"))	    # type: tuple
x = range(6)	                                # type: range
x = dict(name="John", age=36)	                # type: dict
x = set(("apple", "banana", "cherry"))	      # type: set
x = frozenset(("apple", "banana", "cherry"))  # type: frozenset
x = bool(5)	                                  # type: bool
x = bytes(5)	                                # type: bytes
x = bytearray(5)	                            # type: bytearray
x = memoryview(bytes(5))	                    # type: memoryview
```

# Numbers

There are three numeric types in Python:
*  Int: Int, or interger, is a whole number, positive or negitive, without, decimals, of unlimited length.
*  Float: Float, or "floating point number" is a number, positive or negative, containing one or more decimals.
*  Complex: Complex numbers are written with a "j" as the imaginary part

## Type Conversion
  You can convery from one type to another with the int(), float(), and complex() methods

## Random Number
  Python does not have a random() function to make a random number, but Python has a built-in module called random that can be used to make random numbers.
  ```python
  import random
  print(random.randrange(1, 10)) # output: a random number between 1 and 9
  ```
# Strings

Strings in python are surrounded by either  single quotation makes, or double quotation marks.

### Strings are arrays
Like many other languages, strings in Python are arrays of bytes representing unicode.

## Slicing Stringd
You can return a range of characters using the slice syntax.

```python
b = "Hello, World!"
print(b[2:5]) # output: "llo"
```
  ### Slice From the Start
  By leaving out the start index, the range will start at the first character:

  ```python
    b = "Hello, World!"
    print(b[:5]) # output: "Hello"
  ```
 ### Slice To the End
 By leaving out the end index, the range will go to hte end:

 ```python
    b = "Hello, World!"
    print(b[2:]) # output: "llo, World!"
  ```
 ### Negative Indexing
 Use negative indexes to start the slice from the end of the string

 ex desc:
 * Get the characters:
 * From "o" in "World!" (position -5) To, but not included "d" in "World!" (position -2):

  ```python
    b = "Hello, World!"
    print(b[-5:-2]) # output: "orl"
  ```
## Modify Strings
Python has a set of built-in methods that you can use on strings.

  ### Upper Case



