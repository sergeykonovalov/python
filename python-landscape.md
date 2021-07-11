# Python Landscape

## Installation

## Basics

- Variables (naming, multiple assignment)
- constants
- Comments
- print()
- input()
- Operators and operations (ppresedence) > < >> <<
- eval()
- expressions and statements
- docstring
- walrus operator :=
- division/floor/modulo
- first-class objects: functions, modules, classes. You can pass them as arguments.
- Everything is an object.
- Context:
  - If excpetion if not handled in function, it goes up the stack and handled in parent, and so forth. Python will add traceback to standard error.

## Conditions and Control

- if
- elif
- AND
- OR
- ternary
- is vs ==
- not

## Loops

- while
- for
- range
  - range(20) == range(0, 20)  # last element will be 19
  - Third argument defines step (integer).
- iterables
- enumerate
- break, continue, pass
  - pass should be the least available line

## Data Types

- type()
- Casting
- Conversion
- immutability
- booleans: true, false
- None
  - object, representing absence of value
  - Similar to null.
  - Same, as 0, [] and empty string.
  - Any function returns None if not explicitly indicated otherwise.
  - So when you assign value to a function, without return inside, value will be None: `SomeVar = func_name()`
- NUmericalL int, floats, decimals, complex
- Strings (methods, splitting, replace, fromatting; immutability, len, concat, index, slicing, methods, startswith, endswith, strips , casing) + f-strings
- Lists (add, update, delete, methods, multidimensional, index, slice, iteration, mutation - exted, insert(index, element) +pop+del+remove(element)+clear+reverse+ sort, copy, split, join; comprehensions) + methods append(element), count(element) + using min() and max() with lists.
- Sets: add update remove discard, union, difference, symmetrci_diccference, issubset, issuperset, frozenset)
- Tuples + named tuples
  - Similar to lists but immutable: mytup = (1, "www", 36.6)
  - Trying to reassign value causes TypeError
  - Like with lists and dictionaries, TUPLES can be nested in each other.
  - One can create also: `mytup2 = ()` or `mytup3 = "one", "two", "three"`
  - TUPLES are faster than lists.
- Dictionaries (in not, pop, clear, update, sorted, comprehensions)
  - Pairs of key-value.
  - dict = {"Name1": 36.6, "Name2", 42}
  - print(dict["Name1"])
  - Trying to address invalid key raises KeyError:
  - dict(["Name3"]) --> KeyErrror: "Name3"
  - If you create empty dictionary {}, and address missing element dict[0], also KeyError raises.
  - Only immutable objects can be dictionary keys.
  - Mutable cannot be hashed.
  - Lists and dictionaries are mutable.
  - bad_dict = {[0, 1, 2]: "value"}
  - Key (list) is mutable --> TypeError.
  - List values can be changed, and if you set dictionary element with key it yet does not have, it will add element to dictionary:
  - dict["Name3"] = "three"
  - To determine if a key in dictionary one can use in nd not in construction.
  - print("Name3" in dict) --> True
  - Dictionaries have method .get(index, optionalRetrunValueIfNoKey) which returns value by index key or None if not found.
  - print(dict.get("Name4", "Not in my dict") --> Not in my dict
  - print(dict.get("Name2") --> 42
  - print(dict.get("Name700", 699) --> 699
  - defaultdict
  - ordereddict
  - userdict
  - counter
- Ranges as data type
- Associative arrays
- HashMaps
- Bytes
- ByteArray
- Slicing
  - Colon separated integers where first is index start,second is end (inclusively)
  - As arguments to range will include first index element, but not the second index argument,This also valid for ranges supplied as function arguments. :7 8:
  - Slicing can also be done on TUPLES.
  - Optional third argument to slices is step used to walk throught the list or TUPLE?

## Debugger

- step over
- logging

## Regular Expressions

- findall
- finditer
- sub()
- split
- subn
- match
- search

## Networking

- check IP
- ssh
- sniffing
- lldp
- dhcp

## Functions

- arguments (args, kwargs, default)
  - variable length
  - The *args and **keywordargs forms are used for passing lists of arguments and dictionaries of arguments, respectively.
- by reference vs by value
- recursion
- global/local scope (global and nonlocal)
- map
- filter
- zip
- sort
- reduce
- lambdas
- decorators (higher order functions; closures; nonlocal; functools.wrap; next and iter)
- generators
  - as coroutines
- list comprehensions
- set/dict comprehensions
- return

## OOP

- principles: inheritance, encapsulation, abstraction, polymorphism
  - method resolution order
  - isinstance
  - issubclass
- constrictors
- self
- equality vs identity
- shallow vs deep copy
- methods
  - getter / setters
  - classmethod
  - staticmethod
  - dunder
    - _str__
    - __rep__
    - __eq__
    - __bool__
    - __len__
    - __getitem__
    - __setitem__
    - __del__
- properties (attributes; static; default values; protected)
  - private vs public
- super()
- __init__()
- abstract classes
- descriptors

## Multithreading

- multiprocessing vs multithreading
- locks
- sharing data

## Asynchronious

- Async IO

## Modules

- Create
- import
- __name__
- PIP
- as
- reloading
- naming conflict

## HTTP

- request: get, post, put, delete

## I/O

- sys
- argparse
- create
- write
- append
- read (file or by line)
- directories
- copy/move
  - directory tree
  - with
  - cursor
- unicode

### CSV

- reading (deserialization)
- writing (serialization)
- dialects

## Pickle

- reading (deserialization)
- writing (serialization)

## Shelve

### JSON

- reading (deserialization)
- writing (serialization)

## Standard Library

- math
- datetime (compare, operations)
- time
- timedelta
- random (random, randint, and randrange; choice, sample, shuffle)
- help
- all
- max
- min
- sum
- dir
- os
- shutil
- subprocess
- decimal

## GUI

- Tkinter
- Control mouse
- Control kb
- Making executable

## Third-Party Modules

### OpenCV

- loading
- displaying
- resizing
- saving
- motion detector

### Image Processing

### Bokeh

- plots
- connecting with pandas
- visual attributes

### Plotly

- scatter plot
- line chart
- pie chart
- bar chart
- histogram

### PDF

### Emails

- udp vs tcp
- plaintext
- html
- attachments

### Word

### Excel

- read file
- read cells
- create files
- modify sheets
= modify styles

### Arcade

### SQL

- CRUD
- Manage tables
- parametrized statemsnts for SQL
- psycopg2
- sqlite

### Flask

- routes and arguments
- controllers
- templates
- statics

## Exceptions and Error Handling

- try
- except
- finally
- raise
- NameError (unknown variable used)
- ValueError (function called on a value of correct type, but wrong value)
- TypeError (a function is called on a value of unappropriate type)
- SyntaxError (code cannot be parsed properly)
- IndexError (list indexed for out of range)
- ImportError (failed import)

## Testing

### doctest

### unittest

- assertEqual
- assertNotEqual
- truthy/falsy
- nullness
- types
- errors
- setUp and tearDown

### Mocking

- return_value
- side_effect

### pytest

### selenium

## Machine Learning

- linear regression
- multiple (polynominal) linear regression
- KNN
- Naive Bayes

- importing
- visualization
- splitting
- training
- testing
- CNN

## Data Scienece

### Pandas

- Load CSV
- write CSV
- rows
- columns
- series vs datra frames
- filtering
- analyzing
- index / multiindex
- merging, joining
- groupby

### Matplotlib

### Seaborn

### Numpy

- convert images to array
-indexing
- slicing
-stackng
- splitting

## Scraping

### Beautiful Soup

### Scrapy

## APIs

- Twitter
- OpenWeather
- RazorPay
- Twilio

## Virtual Environemnts

- venv
- config vscode
- config eclipse

## Linting

- pylint

## Django

- settings
- urls and views
- templates
- models
- query sets
- forms
- variables
- admin
- DRF
- serializers

## Context Manager

## Enumarators

## Metaprogramming

- __new__
- meta class
- class decorator
- __prepare__
- attributre read and write

## Algorithms

- Big O
- array sequence
- stack queue
- linked list
- tree
- search
- sorting
- graph
- riddles

## Design Patterns

- SOLID
- builder
- factores
- prototype
- singleton
- adapter
- bridge
- composite
- decorator
- facade
- flyweight
- proxy
- chain of resp
- command
- intrepreter
- iterator
- mediator
- momento
- observer
- state
- strategy
- template method
- visitor

## Python Tops

(Python Developer Survey by JetBrains)[https://www.jetbrains.com/lp/python-developers-survey-2020/]

- Web
  - 46 Flask
  - 43 Django
- Data Science
  - 62 NumPy
  - 56 Pandas
  - 46 Matplotlib
  - 33 SciPy
  - 31 SciKit Learn
  - 25 Tensorflow
  - 19 Keras
  - 18 Seaborn
  - 17 Pytorch
  - 12 NLTK
- Unit Testing
  - 49 pytest
  - 28 unittest
- Other
  - 54 Requests
  - 32 Pillow
  - 22 AsyncIO
  - 19 Tkinter
  - 16 Scrapy
- ORM
  - 35 SQLAlchemy
  - 32 RAW SQL
- Databases
  - 46 Postgres
  - 39 SQLite
  - 38 MySQL
  - 19 Mongo
  - 18 Redis
- Big Data
  - 11 Spark
  - 9 Kafka
- CI
  - GitLab 23
  - Jenkins 21