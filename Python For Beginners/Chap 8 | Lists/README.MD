# Lists

## Intro to Lists

- **list** is a collection of items that are stored in a specific order.
- we can access individual elements in the list by **indexing** it just like with a string
- We can also get the number of elements within the list by calling the `len()` function.
- Lists are **mutable**, meaning we can change the values of the elements in the list.
- Lists can also store more than just numbers, they can store everything from strings to other lists.
- We can even mix and match different types of elements in a list. This is generally not recommended, but it is possible.

## List Operations

- Lists can also be used within conditional statements. For example, we can check if a list is empty or not:

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

- The above two conditional statements are equivalent. The second one is more concise and is generally preferred.

- We can also use the `in` operator to check if an element is present in a list:

- ```python
  my_list = [1, 2, 3]
  
  if 2 in my_list:
      print("2 is in the list")
  else:
      print("2 is not in the list")
  ```

- If we want to check if an element is not in the list, we can use the `not in` operator:

- ```python
  my_list = [1, 2, 3]
  
  if 4 not in my_list:
      print("4 is not in the list")
  else:
      print("4 is in the list")
  ```

## List Looping

- We can also loop through lists similar to how we loop through strings 

- By using the length of the list 

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  length = len(my_list)
  
  for i in range(length):
      print(my_list[i])
  ```

- Or by using the `in` operator:

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  for element in my_list:
      print(element)
  ```

- Both of these methods will print each element of the list on a separate line. If we don't need the index of the element, the second method is generally preferred since it is more concise.

## List Functions

- Python also provides some built in functions to get the sum, minimum, and maximum of a list:

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  print(sum(my_list))  # Output: 15
  print(min(my_list))  # Output: 1
  print(max(my_list))  # Output: 5
  ```

- The `sum()` function returns the sum of all the elements in the list.
- The `min()` function returns the smallest element in the list.
- The `max()` function returns the largest element in the list.

## List Append

- We can also add new elements to the end of a list using the `append()` function.

  ```python
  my_list = [1, 2, 3]
  
  print(my_list)  # Output: [1, 2, 3]
  
  my_list.append(4)
  
  print(my_list)  # Output: [1, 2, 3, 4]
  ```

## List Pop

- We can also remove elements from a list using the `pop()` function

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

- Notice that we called `pop(0)` twice to remove the first two elements from the list. After removing the first element, the second element becomes the first element. So we call `pop(0)` again to remove the new first element.

## List Find

- We can also find the index of an element in a list using the `index()` function.

  ```python
  my_list = [1, 2, 3, 4, 5, 3]
  
  print(my_list.index(3))  # Output: 2
  ```

- The above code snippet will print the index of the first occurence of the element `3` in the list `my_list`. There are two `3`s in the list, but the first one is at index `2`, so `2` is printed. If the element is not present in the list, a `ValueError` will be raised.

