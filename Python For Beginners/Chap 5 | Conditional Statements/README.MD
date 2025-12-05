# Conditional Statements

## Comparision Operators 

-  Comparision operators are used to compare values.They evaluate to `True` or `False` depending on the values you compare  
- The comparision operators are:
  - `==` Equal to
  - `!=` Not equal to
  - `<` Less than
  - `>` Greater than
  - `<=` Less than or equal to
  - `>=` Greater than or equal to

## If Statement

- if we wanted to run some code only in certain situations we can use the keyword if 

## If statement Scope

- Unlike functions, `if` statements do not create a new scope. This means that variables defined inside an `if` statement are accessible outside of the `if` statement

  ```python
  if True:
      message = "Hello"
  
  print(message)  # This will print "Hello"
  ```

- within functions , if statements have the same scope as the function.This means that variables defined inside an if statement are accessible within that function , but not outside of it 

- ```python
  def is_balance_low(balance: int):
      if balance <= 100:
          message = "Warning: Low balance."
      print(message)
  
  is_balance_low(50)  # This will print "Warning: Low balance."
  print(message)  # This will cause an error
  ```

   

## If-Else Statements

- else statement runs a seperate piece of code when an if statement fails to execute 

- ```python
  balance = 100
  
  if balance < 0:
      print("Account is overdrawn.")
  else:
      print("Account is in good standing.")
  ```

## elif statements

- We can create a chain of conditional statements using the `elif` keyword (standing for else-if). This allows us to check multiple conditions in order, until one of them is true. Here's an example:

- ```python
  balance = 1000
  
  if balance < 0:
      print("Your account is overdrawn.")
  elif balance == 0:
      print("Your account balance is zero.")
  elif balance < 100:
      print("Your account balance is low.")
  else:
      print("Your account balance is healthy.") # This will execute
  ```

## Logic Condition

- we can use the `or` , `and` and `not` operators to evaluate expressions into `True` or `False` . We can use these expressions to execute conditional code blocks

  ```python
  balance = 500
  
  if balance > 0 and balance < 1000:
      print("Balance is between 0 and 1000.")
  ```

##  Truthy and Falsy

- it's possible to use non-boolean values to execute conditional statements.

- Python has the concept of **truthy** and **falsy** values

  - truthy
    - A value is **truthy** if it is:
      - `True` (boolean)
      - All integers other than `0`
      - All floats other than `0.0`
      - All strings other than `""`
      - All collections with at least one element
  - falsy
    - A value is **falsy** if it is:
      - `False` (boolean)
      - `None` (NoneType)
      - `0` (integer)
      - `0.0` (float)
      - `""` (empty string)
      - `[]` (empty list)
      - Most other empty collections (e.g. empty tuple, empty set, empty dictionary)

  