# Strings

## Length Function

- The `len()` function gives us the length of a string

  ```python
  my_str = "NeetCode"
  print(len(my_str))  # Output: 8
  ```

## String Indexing

- If we want to access individual characters from a string , we can do this by indexing the string 

- ```python
  my_str = "Hello"
  print(my_str[0])  # Output: H
  print(my_str[1])  # Output: e
  print(my_str[2])  # Output: l
  print(my_str[3])  # Output: l
  print(my_str[4])  # Output: o
  ```

## String Looping 

- To loop over a string we can use the following technique

- ```python
  my_string = "Hello, World!"
  
  length = len(my_string) # 13
  
  for i in range(length):
      print(my_string[i])
  ```

## String Looping Shorthand 

- If we don't explicitly need the index , we can use a shorthand to loop through each character in the string

- ```python
  my_string = "Hello"
  
  for char in my_string:
      print(char)
  ```

## String Concatenation

- concatenation is the process of combining two or more strings into a single string .Python provides the `+` operator for concatenating strings 
- when we use the `+` operator with two strings ,Python joins them together to create a new string

## String Slicing

- Slicing allows us to extract a substring by specifying a range of indices

- In the below example we are extracting the substring from index 1 to 5 (not including 5) from the string `"Hello, World!"`

  ```python
  my_string = "Hello, World!"
  
  start, end = 1, 5
  
  print(my_string[start:end])  # Output: ello
  ```

- If we don't specify the start , it's equivalent to starting from the beginning of the string

  ```python
  my_string = "NeetCode"
  
  print(my_string[:3])  # Output: Nee
  ```

- If we don't specify the end, it's equivalent to ending at the end of the string.

- ```python
  my_string = "NeetCode"
  
  print(my_string[4:])  # Output: Code
  ```

- If we don't specify either , we get the entire string

- ```python
  my_string = "NeetCode"
  
  print(my_string[:])  # Output: NeetCode
  print(my_string)     # Output: NeetCode
  ```

## Reversing a String

- By not specifying the starting index or the ending index, and setting the step to -1, the string will be reversed.

  

  ```python
  my_string = "Hello"
  
  print(my_string[::-1])  # Output: olleH
  ```

## Strings are Immutable

- We  are creating a new string with the sliced character .This is because strings are immutable in Python , which means they cannot be changed after they are created 

## String Formatting

- f-strings

  - These are prefixed with an `f` before the string and allow you to insert variables directly into the string. 

    ```python
    name = "Alice"
    age = 25
    
    msg = f"Hello, {name}. You are {age} years old."
    ```