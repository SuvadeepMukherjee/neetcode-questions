# Lists 

## Intro to Lists

- a list is a collection of items that are stored in a specific order 

- We can access individual elements in the list by **indexing** it 

- We can also get the number of elements within the list by calling the `len()` function

  ```
  my_list = [1, 2, 3]
  
  print(len(my_list))  # Output: 3
  
  print(my_list[0])  # Output: 1
  print(my_list[1])  # Output: 2
  print(my_list[2])  # Output: 3
  ```

- Lists are **mutable**, meaning we can change the values of the elements in the list.
- Lists can store everything and we can even mix and match different types of elements in a list

## List Operations

- Lists can be used within conditional statements . For example we can check if a list is empty or not 

  ```python
  my_list = [1, 2, 3]
  
  if len(my_list) > 0:
      print("The list is not empty")
  else:
      print("The list is empty")
  
  if my_list:
      print("The list is not empty")
  else:
      print("The list is empty")
  ```

- We can also use the `in` operator to check if an element is present in a list 

- ```python
  my_list = [1, 2, 3]
  
  if 2 in my_list:
      print("2 is in the list")
  else:
      print("2 is not in the list")
  ```

- If we want to check if an element is not in the list , we can use the `not in` operator 

- ```python
  my_list = [1, 2, 3]
  
  if 4 not in my_list:
      print("4 is not in the list")
  else:
      print("4 is in the list")
  ```

    

## List Looping 

- We can loop through list the following ways 

  - By using the length of the list

    ```python
    my_list = [1, 2, 3, 4, 5]
    
    length = len(my_list)
    
    for i in range(length):
        print(my_list[i])
    ```

  - By using the `in` operator

    ```python
    my_list = [1, 2, 3, 4, 5]
    
    for element in my_list:
        print(element)
    ```

  - Note ➡️ If we dont need the index of the element the second method is preferred since it is more concise  

## List Functions

- Python also provides some built in functions to get the sum , minimum and maximum of a list 

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  print(sum(my_list))  # Output: 15
  print(min(my_list))  # Output: 1
  print(max(my_list))  # Output: 5
  ```

## List Append

- We can add new elements to the end of a list using the `append()` function 

  ```python
  my_list = [1, 2, 3]
  
  print(my_list)  # Output: [1, 2, 3]
  
  my_list.append(4)
  
  print(my_list)  # Output: [1, 2, 3, 4]
  ```

## List Pop 

- We can remove elements from a list using the `pop()` function 

  ```python
  my_list = [1, 2, 3]
  
  my_list.pop()
  
  print(my_list)  # Output: [1, 2]
  ```

- By default, `pop()` removes the last element from the list. We can also specify an index to remove a specific element, as shown below.

  ```python
  my_list = [1, 2, 3]
  
  my_list.pop(0)
  
  print(my_list)  # Output: [2, 3]
  
  my_list.pop(0)
  
  print(my_list)  # Output: [3]
  ```

## List Find

- The `index()` function will print the index of the first occurence of an element in the list 

- ```python
  my_list = [1, 2, 3, 4, 5, 3]
  
  print(my_list.index(3))  # Output: 2
  ```

## List Slicing

- To review, we can get a portion of the list by specifying the start and end index. If we omit the start index, it will default to the beginning of the list. If we omit the end index, it will default to the end of the list. We can also specify a negative step, after two colons, to reverse the list.

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  print(my_list[1:3])  # Output: [2, 3]
  
  print(my_list[:3])   # Output: [1, 2, 3]
  
  print(my_list[2:])   # Output: [3, 4, 5]
  
  print(my_list[::-1]) # Output: [5, 4, 3, 2, 1]
  ```

- none of these operations modify the original list. They only return a new list with the specified slice.

- Using `-1` to access an element in a list will give us the last element, `-2` will give us the second-to-last element, and so on. 

- ```python
  my_list = [1, 2, 3, 4, 5]
  
  print(my_list[-1]) # Output: 5
  print(my_list[-2]) # Output: 4
  print(my_list[-3]) # Output: 3
  ```

## Tuples

- Tuples are very similar to lists , but thy have one key difference : they are immutable . This means that once a tuple is created , it cannot be changed 

- We can create a tuple by using parentheses instead of square brackets 

- ```python
  my_tuple = (4, 5, 6)
  
  print(my_tuple)  # Output: (4, 5, 6)
  ```

- We can index a tuple  just like a list:

- ```python
  my_tuple = (4, 5, 6)
  
  print(my_tuple[0])  # Output: 4
  print(my_tuple[1])  # Output: 5
  print(my_tuple[2])  # Output: 6
  ```

- We can slice a tuple just like a list, slicing a tuple doesn't modify it , instead it creates a new tuple with the specified slice

  ```python
  my_tuple = (4, 5, 6)
  
  print(my_tuple[1:])  # Output: (5, 6)
  ```

- We can't modify a tuple, the following code will raise an error:

- ```python
  my_tuple = (4, 5, 6)
  
  my_tuple[0] = 1 # Raises an error
  ```

- We also can't call `append` or `pop` on a tuple, since these functions would modify it. We can however still call `sum()`, `max()`, and `min()` on a tuple, since these functions don't modify the tuple.