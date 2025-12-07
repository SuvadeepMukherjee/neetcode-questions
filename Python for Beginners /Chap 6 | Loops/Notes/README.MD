# Loops

## While Loops

- We can print `I love Python!` using while loops the following way

  ```python
  i = 0
  while i < 5:
      print("I love Python!")
      i += 1
  ```

## For Loops

- To print from 0 to 9 we can use a for loop ,the syntax is given below

  ```python
  for i in range(10):
      print(i)
  ```

- To print from 2 to 4 we can use the following syntax

  ```python
  for i in range(2, 5):
      print(i)
  ```

- To print `0`,`2`,`4`,`6` and `8` we can use a for loop in this way 

- ```python
  for i in range(0, 10, 2):
      print(i)
  ```

- To print from 10 to 1 we can use a negative step 

- ```python
  for i in range(10, 0, -1):
      print(i)
  ```

## Nested Loops 

- To print Nested loops we can use 2 for loops

  ```python
  for i in range(1, 4):
      for j in range(1, 4):
          print(i, j)
  ```

- This will print 

- ```plaintext
  1 1
  1 2
  1 3
  2 1
  2 2
  2 3
  3 1
  3 2
  3 3
  ```

## Control Flow 

- Python provides control statements to alter the execution of loops.

  - `break`: Exits the loop immediately.

  - `continue`: Skips the remaining code inside the loop for the current iteration and moves to the next iteration.

  - `pass`: Acts as a placeholder and does nothing. We cannot have empty loops, so we use `pass` to avoid errors. It can also be used in conditional statements and functions.

    ```python
    for i in range(1, 8):
        pass
    
    if True:
        pass
    
    def unfinsished_function():
        pass
    ```