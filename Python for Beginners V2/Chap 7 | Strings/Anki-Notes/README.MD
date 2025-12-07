# Strings (Anki Notes)

**Q1**: What does the `len()` function return for a string ? 

**Solution**:

The number of characters in the string

Example: `len("NeetCode")` → 8.

**Q2**: How do you access individual characters in a Python string ? 

**Solution**:

By indexing the string with square brackets

Example: `"Hello"[0]` → `H`, `"Hello"[4]` → `o`.

**Q3**: What are the two ways to loop over characters in a string in Python ? 

**Solution**:

Loop by index or loop directly over characters.

Index method: `for i in range(len(s))`; shorthand: `for char in s`.

```python
my_string = "Hello, World!"

length = len(my_string) # 13

for i in range(length):
    print(my_string[i])
```

```python
my_string = "Hello"

for char in my_string:
    print(char)
```

**Q4**: What happens when you concatenate strings in Python ? 

**Solution**:

A completely new string is created.

Strings are immutable, so `"a" + "b"` builds a new string — the originals are unchanged.

**Q5**: How does slicing work on strings in Python ? 

**Solution**:

It extracts a substring using `string[start:end]`.

Omitting `start` begins at the start; omitting `end` goes to the end; omitting both returns the entire string (e.g., `s[:]`).

**Q6**: How can we reverse a string ? 

**Solution**:

- By not specifying the starting index or the ending index, and setting the step to -1, the string will be reversed.

  ```python
  my_string = "Hello"
  
  print(my_string[::-1])  # Output: olleH
  ```

**Q7**: Why does slicing or modifying part of a string create a new string in Python?

**Solution**:

- Because strings are immutable.
- Once created, a string cannot be changed — any “modification” produces a brand-new string.

**Q8**: What are f-strings used for in Python ? 

**Solution**:

Inserting variables directly into a string using `f"..."`.

```python
name = "Alice"
age = 25

msg = f"Hello, {name}. You are {age} years old."
```

