# Loops (Anki Notes)

**Q1**: How does a `while` loop work in Python ? 

**Solution**:

It repeats as long as its condition is `True`

```python
i = 0
while i < 5:
    print("I love Python!")
    i += 1
```

**Q2**: What does `range()` allow a `for` loop to control in Python ? 

**Solution**:

The start, stop, and step of the loop.

```python
for i in range(10):
    print(i)

# prints 0 -> 9 
```

```python
for i in range(2, 5):
    print(i)

# prints 2 -> 4 
```

```python
for i in range(0, 10, 2):
    print(i)

# prints 0 , 2 , 4 , 6 , 8
```

```python
for i in range(10, 0, -1):
    print(i)

# prinys 10 to 1 
```

**Q3**: What control statements can alter loop execution in Python ? 

**Solution**:

`break`, `continue`, and `pass`.

`break` exits the loop, `continue` skips to the next iteration, and `pass` does nothing (used as a placeholder in loops, `if` statements, and function bodies).

```python
for i in range(1, 8):
    pass

if True:
    pass

def unfinsished_function():
    pass
```

