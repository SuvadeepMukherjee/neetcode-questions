# Dictionaries

## Intro to Dictionaries

- Dictionaries are used to store key-value pairs (table with 2 columns , the first column is the key and the second column is the value)

  ```python
  my_dict = {"Alice": 25, "Bob": 30, "Charlie": 35}
  
  my_dict = {
      "Alice": 25,
      "Bob": 30,
      "Charlie": 35
  }
  ```

- To declare an empty directory we can use empty curly braces `{}` We can then add key-value pairs to the dictionary using square brackets `[]` and the assignment operator `=`.

- ```python
  my_dict = {}
  
  my_dict["Alice"] = 25
  my_dict["Bob"] = 30
  my_dict["Charlie"] = 35
  ```

## Dict Operations

- The keys within a dictionary must be unique, but the values can be duplicated.

- If we assign the same key a new value , the old value is overwritten 

  ```python
  my_dict = {"a": 1, "b": 2, "c": 3}
  
  print(my_dict["a"]) # Output: 1
  
  my_dict["a"] = 4
  
  print(my_dict["a"]) # Output: 4
  ```

- The values within a dictionary can be of any type including lists , sets and even other dictionaries 

- ```python
  my_dict = {"a": [1, 2, 3], "b": {4, 5, 6}, "c": {"x": 7, "y": 8, "z": 9}}
  
  print(my_dict["a"]) # Output: [1, 2, 3]
  print(my_dict["b"]) # Output: {4, 5, 6}
  print(my_dict["c"]) # Output: {"x": 7, "y": 8, "z": 9}
  ```

- To check if a dictionary conatins a key , we can use the `in` keyword 

- ```python
  my_dict = {"a": 1, "b": 2, "c": 3}
  
  print("a" in my_dict) # Output: True
  print("d" in my_dict) # Output: False
  ```

- In Python 3.7 and later , dictionaries are ordered by the order in which they were inserted ,This means that the order of key-value pairs in a dictionary is preserved 

## Dict Looping

-  We can use the `len()` function to get the length of a dictionary.This will return the number of key-value pairs in the dictionary 

  ```python
  my_dict = {"a": 1, "b": 2, "c": 3}
  
  print(len(my_dict)) # Output: 3
  ```

-   To Loop over a dict we can use the following 2 methods 

  - Method 1 : 

    - ```python
      my_dict = {"a": 1, "b": 2, "c": 3}
      
      for key in my_dict:
          value = my_dict[key]
          print(key, value)
      ```

  - Method 2: 

    - ```python
      my_dict = {"a": 1, "b": 2, "c": 3}
      
      for key, value in my_dict.items():
          print(key, value)
      ```

    - With `items()` you need to have two variables to unpack the key-value pair. The first will be the key, and the second will be the value

## Dict Practise

**Q**: Given a list `[1, 2, 3, 1, 2, 3, 1, 2, 3]`, count the quantity of each element in the list using a dictionary.The result would be a dictionary like this : 

```python
count = {
    1: 3,
    2: 3,
    3: 3
}
```

**Solution**:

```python
from typing import Dict # this adds type hinting for Dict

def count_characters(word: str) -> Dict[str, int]:
	count ={}
    for char in word:
      if char not in count:
					count[char]= 1
        else:
          count[char]+=1
      return count
```

## Dict Remove

- pop() function 

  - We can remove an item from a dictionary using the `pop()` function. This function takes a key as an argument and removes the key-value pair from the dictionary. If the key doesn't exist, it will raise a `KeyError`.

  - ```python
    my_dict = {"a": 1, "b": 2, "c": 3}
    
    my_dict.pop("a")
    
    print(my_dict) # Output: {"b": 2, "c": 3}
    
    my_dict.pop("d") # Raises KeyError
    ```

  - If we don't want to worry about handling the `KeyError`, you can use the second argument of the `pop()` function. This argument is the default value that will be returned if the key doesn't exist.

  - ```python
    my_dict = {"a": 1, "b": 2, "c": 3}
    
    value = my_dict.pop("d", 0) # Returns 0, no error occurs
    ```

- `del` keyword

  - We can also use the `del` keyword to remove a key-value pair from a dictionary. This is a bit more concise than using the `pop()` function.

    ```python
    my_dict = {"a": 1, "b": 2, "c": 3}
    
    del my_dict["a"]
    ```

## Dict Values

- Loop over the values in a dictionary without needing to access the keys 

- ```python
  my_dict = {"a": 1, "b": 2, "c": 3}
  
  for value in my_dict.values():
      print(value)
  ```

- Convert the values of a dictionary into a list.This can be done by using the `list()` function

  ```python
  my_dict = {"a": 1, "b": 2, "c": 3}
  
  values = list(my_dict.values())
  
  print(values) # Output: [1, 2, 3]
  ```