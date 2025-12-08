# Lists

## Resizable Lists

- Some languages have both fixed-size arrays and resizable arrays. In Python, we only have resizable arrays, which are referred to as lists in Python

- The common operations on a list include:
  
  - `append()` : adds an element to the end of the list
  
  - `pop()`: Removes and returns the last element of the list.
    
    - If the list is already empty, we will get an `IndexError`.
    - We can also pass an integer to `pop()` to remove an element at a specific index.
    - If we `pop(index)` an index that is out of bounds, we will get an `IndexError`.
  
  - `insert()`: Inserts an element at a specified index in the list.
    
    - If the index is too large, the element will be inserted at the end of the list.
    
    - If the index is negative, the element will be inserted at the beginning of the list.

- Here are examples of each:
  
  ```python
  my_list = [1, 2, 3]
  
  my_list.append(4) # [1, 2, 3, 4]
  my_list.append(5) # [1, 2, 3, 4, 5]
  
  my_list.pop() # [1, 2, 3, 4]
  
  my_list.insert(1, 3) # [1, 3, 2, 3, 4]
  ```

- Time Complexity 
  
  - `append()`
    
    - Time complexity: O(1)
  
  - `pop()`.
    
    -     Time complexity: O(1)
  
  - `insert()`.
    
    - Time complexity: O(n), where n is the number of elements in the list.

- These list operations are less common , but they are absolutely worth knowing:
  
  - `index()`: Returns the index of the first occurrence of a specified element in the list.
    
    - If the element is not in the list, we will get an `ValueError`.
  
  - `remove()`: Removes the first occurrence of a specified element from the list.
  
  - `extend()`: Adds the elements of another list to the end of the list.

- Here are examples of each:
  
  ```python
  my_list = [1, 3, 2, 3]
  
  my_list.index(3) # 1
  
  my_list.remove(3) # [1, 2, 3]
  
  my_list.extend([4, 5]) # [1, 2, 3, 4, 5]
  ```

- If we want to check if an element is in a list, we can use the `in` operator. This is preferable to using `index()` unless we actually need the index of the element.
  
  ```python
  my_list = [1, 2, 3]
  
  if 3 in my_list:
      print("3 is in the list")
  ```

- Time Complexity 
  
  - `index()`
    - Time complexity: O(n), where n is the length of the list.
  - remove 
    - Time Complexity : O(n) , where n is the length of the list
  - extend()
    - Time Complexity :O(m) , where m is the length of the list passed to `extend()`
  - `in` operator on a list 
    - Time complexity: O(n), where n is the length of the list.

## List Concat

- Instead of using the `extend()` method there's an even easier way to concatenate two lists in Python. We can use the `+` operator

-   The only difference between this and the `extend()` method is that the `+` operator creates a new list, while the `extend()` method modifies the original list.

-   Time complexity: O(n+m) where n is the length of one list and m is the length of the other list.
  
  ```python
  list1 = [1, 2, 3]
  list2 = [4, 5, 6]
  
  result = list1 + list2 # [1, 2, 3, 4, 5, 6]
  ```

## List Initialization

- The above code will create a list of 5 0s
  
  ```python
  my_list = [0] * 5
  ```

- The above code will create a list of 5 1s 
  
  ```python
  my_list = [1] * 3
  ```

- Time Complexity
  
  - O(n) where n is the size of the resulting list.

## List Clone

- Using the slice method
  
  ```python
  original_list = [1, 2, 3]
  cloned_list = original_list[:]
  ```
  
  - Keep in mind, that if you have a list of objects, the above methods will not create [deep copies](https://developer.mozilla.org/en-US/docs/Glossary/Deep_copy) of the elements within the list. In this case we have a list of integers, which are primitive types, so we don't need to worry about that. But if you had a list of lists, for example, you would need to use the `copy.deepcopy()` method to create a deep copy.

- Using deepcopy method
  
  ```python
  import copy
  
  original_list = [[1, 2], [3, 4]]
  
  cloned_list = copy.deepcopy(original_list)
  ```

- Time Complexity : O(n) where n is the length of the list being copied.

## List Comprehension

- List Comprehension allows us to create lists in a concise way 

```python
my_list = [i for i in range(5)]

print(my_list) # [0, 1, 2, 3, 4]
```

- This is called **list comprehension**. In the above example, we have a `for` loop inside the square brackets. The loop iterates over the range of numbers from `0` to `4`. Before the loop we place the expression `i` which is the value we want to add to the list. This is a very concise way to create a list.

```python
arr1 = [1, 2, 3]
arr2 = [4, 5, 6]

result = [i + j for i, j in zip(arr1, arr2)]
```

- Above we have two lists `arr1` and `arr2`. We use the `zip()` function to iterate over both lists at the same time. We then add the elements of both lists together and create a new list. The expression `i + j` is the value we want to add to the list.

```python
arr = [1, 2, 3, 4, 5]

result = [i for i in arr if i % 2 == 0]
```

- In the above example, we have a list `arr`. We iterate over the list and add the element to the new list only if it's even

- Time Complexity : O(n) where n is the number of times the loop within the list comprehension runs.
