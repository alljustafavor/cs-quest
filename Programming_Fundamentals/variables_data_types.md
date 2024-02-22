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
  Python does not have a ```random()``` function to make a random number, but Python has a built-in module called random that can be used to make random numbers.
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
  The ```upper()``` method returns the string in upper case:
  ```python
    a = "Hello, World!"
    print(a.upper()) # output: "HELLO, WORLD!"
  ```
  ### Lower Case
  The ```lower()``` method returns the string in lower case.
  ```python
    a = "Hello, World!"
    print(a.lower()) # output: "hello, world!"
  ```
  ### Remove Whitespace
  * Whitespace is the space before or after the actual text, and very often you want to remove this space.
  * The ```strip()``` method removes any whitespace from beginning or end:
  ```python
    a = " Hello, World! "
    print(a.strip()) # output: "Hello, World!"
  ```
  ### Replace String
  The ```replace()``` method replaces a string with another string:
  ```python
    a = "Hello, World!"
    print(a.replace("H", "J")) # output: "Jello, World!"
  ```
  ### Split String
  * The ```split()``` method returns a list where the text between the specified separator become the list items.
  * The ```split()``` method splits the string into substring if it finds instances of the separator:
  ```python
    a = "Hello, World!"
    print(a.split(",")) # output: ['Hello', ' World!']
  ```
  
## Format Strings

* We cannot combine string and numbers.
* But We can combine strings and numbers using the ```format()``` method.
* The ```format()``` method takes the passed arguments, formats them, and places them in the string where the placeholders {}.
  ```python
    age = 36
    txt = "My name is John, and I am {}"
  ```
* The ```format()``` method takes unlimited number of arguments, and are placed into the respective placeholders:
  ```python
    quantity = 3
    itemno = 567
    price = 49.95
    myorder = "I want {} pieces of item {} for {} dollars."
  ```
* Use can use the index numbers {0} to be sure the arguments are placed in the correct placeholders:
  ```python
    quantity = 3
    itemno = 567
    price = 49.95
    myorder = "I want to pay {2} dollars for {0} pieces of item {1}."
  ```

## Escape Characters
* To insert characters that are illegal in string, use an escape character.
* An escape character is a backslash \ followed by the charactr you want to insert.
* An example of an illegal  character is a double quote inside a string that is surrounded by double qoutes.
* \'	Single Quote	
* \\	Backslash	
* \n	New Line	
* \r	Carriage Return	
* \t	Tab	
* \b	Backspace	
* \f	Form Feed	
* \ooo	Octal value	
* \xhh	Hex value

## String Methods

* ```capitalize()```
  * The ```capitalize()``` method return a str where its first charcter is upper case, and the rest is lower case.
* ```casefold()```
  * The ```casefold()``` method returns a string where all the characters are lower case.
  * This method is similar to the ```lower()``` method, but the ```casefold()``` method is stronger, more aggressive, meaning that it will xonvert more characters into lower case, and will find more matches when comparing two strings and both are converted are converted using the ```casefold()```
* ```center()```
* ```count()```
  * The ```count(value, start=0, end=len(str)``` method returns the number of times a specifed value appers in the string:
    ```python
      txt = "I love apples, apple are my favorite fruit"
      x = txt.count("apple") # output: 2
    ```
* ```encode()```
* ```endswith()```
  * The ```endswith(value, start, end)``` method returns True id the string ends with the specified value, otherwises False:
    ```python
      txt = "Hello, welcome to my world."
      x = txt.endswith(".") # output: True
    ```
* ```expandtabs()```
* ```find()```
  * The ```find()``` method finds the first occurrence of the specified value.
  * The ```find()``` method return ```-1``` if the value is not found.
  * The ```find()``` method is almost the same as the ```index()``` method, the only difference is that index() method raises an exception if the value is not found.
    ```python
      txt = "Hello, welcome to my world."
      x = txt.find("welcome") # output: 7
    ```
* ```format()```
* ```format_map()```
* ```index()```
* ```isalnum()```
* ```isalpha()```
* ```isascii()```
* ```isdecimal()```
* ```isdigit()```
* ```isidentifier()```
* ```islower()```
* ```isnumeric()```
* ```issapce()```
* ```istitle()```
* ```issupper()```
* ```join()```
* ```ljust()```
* ```lower()```
* ```lstrip()```
* ```maketrans()```
* ```partition()```
* ```replace()```
* ```rfind()```
* ```rindex()```
* ```rjust()```
* ```rpartition()```
* ```rsplit()```
* ```rstrip()```
* ```split()```
* ```splitlines()```
* ```startswith()```
* ```strip()```
* ```swapcase()```
* ```title()```
* ```translate()```
* ```upper()```
* ```zfill()```

# Lists

```python
my_list = ["apple", "banana", "cherry"]
```

## List
* List are used to store multiple items in a single variable.
* Lisrs are one of 4 built-in data types in Python used to store collections of data, the other 3 are Tuple, Set, and Dictionary.

## List Items
* List items are ordered, changeable, and allow dulicate values.
* List items are indexed, the first item has index ```[0]```

## Ordered 
* When we say that lists are ordered, it means that the items have a defined order, and that order will not change.
* If you add new items to the list, the new items will be placed at the end of the list.
* *note*: There are some list methods that will change the order, but in general: the order will not change.

## Changeable
* The list is changeable, meaning that we can change, add, and remove items in a list after it has been created.

## List Length
* To determine how many items a list has, use the ```len()``` function:

## Python Collections
There are four collection data types in Python programming laguage:
* **List** is a collection which is ordered and changeable. Allows dupes
* **Tuple** is a cillection which is orderd and unchangeable. Allows dupes
* **Set** is a collection which is unordered, unchangeable*, and unindexed, No dupes
* **Dictionary** is a collection which is ordered** and changeable. No dupes

## Access List Items

  ### Negative Indexing
  * Negative indexing means starting from the end.
  * ```-1``` refers to the last item, so on etc.
    
    ```python
      thislist = ["apple", "banana", "cherry"]
      print(thislist[-1]) # output: "cherry"
    ```
  ### Range of Indexes
  * You can specify a range of indexes by specifying where start and where to end the range.
  * When specifying a range, the return value will be a new list with the specified items.

    ```python
    thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
    print(thislist[2:5]) # output: "cherry", "orange", "kiwi"
    ```
    
  * By leaving out the *start* value, the range will start at the first item:
    ```python
      thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
      print(thislist[:4]) # output: "apple", "banana", "cherry", "orange"
    ```

  * By leaving out the *end* value, the range will go on to the end of the list:
    ```python
      thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
      print(thislist[2:]) # output: "cherry", "orange", "kiwi", "melon", "mango"
    ```

    ## Range of Negitive Indexes
    * Specific negitive indexes if you want to start the search from the end of the list:
    ```python
        thislist = ["apple", "banana", "cherry", "orange", "kiwi", "melon", "mango"]
        print(thislist[-4:-1]) # output: "cherry", "orange", "kiwi", "melon"
    ```
