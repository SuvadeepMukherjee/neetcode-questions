lists (anki)

**Q1**: What does `append() ` do and what is its Time Complexity ? 

**Solution:**

- `append()` : adds an element to the end of the list

- Time Complexity :O(1)



**Q2**: What does `pop()` do in a list ? 

**Solution**: 

- Removes and returns the last element

- If the list is empty, calling `pop()` raises an `IndexError`.



**Q3**: How do you remove an element at a specific index using `pop()` ? 

**Solution:**

- Pass the index to `pop(index)`.

- Popping an out-of-bounds index also raises an `IndexError`.

**Q4**: What is the Time Complexity of the `pop()` operation in python ? 

**Solution**:

Time Complexity :O(1)

**Q5**: What does the `insert()` method do in a Python list ? 

**Solution:**

- Inserts an element at a specified index.

- If the index is too large, the element is added at the **end**if the index is negative, it is added at the **beginning**.

**Q6:** What is the Time Compexity of `insert()` method in Python ? 

**Solution:**

Time complexity: O(n), where n is the number of elements in the list.
