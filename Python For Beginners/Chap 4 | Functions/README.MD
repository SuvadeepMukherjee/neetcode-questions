# Functions

## Introduction to Functions

- Functions are defined using the `def` keyword followed by the function name and parentheses with a colon `():`

- The code that belongs to the function *must* be indented with whitespace

  ```python
  def greet():
      print("Hello, world!")
  ```

## Function Declaration

- Functions must be defined before they can be called

## Parameters and arguments

- parameter
  -  A **parameter** is a variable in a function definition
- arguments
  - arguments are the data you pass into the function's parameters

## Multiple Parameters

- Functions can be defined to accept more than one parameter

- The parameters are separated by commas in the function definition

- When calling the function, the arguments are also separated by commas.

  

  ```python
  def greet(name, greeting):
      message = greeting + " " + name
      print(message)
  
  greet("Alice", "Hello")  # This will print "Hello Alice"
  ```

## Return statement

- If we return a value from a function we can use the result of the function in other parts of our code , outside of the original function 

- ```python
  def add(x, y):
      return x + y
  
  result = add(3, 5)
  print(result)  # This will print 8
  ```

## Type Hints 

- We can add type hints to our function to indicate what type of data the function expects to receive and return 

- To add a type hint for a parameter, you add a colon after the parameter name and then the type of data you expect. To add a return type, you add a right arrow (`->`) after the closing parenthesis and then the type of data you expect to return (before the colon).

- To not return anything we would return `None`

  ```python
  def add(x: int, y: int) -> int:
      return x + y
  ```

  ```python
  def greet(name: str) -> None:
      print("Hello, " + name)
  ```

## Scope 

- Scope defines where a variable can be seen or used in a program.
- A value passed into a function exists only inside that function’s scope.
- Variables inside the function are separate from variables outside it, even if they have the same name.
- Changes made to the variable inside the function do not affect the variable outside.

## Global Scope and Local Scope

- Global Scope
  - Variables declared outside of any function have a global scope.
  - They can be accessed from anywhere in the program, including inside functions.
- Local Scope
  - Variables declared outside of any function have a global scope.
  - They can be accessed from anywhere in the program, including inside functions.

## Default Arguments

- To specify default values for parameters in a function definition we use the following technique

  ```python
  def greet(name="world"):
      print("Hello, " + name + "!")
  
  greet()       # This will print "Hello, world!"
  greet("Bob")  # This will print "Hello, Bob!"
  ```

 