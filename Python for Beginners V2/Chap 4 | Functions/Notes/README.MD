# Functions

## Introduction to Functions

- Below we are defining a function that prints "Hello, world! "

  ```python
  def greet():
      print("Hello, world!")
  ```

## Function Declaration

- Functions must be defined before they can be called

## Parameters

- a function can be defined with parameters

  ```python
  def greet(name):
      msg = "Hello, " + name
      print(msg)
  
  greet("Alice")  # This will print "Hello, Alice"
  ```

## Multiple Parameters

- Functions can be defined to accept more than one parameter.

- The parameters are separated by commas in the function definition

- When calling the function, the arguments are also separated by commas

  ```python
  def greet(name, greeting):
      message = greeting + " " + name
      print(message)
  
  greet("Alice", "Hello")  # This will print "Hello Alice"
  ```

## Return Statement

- We can also return a value from a function 

- ```python
  def add(x, y):
      return x + y
  
  result = add(3, 5)
  print(result)  # This will print 8
  ```

## Type Hints

- In Python, you can add type hints to your functions to indicate what type of data the function expects to receive and return

- ```python
  def add(x: int, y: int) -> int:
      return x + y
  ```

## Scope

- scope refers to the visibility or accessibility of variables within different parts of the code
- Global scope
  - Variables declared outside of any function have a global scope.
  - They can be accessed from anywhere in the program, including inside functions.
- Local scope
  - Variables declared within a function have a local scope.
  - They can only be accessed within the function in which they are defined.
  - Local variables are created when the function is called and destroyed when the function exits.

## Default Arguments

- We can specify default values for parameters in a function defination

  ```python
  def greet(name="world"):
      print("Hello, " + name + "!")
  
  greet()       # This will print "Hello, world!"
  greet("Bob")  # This will print "Hello, Bob!"
  ```