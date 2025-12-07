# Anki Notes : Lists

**Q1**: What is mutability ? 

**Solution**: mutable means we can change it 

**Q2**: Are Lists mutable in Python ? 

**Solution**:Lists are mutable in Python

**Q3**: How can we check if a list is empty or not ? 

**Solution**: We can check if a list is empty or not using the following wayif 

```python
my_list = [1, 2, 3]

my_list:
    print("The list is not empty")
else:
    print("The list is empty")
```

**Q4**: How can we check if an element is present in a list ? 

**Solution**:

We can check if an element is present in a list using the `in` operator 

```python
my_list = [1, 2, 3]

if 2 in my_list:
    print("2 is in the list")
else:
    print("2 is not in the list")
```

**Q5**: How can we check if an element is not in the list ? 

**Solution**:

If we want to check if an element is not in the list we can use the `not in` operator 

```python
my_list = [1, 2, 3]

if 4 not in my_list:
    print("4 is not in the list")
else:
    print("4 is in the list")
```

**Q6**: How can we loop through a list of? 

**Solution**:

We can loop through a list in the following ways 

- By using the length of the list

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  length = len(my_list)
  
  for i in range(length):
      print(my_list[i])
  ```

- By using the in operator 

  ```python
  my_list = [1, 2, 3, 4, 5]
  
  for element in my_list:
      print(element)
  ```

Note ➡️ If we dont need the index of the element the second method is preferred since it is more concise  

**Q7**: How can we get the sum , minimum and maximum of a list ? 

**Solution**:

We can get the sum , minimum and maximum of a list in the following way 

```python
my_list = [1, 2, 3, 4, 5]

print(sum(my_list))  # Output: 15
print(min(my_list))  # Output: 1
print(max(my_list))  # Output: 5
```

**Q8**: How can we add an element to the end of a list ? 

**Solution**:

We can add a new element to the end of a list using the `append()` function 

```python
my_list = [1, 2, 3]

print(my_list)  # Output: [1, 2, 3]

my_list.append(4)

print(my_list)  # Output: [1, 2, 3, 4]
```

**Q9**: Answer the following questions about pop()

- What does `pop()` do to a list?
- Which element does `pop()` remove by default?
- How do you remove a specific element using `pop()`?

**Solution**:

- Removes an element from the list.
- The last element.
- Pass an index to `pop()`.

```python
my_list = [1, 2, 3]

my_list.pop()

print(my_list)  # Output: [1, 2]
```

```python
my_list = [1, 2, 3]

my_list.pop(0)

print(my_list)  # Output: [2, 3]

my_list.pop(0)

print(my_list)  # Output: [3]
```

**Q10**: What does the index() function do in a list ? 

**Solution**:

Returns the index of the first occurrence of a given element.

```python
my_list = [1, 2, 3, 4, 5, 3]

print(my_list.index(3))  # Output: 2
```

**Q11**:What is the basic syntax of list slicing?

**Solution**:

`list[start:end:step]`

```python
my_list = [1, 2, 3, 4, 5]

print(my_list[1:3])  # Output: [2, 3]

print(my_list[:3])   # Output: [1, 2, 3]

print(my_list[2:])   # Output: [3, 4, 5]

print(my_list[::-1]) # Output: [5, 4, 3, 2, 1]
```

To review, we can get a portion of the list by specifying the start and end index. If we omit the start index, it will default to the beginning of the list. If we omit the end index, it will default to the end of the list. We can also specify a negative step, after two colons, to reverse the list.

**Q12**: Does slicing modify the list ? 

**Solution**:

slicing does not  modify the original list. It only returns a new list with the specified slice.

**Q13**: What does an index of `-1` ,`-2`access in a list?

**Solution**:

the last element , the second last element

**Q14**:What is the key difference between tuples and lists ? 

**Solution**:

Tuples are immutable 

**Q15**: How do you create a tuple ? 

**Solution**:

By using parentheses

```python
 my_tuple = (4, 5, 6)

print(my_tuple)  # Output: (4, 5, 6)
```

**Q16**: Can a tuple be modified after creation ? 

**Solution**: 

No - any change attempt causes an error 

**Q17**:Can you index and slice a tuple like a list ? 

**Solution**:

Yes

**Q18**: Why can't tuples use methods like `append()` or `pop()` ? 

**Solution**:

Because those methods modify the data 

**Q19**: Can we use methods like `sum()` , `max()` and `min()` on a tuple ? 

**Solution**:

We can use methods like `sum()` , `max()` and `min()` on a tuple since these functions don't modify the tuple 