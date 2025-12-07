# Reading Stdin

## Reading Input

- The `input()` function is used to read input to the program while the program is running. This input comes from a stream of data called *standard input* or *stdin*. This can either mean the data a user types in manually into the terminal (console) or input that is supplied to the program before it is run.

  ```python
  user_input = input("Enter some text: ") 
  
  print(user_input) # This will print the input to the console
  ```

## Type Conversion with Input

- By default, `input()` returns the user input as a *string*. If you're expecting a different type of input like an *integer* or a *float*, you need to explicitly convert it using `int()` or `float()`.

- ```python
  age = int(input("Enter your age: "))
  
  temperature = float(input("Enter the temperature: "))
  ```

## Parse Input

- Sometimes we have to do more than just convert the input to a single type. We might need to restructure the input in some way. This is called **parsing** the input.

- Suppose you read a list of integers separated by commas into a string, but you want to store them as a list. You can use the `split()` method to split the string by commas. This will convert "1,2,3" into a list of strings `["1", "2", "3"]`.

  ```python
  number_string = "1,2,3"
  
  string_list = number_string.split(",")
  
  print(string_list) # Output: ['1', '2', '3']
  ```