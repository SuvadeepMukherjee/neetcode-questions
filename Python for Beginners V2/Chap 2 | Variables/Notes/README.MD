# Variables

## Variable Declaration 

- To declare a variable use the following way 

  ```python
  message="Hello , world!"
  ```

## Variable Naming

- a variable name should be descriptive and easy to understand

  ```python
  capital_of_uk = "London"
  print(capital_of_uk)
  ```

## Naming Convention

- In python we typically use snake case to declare a variable 

## Reassigning Variables

- We can reassign variables 

  ```python
  message = "The first message"
  message = "The second message"
  print(message)
  ```

## Multiple Assignments

- Multiple assignment in python 

  ```python
  msg1, msg2 = "Hello", "World"
  ```

- Swapping the values of variables

- ```python
  msg1, msg2 = "Hello", "World" # msg1 = "Hello", msg2 = "World"
  msg1, msg2 = msg2, msg1       # msg1 = "World", msg2 = "Hello"
  ```

## Variable Types

- A variable is an integer type when it holds a whole number value.

- A variable is a floating-point number type when it holds a decimal number value.

- A variable is a boolean type when it holds a `True` or `False` value

- A variable is a string type when it holds a sequence of characters, inside quotes.

- A variable is a list type when it holds a collection of comma separated values, inside square brackets.

- We can print the type of a variable or value using the `type()` function in Python. For example:

  ```python
  print(type(10))
  ```

## Dynamic Typing

- In Python a single variable's type can change throughout the code. This is called **dynamic typing**

## Type Casting

- A variable in Python can be converted to a different type using **type casting**

- For example, the following code will run without any errors:

  ```python
  variable = 10.9
  print(int(variable)) # 10
  ```

## Type Errors 

- We can't convert a string to an integer , unless the string is a number .This code will cause a **ValueError**

  ```python
  message = "Hello"
  message = int(message)
  ```

   

## Empty Variable 

- If we want to declare a variable without a value, we can use the `None` keyword. This is used to indicate that the variable has no value.

- If we try to declare a variable without explicity assigning a value to it, we will get an error.

  ```python
  name
  ```

- However, if we assign the variable to `None`, we can declare the variable without a value.

  ```python
  name = None
  ```

  