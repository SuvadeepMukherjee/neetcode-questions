# Functions (Anki Notes)

Anki Tag ➡️ 04-functions

**Q1**: What are the essential things you can do when defining a function in Python ? 

**Solution**:

Define it with `def`, use parameters, and optionally return a value.

```python
def add(x: int, y: int) -> int:
    return x + y


```

**Q2**: How can you specify what types a function should receive or return?

**Solution**:

By using type hints.

```python
def add(x: int, y: int) -> int:
    return x + y
```

**Q3**: What do default arguments allow you to do in Python functions?

**Solution**:

Provide a preset value for a parameter.

```python
def greet(name="world"):
    print("Hello, " + name + "!")

greet()       # This will print "Hello, world!"
greet("Bob")  # This will print "Hello, Bob!"
```

