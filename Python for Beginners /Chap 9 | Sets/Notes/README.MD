# Sets

## Intro to Sets

In Python, a **set** is very similar to a list, but with a few key differences.

- A set is unordered , meaning the elements are not stored in a specific order. If order is important, you should use a list.

- A set can only contain *unique* elements. If you try to add a duplicate element to a set, it will be ignored.

  ```python
  my_set = {1, 2, 3}
  
  print(my_set)  # Output: {1, 2, 3}
  
  my_set = {3, 2, 1}
  
  print(my_set)  # Output: {1, 2, 3}
  ```

- A set can be created using curly braces `{}` with elements separated by commas. When printing a set, the elements sometimes appear in sorted order, but this is *not* guaranteed. A `set` makes no gurantees about the order of the elements stored.

- We declared an empty set with `set()`. We then added the elements `1` and `2` to the set. When we tried to add `1` again, it was ignored because it was already in the set. This is because sets can *not* contain duplicate elements.

  ```python
  my_set = set()
  
  my_set.add(1)
  my_set.add(2)
  my_set.add(1)
  
  print(my_set)  # Output: {1, 2}
  ```

Note ➡️ We cannot declare an empty set with curly braces . If we used empty curly braces `{}`, it would **not** have declared a set. That's because Python uses curly braces to declare an empty dictionary. A dictionary is a data structure that stores key-value pairs.

## Set Operations

- Removing elements 

  - To remove elements from a set we use the `remove()` function .If the element is not present in the set a `KeyError` will be raised 

    ```python
    my_set = {1, 2, 3}
    
    my_set.remove(2)
    
    print(my_set)  # Output: {1, 3}
    
    my_set.remove(4)  # Raises KeyError
    ```

- Looping

  - we can loop over elements within a set using `for` loops. The difference is that we can't access elements by index because sets are unordered. The order that we loop over a set is not guaranteed.

    ```python
    my_set = {1, 2, 3}
    
    for element in my_set:
        print(element)
    ```

- How to remove duplicates from a list using set ?

  - We can also convert a list into a set by passing the list into the `set()` function. We can then convert the set back into a list by passing it into the `list()` function. This is an easy way to remove duplicates from a list.

    

    ```python
    my_list = [1, 2, 3, 4, 5, 1, 2, 5]
    
    my_set = set(my_list)
    
    print(my_set)  # Output: {1, 2, 3, 4, 5}
    
    my_list_no_duplicates = list(my_set)
    ```

- How to check whether an element is present in a set ? 

  - we can  use the `in` keyword to check if an element is present in a set.

    ```python
    my_set = {"Cat", "Dog", "Mouse"}
    
    contains_cat = "Cat" in my_set   # True
    contains_lion = "Lion" in my_set # False
    ```