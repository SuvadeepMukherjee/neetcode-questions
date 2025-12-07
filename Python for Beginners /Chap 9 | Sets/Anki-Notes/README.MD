# Sets - Anki Notes

**Q1**: Is a set unordered ? 

**Solution**
A set is unordered , meaning the elements are not stored in a specific order 

**Q2**: Can a set have duplicate elements ? 

**Solution**:

a set cannot have duplicate elements , if we try to add a duplicate element to a set it will be ignored 

**Q3**: Does a set gurantee about the order of elements stored ? 

**Solution**:

When printing a set, the elements sometimes appear in sorted order, but this is *not* guaranteed. A `set` makes no gurantees about the order of the 

```python
my_set = {1, 2, 3}

print(my_set)  # Output: {1, 2, 3}

my_set = {3, 2, 1}

print(my_set)  # Output: {1, 2, 3}
```

**Q4**: How to declare an empty set and a non-empty set ? 

**Solution**:

```python
my_set = {1, 2, 3}

my_second_set = set()
```

Note ➡️ We cannot declare an empty set with curly braces . If we used empty curly braces `{}`, it would **not** have declared a set. That's because Python uses curly braces to declare an empty dictionary. A dictionary is a data structure that stores key-value pairs.

**Q5**: How to add an element to a set ? 

**Solution**:

we use the `add()` method to add elements to a set

```python
my_set = set()

my_set.add(1)
my_set.add(2)
my_set.add(1)

print(my_set)  # Output: {1, 2}
```

**Q6**: Which function removes an element from a set ? 

**Solution**:

`remove()`

It raises a `KeyError` if the element doesn’t exist.

```python
my_set = {1, 2, 3}

my_set.remove(2)

print(my_set)  # Output: {1, 3}

my_set.remove(4)  # Raises KeyError
```

**Q7**: What happens if you call `remove()` on a value not in the set?

**Solution**:

A `KeyError` is raised.

```python
my_set = {1, 2, 3}

my_set.remove(2)

print(my_set)  # Output: {1, 3}

my_set.remove(4)  # Raises KeyError
```

**Q8**: How to loop over a set ? 

**Solution**:

```python
my_set = {1, 2, 3}

for element in my_set:
    print(element)
```

Note ➡️ we can't access elements by index because sets are unordered. The order that we loop over a set is not guaranteed.

**Q9**: How to remove duplicates from a set ? 

**Solution**:

- Convert the list to a set with `set()`.
- Then convert back to a list with `list()` to keep only unique values.

```python
my_list = [1, 2, 3, 4, 5, 1, 2, 5]

my_set = set(my_list)

print(my_set)  # Output: {1, 2, 3, 4, 5}

my_list_no_duplicates = list(my_set)
```

**Q10**: How do we check if an element exists in a set ? 

**Solution**:

Use the `in` keyword 

```python
my_set = {"Cat", "Dog", "Mouse"}

contains_cat = "Cat" in my_set   # True
contains_lion = "Lion" in my_set # False
```

