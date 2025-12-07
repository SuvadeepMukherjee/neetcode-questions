# Conditional Statements

## Comparision Operators

- Comparison operators are used to compare values. They evaluate to `True` or `False` depending on the values you compare
- Comaprision Operators
  - `==` Equal to
  - `!=` Not equal to
  - `<` Less than
  - `>` Greater than
  - `<=` Less than or equal to
  - `>=` Greater than or equal to

## If Statements

- if statements allow us to run some code only in certain situations

## If Statements Scope 

- If statements do not create a new scope .This means that variables defined inside an `if` statement are accessible outside of the `if` statement.

  ```python
  if True:
      message = "Hello"
  
  print(message)  # This will print "Hello"
  ```

## If-Else Statements

- else block will only execute if previous if statement fails to execute

## Else-If Statements

- We can create a chain of conditional statements using the `elif` keyword (standing for else-if). This allows us to check multiple conditions in order, until one of them is true

## Logic Condition

- We can use the `or` , `and` and `not` operators to evaluate expressions into `True` or `False` 

- We can use these expressions to execute conditional code blocks

  ```python
  balance = 500
  
  if balance > 0 and balance < 1000:
      print("Balance is between 0 and 1000.")
  ```

## Truthy and Falsy

- A value is considered **truthy** if it evaluates to `True` in a boolean context
- A value is considered **falsy** if it evaluates to `False` in a boolean context
- A value is **falsy** if it is:
  - `False` (boolean)
  - `None` (NoneType)
  - `0` (integer)
  - `0.0` (float)
  - `""` (empty string)
  - `[]` (empty list)
  - Most other empty collections (e.g. empty tuple, empty set, empty dictionary)
- A value is **truthy** if it is:
  - `True` (boolean)
  - All integers other than `0`
  - All floats other than `0.0`
  - All strings other than `""`
  - All collections with at least one element