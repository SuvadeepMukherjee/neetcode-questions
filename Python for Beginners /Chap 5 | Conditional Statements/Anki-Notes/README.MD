# Conditional Statements



**Q1**: Do `if` statements create a new scope in Python ? 

**Solution**:

No , they do not 

Variables created inside an `if` block are accessible outside it — e.g., `message` defined in an `if` can be used later.

```python
if True:
    message = "Hello"

print(message)  # This will print "Hello"
```

**Q2**: A value is falsy if it is : 

**Solution**:

A value is falsy if 

- `False` (boolean)
- `None` (NoneType)
- `0` (integer)
- `0.0` (float)
- `""` (empty string)
- `[]` (empty list)
- Most other empty collections (e.g. empty tuple, empty set, empty dictionary)

**Q3**: A value is truthy if it is: 

**Solution**:

A value is **truthy** if it is:

- `True` (boolean)
- All integers other than `0`
- All floats other than `0.0`
- All strings other than `""`
- All collections with at least one element