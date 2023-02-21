# Python Cheatsheet

Python is a popular programming language that is widely used. This cheatsheet for some common Python commands, organized by difficulty level:

## Beginner:

- print()
  This function is used to output text or variables to the console.

```python
 print("Hello, world!")
```

- input()
  This function is used to receive input from the user.

```python
 name = input("What is your name? ")
 print("Hello, " + name + "!")
```

- variables
  This is used to store data in a program.

```python
 x = 5
 y = 3
 print(x + y)
```

- if-else
  This is used for conditional statements.

```python
 x = 5
 if x > 0:
     print("x is positive")
 else:
     print("x is negative")
```

- for loop
  This is used to iterate over a sequence of items.

```python
fruits = ["apple", "banana", "cherry"]
for x in fruits:
    print(x)
```

## Intermediate:

- functions
  This is used to group a set of related code.

```python
 def greet(name):
     print("Hello, " + name + "!")
 greet("John")
```

- classes
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

- try-except
  This is used to handle errors and exceptions.

```python
 try:
     x = 5/0
 except ZeroDivisionError:
     print("Cannot divide by zero.")
```

- list comprehension
  This is a concise way to create lists.

```python
 nums = [1, 2, 3, 4, 5]
 squared_nums = [x**2 for x in nums]
 print(squared_nums)
```

- dictionaries
  This is a data structure that stores key-value pairs.

```python
 person = {'name': 'John', 'age': 30, 'city': 'New York'}
 print(person['name'])
```

## Advanced:

- lambda functions
  This is a way to create small, anonymous functions.

```python
 double = lambda x: x*2
 print(double(5))
```

- map()
  This is a built-in function that applies a given function to all items in an input list.

```python
 nums = [1, 2, 3, 4, 5]
 squared_nums = list(map(lambda x: x**2, nums))
 print(squared_nums)
```

- filter()
  This is a built-in function that filters items in an input list based on a given condition.

```python
 nums = [1, 2, 3, 4, 5]
 even_nums = list(filter(lambda x: x % 2 == 0, nums))
 print(even_nums)
```

- decorators
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

- generators
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

- advanced string formatting
  This is a way to format strings in a more powerful and flexible way.

```python
 name = "John"
 age = 30
 print(f"My name is {name} and I am {age} years old.")
```

- list and dictionary comprehension
  This is a more advanced way to create lists and dictionaries by using a single line of code.

```python
nums = [1, 2, 3, 4, 5]
squared_nums = {x: x**2 for x in nums}
print(squared_nums)
```

This cheatsheet is just a sample of the many features and capabilities of the Python language. It is highly recommended to continue learning and practicing Python to become proficient in using it.
