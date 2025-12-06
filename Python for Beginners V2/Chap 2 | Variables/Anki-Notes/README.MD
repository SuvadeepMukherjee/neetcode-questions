# Variables(Anki Notes)

Anki Tag ➡️ 02-variables

**Q1**: How we do multiple assignment in Python ? 

**Solution**:

```python
msg1, msg2 = "Hello", "World"
```

**Q2**: How do we swap two variables in Python without a temp variable ? 

**Solution**:

Use multiple assignment: `a, b = b, a`.

```python
msg1, msg2 = "Hello", "World" # msg1 = "Hello", msg2 = "World"
msg1, msg2 = msg2, msg1       # msg1 = "World", msg2 = "Hello"
```

**Q3**: How do we check the type of a variable or value in Python ? 

**Solution**:

Use the `type()` function 

Example: `type(10)` returns `<class 'int'>`.

**Q3**: What does type casting allow you to do in Python ? 

**Solution**:

Convert a variable from one type to another.

Example: `int(10.9)` → `10` (decimal is removed, not rounded).

**Q4**: When does converting a string to an integer cause an error in Python ? 

**Solution**:

When the string does not represent a number.

Example: `int("Hello")` raises a `ValueError`.

**Q5**: How do you declare a variable with no value in Python?

**Solution**:

Assign it the value `None`.

Writing a variable name alone (without a value) causes an error, but `name = None` is valid.