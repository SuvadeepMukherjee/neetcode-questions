# Loops

## While Loops

```python
i = 0
while i < 5:
    print("I love Python!")
    i += 1
```

## For Loops

- to print the numbers 0 through 9 we can use a  for loop

  ```python
  for i in range(10):
      print(i)
  ```

- to print the numbers 2 through 4 we use the following syntax

  ```python
  for i in range(2, 5):
      print(i)
  ```

  - the first parameter to the `range()` function is the starting number, and the second parameter is the ending number. The ending number is not included in the sequence

- to print the numbers 0 , 2 , 4 , 6 , 8 we use the following syntax

- ```python
  for i in range(0, 10, 2):
      print(i)
  ```

  - The `0` passed into the `range()` function is the starting number.
  - The `10` passed into the `range()` function is the ending number. The loop will **stop** once it reaches or exceeds this number. Meaning that the number `10` is not included in the sequence.
  - The `2` passed into the `range()` function is the step. This is how much the variable will increment by on each iteration of the loop.

- to print a number in reverse order we can also use a for loop 

  ```python
  for i in range(10, 0, -1):
      print(i) 
  ```

## Nested Loops

- Suppose we wanted to print all possible pairs from the following set of integers `1, 2, 3`, where the order of the pairs matters. This would look like:

- |      |      |      |
  | :--- | :--- | :--- |
  | 1,1  | 1,2  | 1,3  |
  | 2,1  | 2,2  | 2,3  |
  | 3,1  | 3,2  | 3,3  |

- This can be accomplished by placing a loop inside of another loop. This is called a **nested loop**.

  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(i, j)
  ```

## Control Flow

- Python provides control statements to alter the execution of loops.

  - `break`: Exits the loop immediately.

  - `continue`: Skips the remaining code inside the loop for the current iteration and moves to the next iteration.

  - `pass`: Acts as a placeholder and does nothing. We cannot have empty loops, so we use `pass` to avoid errors. It can also be used in conditional statements and functions.

  - Here's an example demonstrating `pass`:

    ```python
    for i in range(1, 8):
        pass
    
    if True:
        pass
    
    def unfinsished_function():
        pass
    ```