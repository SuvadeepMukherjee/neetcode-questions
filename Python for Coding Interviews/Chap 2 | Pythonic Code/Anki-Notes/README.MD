Anki Notes : Pythonic Code

**Q1**: What is unpacking in Python ? 

**Solution**:

Assigning multiple variables from a list in one statement

```python
point1 = [0, 0]
point2 = [2, 4]

x1, y1 = point1 # x1 = 0, y1 = 0
x2, y2 = point2 # x2 = 2, y2 = 4

```

**Q2**: Print 0,0,2,4,3,6,5,10 using loop unpacking `points = [[0, 0], [2, 4], [3, 6], [5, 10]]`

**Solution**:

```python
points = [[0, 0], [2, 4], [3, 6], [5, 10]]

for x, y in points:
    print(f"x: {x}, y: {y}")

```

- We can also use unpacking in loops to iterate over a list of lists. This is useful when we know the size of the inner lists and want to unpack them into variables.

**Q3**: What is the Pythonic way to loop over both the index and the value in a list ? 

**Solution**: 

- Use the `enumerate()` function 
  
  ```python
   nums = [2, 7, 9, 2]
  
  for i, n in enumerate(nums):
      print(i, n)
  
  ```

- `enumerate()` returns a tuple of the index and the element

**Q4**: What does `enumerate()` return during iteration ?

**Solution:**

A tuple of the index and the element

```python
 nums = [2, 7, 9, 2]

for i, n in enumerate(nums):
    print(i, n)
```

**Q5**:What does the `zip()` function do in Python ? 

**Solution**: Combines multiple lists into tuples of corresponding elements 

```python
names = ['Alice', 'Bob', 'Charlie', 'David']
scores = [90, 85, 88, 92]

for name, score in zip(names, scores):
    print(f"{name} scored {score}")

```

Time and Space Complexity

- Time Complexity :O(1)
  
  - The `zip()` function returns an iterator at the beginning of the input lists, so it doesn't traverse the entire lists.

- Space complexity: O(1)
  
  - The `zip()` function returns an iterator so it doesn't actually create a new list of tuples in memory.

**Q6:** What is the time and space complexity of calling `zip()` ? 

**Solution**:

- Time Complexity :O(1)
  
  - The `zip()` function returns an iterator at the beginning of the input lists, so it doesn't traverse the entire lists.

- Space complexity: O(1)
  
  - The `zip()` function returns an iterator so it doesn't actually create a new list of tuples in memory.

**Q7**: Convert this code to pythonic code ? 

```python
x = 5

if 0 < x and x < 10:
    print('x is between 0 and 10')

```

**Solution**: 

```python
x = 5

if 0 < x < 10:
    print('x is between 0 and 10')

```

**Q8**: How can you prevent a value from going below a minimum in Python?

**Solution:**

- Use `max(min_value, x)`.

- Example: `transactions = max(0, transactions)` ensures the number never becomes negative. This replaces an `if x < min_value` check.

**Q9:** How can you prevent a value from exceeding a maximum in Python?

**Solution:**



- Use `min(max_value, x)`.

- Example: `transactions = min(100, transactions)` caps the number at 100. This replaces an `if x > max_value` check


