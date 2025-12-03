# Variables

## Variable declaration

- To declare a variable we use the following syntax 

  ```python
  message ="hello world" print(message)
  ```

## Variable Naming

- If we wanted a variable to store the capital of the United Kingdom we would use the following naming convention 

- The above naming convention is called snake_case

  ```python
  capital_of_uk = "London"
  print(capital_of_uk)
  ```

## Reassigning Variables

- Variables can change their value , this is called re assigning a variable 

- ```python
  message = "The first message"
  message = "The second message"
  print(message)
  ```

## Multiple assignments 

- To assign multiple variables in a single line use the following syntax 

  ```python
  msg1, msg2 = "Hello", "World" 
  ```

- is equivalent to:

  ```python
  msg1 = "Hello"
  msg2 = "World"
  ```

## Swap 

- To swap 2 values use the following syntax

  ```python
  msg1, msg2 = "Hello", "World" # msg1 = "Hello", msg2 = "World"
  msg1, msg2 = msg2, msg1       # msg1 = "World", msg2 = "Hello"
  ```

## Variable Types

- Python can hold different types of data, such as *integers*, *decimal numbers* (aka floating-point numbers), *strings*, *booleans*, *lists*, and more

- ```python
  age = 25             # integer
  temperature = 98.6   # floating-point number
  is_true = True       # boolean
  name = "Alice"       # string
  my_list = [1, 2, 3]  # list
  ```

## Dynamic Typing

- In Python a single variable's type can change throughout the code. This is called **dynamic typing**

## Type Casting

- A variable in python can be converted to a different type using type casting 

  ```python
  variable = 10.9
  print(int(variable))
  ```

- This code will output: `10`

## Type Errors 

- Even though variable types can change there are still rules about what types of varibles can be used together . We can't convert a string to an integer , unless the string is a number .The beiow code will cause a ValueError

```python
message = "Hello"
message = int(message)
```

## Empty Variable

- If we want to declare a variable without a value we can use the `None` keyword.This is used to indicate that the variable has no value  

  ```python
  var = None
  ```

  