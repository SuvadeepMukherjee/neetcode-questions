# Math

## Arithmatic Operators

- If we divide `y` by `x`, the result will be `2.0` and *not* `2`. This is because the result of division is always a float in Python.
- For the arithmetic operators (like addition ,substraction , multiplication) the result will be an integer if both operands are integers. If one of the operands is a float, the result will be a float.

## More Operators

- Floor Division

  - Divides the first operand by the second and rounds down the result to an integer.

    ```python
    x, y = 7, 2
    
    print(x // y) # Output: 3  (7 divided by 2 is 3.5, after rounding down we get 3)
    ```

- Modulas 

  - Returns the remainder of the division of the first operand by the second

  - ```python
    print(x % y)  # Output: 1  (7 divided by 2 is 3, with a remainder of 1)
    ```

- Exponention

  - Raises the first operand to the power of the second operand.

    ```python
    print(x ** y) # Output: 49 (7 raised to the power of 2 is 49, 7*7 = 49)
    ```

## Shorthand Operators

- `+=` is shorthand for `count = count +`

- `-=` is shorthand for `count = count -`
- `*=` is shorthand for `count = count *`
- `/=` is shorthand for `count = count /`
- `%=` is shorthand for `count = count %`
- `//=` is shorthand for `count = count //`
- `**=` is shorthand for `count = count **`

## Boolean OR

- The OR operation returns `True`  if at least one of the operands is `True`

## Boolean and 

- The `and` operation returns `True` if all the operands are `True`

## Boolean and 

- It simply inverts the value of the operand. If the operand is `True`, the result is `False`. If the operand is `False`, the result is `True`.

  

  ```python
  a = True
  b = False
  print(not a)  # Output: False
  print(not b)  # Output: True
  ```