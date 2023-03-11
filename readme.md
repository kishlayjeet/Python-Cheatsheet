# Python Cheatsheet 🐍

Welcome to the Python Cheatsheet repository, the go-to reference guide for Python programmers of all levels. Our collaborative effort has produced a comprehensive and concise cheatsheet that serves as a quick and handy reference for essential syntax, data structures, and code examples. Whether you're looking to refresh your knowledge or learn new Python concepts, this cheatsheet is the perfect tool to help you do so efficiently. Join our community and start exploring the vast world of Python programming today!

![python trademark](https://imgur.com/EI3tlCc.png)

- [Python Cheatsheet](#)
  - [Beginner](#beginner)
    - [Strings](#strings)
    - [If-else](#if-else)
    - [For-loop](#for-loop)
    - [List](#list)
    - [Tuples](#tuples)
    - [Sets](#sets)
  - [Intermediate](#intermediate)
    - [Functions](#functions)
    - [Recursion](#recursion)
    - [List Comprehension](#list-comprehension)
    - [Dictionaries](#dictionaries)
  - [Advanced](#advanced)
    - [Lambda Functions](#lambda-functions)
    - [Map](#map)
    - [Filter](#filter)
    - [Decorators](#decorators)
    - [Generators](#generators)
    - [File I/O](#file-i-o)
    - [Dictionary Comprehension](#dictionary-comprehension)
  - [Exception Handling](#exception-handling)
  - [Regular Expressions](#regular-expressions)
  - [Multithreading and Multiprocessing](#multithreading-and-multiprocessing)
  - [Object-Oriented Programming](#object-oriented-programming)
- [Contribution](#contributing)

## Beginner:

### Strings

Strings are a fundamental data type in Python, and there are many built-in functions and methods for working with strings.

```python
# String creation
s1 = 'hello world'
s2 = "hello world"
s3 = '''hello
world'''
s4 = """hello
world"""

# String formatting
name = "John"
age = 25
print("My name is %s and I'm %d years old." % (name, age))
print("My name is {} and I'm {} years old.".format(name, age))

# String manipulation
s = "hello world"
print(len(s))
print(s.lower())
print(s.upper())
print(s.strip())
print(s.replace("world", "there"))
print(s.split())

# String slicing
print(s[0])
print(s[0:5])
print(s[6:])
print(s[0:5:2])

# String concatenation
s1 = "hello"
s2 = "world"
print(s1 + " " + s2)
print(" ".join([s1, s2]))

# String formatting with f-strings
print(f"My name is {name} and I'm {age} years old.")
```

### If-else

The if-else statement is used to execute a block of code if a certain condition is true, and another block of code if the condition is false.

```python
# If-else statement
if condition:
    # code to execute if the condition is true
else:
    # code to execute if the condition is false

# Comparison operators
# ==, !=, <, >, <=, >=

# Logical operators
# and, or, not

# If-elif-else statement
if condition1:
    # code to execute if condition1 is true
elif condition2:
    # code to execute if condition2 is true
else:
    # code to execute if all conditions are false

# Ternary operator
value_if_true if condition else value_if_false

# Truthiness
# non-zero values are true, while zero, None, and empty  sequences are false
```

### For-loop

This is used to iterate over a sequence of items.

```python
# For-loop
for value in sequence:
    # code to execute for each value

# Range function
range(start, stop, step)

# Break statement
for value in sequence:
    if condition:
        break

# Continue statement
for value in sequence:
    if condition:
        continue
    # code to execute for each value (except those that meet  the condition)

# Enumerate function
for index, value in enumerate(sequence):
    # code to execute for each index and value

# Zip function
for value1, value2 in zip(sequence1, sequence2):
    # code to execute for each pair of values

# List comprehension
new_list = [expression for value in sequence if condition]
```

### List

Lists are a versatile data structure in Python that can hold a collection of values.

```python
# List creation
my_list = [1, 2, 3, "four", 5.0]

# List indexing
my_list[0]    # returns the first element (1)
my_list[-1]   # returns the last element (5.0)

# List slicing
my_list[start:stop:step]

# List methods
my_list.append(element)
my_list.extend(sequence)
my_list.insert(index, element)
my_list.remove(element)
my_list.pop(index)
my_list.index(element)
my_list.count(element)
my_list.sort()
my_list.reverse()

# List comprehension
new_list = [expression for element in old_list if condition]

# Nested lists
nested_list = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
```

### Tuples

Tuples are similar to lists, but they are immutable (i.e., their contents cannot be changed once they are created.).

```python
# Tuple creation
my_tuple = (1, 2, 3, "four", 5.0)

# Tuple indexing
my_tuple[0]    # returns the first element (1)
my_tuple[-1]   # returns the last element (5.0)

# Tuple slicing
my_tuple[start:stop:step]

# Tuple methods
my_tuple.count(element)
my_tuple.index(element)

# Tuple packing and unpacking
my_tuple = 1, 2, "three"
a, b, c = my_tuple
```

Tuples are commonly used to group related data, such as a latitude and longitude coordinate or a date and time value.

### Sets

```python
# Set creation
my_set = {1, 2, 3, 4, 5}
my_set = set([1, 2, 3, 4, 5])

# Set operations
my_set.add(element)
my_set.update(sequence)
my_set.remove(element)
my_set.discard(element)
my_set.pop()
my_set.clear()
my_set.union(other_set)
my_set.intersection(other_set)
my_set.difference(other_set)
my_set.symmetric_difference(other_set)
my_set.issubset(other_set)
my_set.issuperset(other_set)

# Set comprehension
my_set = {expression for element in old_set if condition}
```

Sets are commonly used to perform mathematical operations and remove duplicates from a sequence.

## Intermediate:

### Functions

This is used to group a set of related code.

```python
# Function declaration
def my_function(param1, param2=default_value):
    # function body
    return result

# Function arguments
my_function(positional_arg1, positional_arg2)
my_function(keyword_arg1=value1, keyword_arg2=value2)
my_function(*args)
my_function(**kwargs)

# Lambda functions
lambda arg1, arg2: expression

# Function decorators
@my_decorator
def my_function():
    # function body

# Built-in functions
print(value)
len(sequence)
range(start, stop, step)
enumerate(iterable)
zip(iterable1, iterable2)
map(function, iterable)
filter(function, iterable)
sorted(iterable)
```

Functions are used to encapsulate and reuse code, making it more maintainable andeasier to understand. They can be used for a wide variety of tasks, such as performing calculations,processing data, and interacting with APIs and databases.

### Recursion

```python
# Recursive functions
def my_function(arg):
    if base_case:
        # base case
        return value
    else:
        # recursive case
        return my_function(new_arg)

# Memoization
memo = {}

def my_function(arg):
    if arg in memo:
        return memo[arg]
    else:
        # calculate value
        result = ...
        memo[arg] = result
        return result

# Tail recursion
def my_function(arg, accumulator=0):
    if base_case:
        # base case
        return accumulator
    else:
        # recursive case
        return my_function(new_arg, new_accumulator)
```

Recursion can be used to solve problems that can be broken down into smaller subproblems. It is particularly useful for tree and graph traversal, search algorithms, and sorting and partitioning data.

### List Comprehension

This is a concise way to create lists.

```python
# Create a new list using list comprehension
numbers = [1, 2, 3, 4, 5]
squared_numbers = [x**2 for x in numbers]
print(squared_numbers) # Output: [1, 4, 9, 16, 25]

# Create a new list using list comprehension with conditionals
even_numbers = [x for x in numbers if x % 2 == 0]
print(even_numbers) # Output: [2, 4]

# Create a new list of tuples using list comprehension
names = ['John', 'Jane', 'Mike']
name_lengths = [(name, len(name)) for name in names]
print(name_lengths) # Output: [('John', 4), ('Jane', 4),  ('Mike', 4)]

# Flatten a list of lists using list comprehension
list_of_lists = [[1, 2], [3, 4], [5, 6]]
flattened_list = [item for sublist in list_of_lists for item in  sublist]
print(flattened_list) # Output: [1, 2, 3, 4, 5, 6]
```

### Dictionaries

This is a data structure that stores key-value pairs.

```python
# Creating dictionaries
my_dict = {'key1': value1, 'key2': value2}
my_dict = dict(key1=value1, key2=value2)

# Accessing and modifying values
value = my_dict['key']
my_dict['key'] = new_value

# Iterating over dictionaries
for key in my_dict:
    value = my_dict[key]

# Dictionary comprehension
my_dict = {key: expression for item in iterable if condition}

# Built-in methods
keys = my_dict.keys()
values = my_dict.values()
items = my_dict.items()
```

Dictionaries are useful for storing and accessing data using keys, and are often used to represent real-world objects and relationships between them.

## Advanced:

### Lambda functions

This is a way to create small, anonymous functions.

```python
# Syntax of a lambda function
lambda arguments: expression

# Using a lambda function as an argument to a sorting function
my_list.sort(key=lambda x: x[1])

# Using a lambda function as part of a list comprehension
new_list = [lambda_function(x) for x in old_list]
```

**Limitations of Lambda Functions:** Lambda functions are limited to a single expression, which means that they cannot contain statements or multiple lines of code. For more complex operations, it is often better to use a regular function definition.

### Map

This is a built-in function that applies a given function to all items in an input list.

```python
# Syntax of the map() function
map(function, iterable)

# Using the map() function to apply a function to each element  of an iterable
my_list = [1, 2, 3, 4]
new_list = map(lambda x: x**2, my_list)
# Output: [1, 4, 9, 16]

# Using the map() function with built-in functions
my_list = ['1', '2', '3', '4']
new_list = map(int, my_list)
# Output: [1, 2, 3, 4]

# Converting the result of the map() function to a list
my_list = [1, 2, 3, 4]
new_list = list(map(lambda x: x**2, my_list))
# Output: [1, 4, 9, 16]
```

### Filter

This is a built-in function that filters items in an input list based on a given condition.

```python
# Syntax of the filter() function
filter(function, iterable)

# Using the filter() function to remove certain elements from  an iterable
my_list = [1, 2, 3, 4]
new_list = filter(lambda x: x % 2 != 0, my_list)
# Output: [1, 3]

# Using the filter() function with built-in functions
my_list = ['hello', 'world', '', 'python']
new_list = filter(None, my_list)
# Output: ['hello', 'world', 'python']

# Converting the result of the filter() function to a list
my_list = [1, 2, 3, 4]
new_list = list(filter(lambda x: x % 2 != 0, my_list))
# Output: [1, 3]
```

### Decorators

This is a way to modify the behavior of functions by wrapping them in another function.

```python
# Syntax of decorators
@decorator_name
def my_function():
    # function code here

# Creating a decorator
def my_decorator(func):
    def wrapper(*args, **kwargs):
        # code to execute before the original function is called
        func(*args, **kwargs)
        # code to execute after the original function is called
    return wrapper

# Using a decorator
@my_decorator
def my_function():
    # function code here

# Passing arguments to a decorated function
def my_decorator(func):
    def wrapper(*args, **kwargs):
        # code to execute before the original function is called
        func(*args, **kwargs)
        # code to execute after the original function is called
    return wrapper

# Chaining multiple decorators
@decorator1
@decorator2
def my_function():
    # function code here
```

### Generators

This is a way to create iterator objects that can be used to iterate over a sequence of items.

```python
# Creating a generator using a function
def my_generator():
    for i in range(10):
        yield i

# Using a generator
my_numbers = my_generator()
for num in my_numbers:
    print(num)

# Creating a generator using a comprehension
my_generator = (i for i in range(10))

# Passing values to a generator
def my_generator(start, end):
    for i in range(start, end):
        yield i

# Generator expressions
my_numbers = (i for i in range(10))
for num in my_numbers:
    print(num)

# Using the next() function with a generator
my_generator = (i for i in range(10))
print(next(my_generator))

# Generator function as an iterator
class MyGenerator:
    def __init__(self):
        self.start = 0
        self.end = 10

    def __iter__(self):
        return self.generator()

    def generator(self):
        for i in range(self.start, self.end):
            yield i

# Using a generator inside a list comprehension
my_numbers = (i for i in range(10))
squared_numbers = [num**2 for num in my_numbers]

# Passing arguments to a generator through send()
def my_generator():
    received_value = yield
    print(received_value)

my_numbers = my_generator()
next(my_numbers)
my_numbers.send(10)
```

### File I/O

```python
# Open file for reading
file = open('filename.txt', 'r')

# Read file contents
file_contents = file.read()

# Close file
file.close()

# Open file for writing
file = open('filename.txt', 'w')

# Write to file
file.write('Hello, World!')

# Close file
file.close()

# Append to file
file = open('filename.txt', 'a')
file.write('Hello again, World!')
file.close()

# Read file line by line
file = open('filename.txt', 'r')
for line in file:
    print(line)
file.close()

# Check if file exists
import os
if os.path.exists('filename.txt'):
    print('File exists')

# Use "with" statement to open and close file
with open('filename.txt', 'r') as file:
    file_contents = file.read()

# Read CSV file using CSV module
import csv
with open('filename.csv', 'r') as csv_file:
    csv_reader = csv.reader(csv_file)
    for row in csv_reader:
        print(row)

# Write to CSV file using CSV module
import csv
with open('filename.csv', 'w', newline='') as csv_file:
    csv_writer = csv.writer(csv_file)
    csv_writer.writerow(['Name', 'Age', 'Country'])
    csv_writer.writerow(['John', '25', 'USA'])
    csv_writer.writerow(['Jane', '30', 'Canada'])
```

### Dictionary Comprehension

This is a more advanced way to create dictionaries by using a single line of code.

```python
# Create a new dictionary using dictionary comprehension
numbers = {'one': 1, 'two': 2, 'three': 3, 'four': 4}
squared_numbers = {key: value**2 for key, value in numbers.items ()}
print(squared_numbers) # Output: {'one': 1, 'two': 4, 'three':  9, 'four': 16}

# Create a new dictionary using dictionary comprehension with  conditionals
even_numbers = {key: value for key, value in numbers.items() if  value % 2 == 0}
print(even_numbers) # Output: {'two': 2, 'four': 4}

# Swap keys and values of a dictionary using dictionary  comprehension
numbers = {'one': 1, 'two': 2, 'three': 3, 'four': 4}
swapped_numbers = {value: key for key, value in numbers.items()}
print(swapped_numbers) # Output: {1: 'one', 2: 'two', 3:  'three', 4: 'four'}
```

## Exception Handling

```python
try:
    # block of code to be attempted
except ExceptionType1:
    # handle exception of type ExceptionType1
except ExceptionType2:
    # handle exception of type ExceptionType2
else:
    # execute if no exception is raised in the try block
finally:
    # execute regardless of whether an exception was raised or not
```

- Use a try block to enclose the code that might raise an exception.
- Use one or more except blocks to handle specific exception types.
- The else block is optional and executes only if no exceptions are raised in the try block.
- The finally block is optional and executes regardless of whether an exception was raised or not.

#### Common Built-in Exception Types:

- `Exception`: the base class for all exceptions.
- `ValueError`: raised when an argument has the right type but an inappropriate value.
- `TypeError`: raised when an operation or function is applied to an object of inappropriate type.
- `IndexError`: raised when an index is out of range.
- `KeyError`: raised when a key is not found in a dictionary.
- `FileNotFoundError`: raised when a file or directory is requested but does not exist.
- `IOError`: raised when an I/O operation (such as reading or writing a file) fails.
- `ZeroDivisionError`: raised when division or modulo by zero occurs.

#### Example:

```python
try:
    x = int(input("Enter a number: "))
    y = 1 / x
except ValueError:
    print("Invalid input. You must enter a number.")
except ZeroDivisionError:
    print("You cannot divide by zero.")
else:
    print(f"The reciprocal of {x} is {y}.")
finally:
    print("Thank you for using this program.")
```

This code prompts the user to enter a number and calculates its reciprocal. It handles two possible exceptions that can occur: ValueError if the user enters an invalid input (not a number) and ZeroDivisionError if the user enters zero. If no exception is raised, it prints the result. The finally block always executes, thanking the user for using the program.

## Regular Expressions

## Object-Oriented Programming

## Multithreading and Multiprocessing

Remember, Python is a powerful and constantly evolving language with many more features and capabilities beyond what is covered in this cheatsheet. To become proficient in using Python, it is important to continue learning and practicing.

## Contributing

We believe that the best cheatsheet is one that is created collaboratively by the community. Therefore, we welcome and encourage contributions of any size or form from the community. Whether it's fixing a typo or adding a new section, any contribution you make will help make this cheatsheet more helpful and accurate.

To contribute, please follow these steps:

1. Fork the repository and create a new branch for your changes.
2. Make your changes to the cheatsheet.
3. Test your changes to ensure they are working properly.
4. Submit a pull request to the main repository and wait for the review.

We value and appreciate all contributions, big or small, and we are committed to working with you to make this cheatsheet the best it can be. Thank you for your help in making this cheatsheet a valuable resource for the community.
