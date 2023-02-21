# Python Cheatsheet

Welcome to the Python Cheatsheet repository, a collaborative effort to create a comprehensive and concise reference guide for Python programmers of all levels. This cheatsheet is designed to provide a quick and handy reference for essential syntax, data structures, and code examples, making it an ideal tool for anyone looking to quickly refresh their knowledge or learn new Python concepts.

![pyrhon trademark](https://imgur.com/EI3tlCc.png)

- [Python Cheatsheet](#python-cheatsheet)
  - [Beginner](#beginner)
    - [Print](#print)
    - [Input](#input)
    - [Variables](#variables)
    - [If-else](#if-else)
    - [For-loop](#for-loop)
  - [Intermediate](#intermediate)
    - [Functions](#functions)
    - [Classes](#classes)
    - [Try-except](#try-except)
    - [List comprehension](#list-comprehension)
    - [Dictionaries](#dictionaries)
  - [Advanced](#advanced)
    - [Lambda functions](#lambda-functions)
    - [Map](#map)
    - [Filter](#filter)
    - [Decorators](#decorators)
    - [Generators](#generators)
    - [Advanced string formatting](#advanced-string-formatting)
    - [List and dictionary comprehension](#list-and-dictionary-comprehension)

## Beginner:

#### [~ print()]()

This function is used to output text or variables to the console.

```python
 print("Hello, world!")
```

#### [~ input()]()

This function is used to receive input from the user.

```python
 name = input("What is your name? ")
 print("Hello, " + name + "!")
```

#### [~ variables]()

This is used to store data in a program.

```python
 x = 5
 y = 3
 print(x + y)
```

#### [~ if-else]()

This is used for conditional statements.

```python
 x = 5
 if x > 0:
     print("x is positive")
 else:
     print("x is negative")
```

#### [~ for-loop]()

This is used to iterate over a sequence of items.

```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
    print(x)
```

## Intermediate:

#### [~ functions]()

This is used to group a set of related code.

```python
 def greet(name):
     print("Hello, " + name + "!")
 greet("John")
```

#### [~ classes]()

This is used to define new types of objects.

```python
 class Person:
     def __init__(self, name):
         self.name = name
     def greet(self):
         print("Hello, " + self.name + "!")
 p = Person("John")
 p.greet()
```

#### [~ try-except]()

This is used to handle errors and exceptions.

```python
 try:
     x = 5/0
 except ZeroDivisionError:
     print("Cannot divide by zero.")
```

#### [~ list comprehension]()

This is a concise way to create lists.

```python
 nums = [1, 2, 3, 4, 5]
 squared_nums = [x**2 for x in nums]
 print(squared_nums)
```

#### [~ dictionaries]()

This is a data structure that stores key-value pairs.

```python
 person = {'name': 'John', 'age': 30, 'city': 'New York'}
 print(person['name'])
```

## Advanced:

#### [~ lambda functions]()

This is a way to create small, anonymous functions.

```python
 double = lambda x: x*2
 print(double(5))
```

#### [~ map()]()

This is a built-in function that applies a given function to all items in an input list.

```python
 nums = [1, 2, 3, 4, 5]
 squared_nums = list(map(lambda x: x**2, nums))
 print(squared_nums)
```

#### [~ filter()]()

This is a built-in function that filters items in an input list based on a given condition.

```python
 nums = [1, 2, 3, 4, 5]
 even_nums = list(filter(lambda x: x % 2 == 0, nums))
 print(even_nums)
```

#### [~ decorators]()

This is a way to modify the behavior of functions by wrapping them in another function.

```python
 def my_decorator(func):
     def wrapper():
         print("Something is happening before the function is  called.")
         func()
         print("Something is happening after the function is  called.")
     return wrapper

 @my_decorator
 def say_hello():
     print("hello")

 say_hello()
```

#### [~ generators]()

This is a way to create iterator objects that can be used to iterate over a sequence of items.

```python
 def my_range(x):
     i = 0
     while i < x:
         yield i
         i += 1

 for num in my_range(5):
 print(num)
```

#### [~ advanced string formatting]()

This is a way to format strings in a more powerful and flexible way.

```python
 name = "John"
 age = 30
 print(f"My name is {name} and I am {age} years old.")
```

#### [~ list and dictionary comprehension]()

This is a more advanced way to create lists and dictionaries by using a single line of code.

```python
nums = [1, 2, 3, 4, 5]
squared_nums = {x: x**2 for x in nums}
print(squared_nums)
```

This cheatsheet is just a sample of the many features and capabilities of the Python language. It is highly recommended to continue learning and practicing Python to become proficient in using it.

## Contributing

We believe that the best cheatsheet is one that is created collaboratively by the community. Therefore, we welcome and encourage contributions of any size or form from the community. Whether it's fixing a typo or adding a new section, any contribution you make will help make this cheatsheet more helpful and accurate.

To contribute, please follow these steps:

1. Fork the repository and create a new branch for your changes.
2. Make your changes to the cheatsheet file.
3. Test your changes to ensure they are working properly.
4. Submit a pull request to the main repository and wait for the review.

We value and appreciate all contributions, big or small, and we are committed to working with you to make this cheatsheet the best it can be. Thank you for your help in making this cheatsheet a valuable resource for the community.
