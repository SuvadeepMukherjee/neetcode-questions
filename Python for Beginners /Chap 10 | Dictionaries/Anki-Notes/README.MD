# Dictionaries (Anki Notes)

**Q1**: What do Python dictionaries store ? 

**Solution**:

Key-value pairs 

```python
my_dict = {
    "Alice": 25,
    "Bob": 30,
    "Charlie": 35
}
```

**Q2**: How do you create a dictionary with values ? 

**Solution**:

Using curly braces`{}` with key-value pairs

my_dict = {"Alice": 25, "Bob": 30, "Charlie": 35}

```python
my_dict = {
    "Alice": 25,
    "Bob": 30,
    "Charlie": 35
}
```

**Q3**: How do you create an empty dictionary and then add key-value pair to the dictionary ? 

**Solution**:

```python
my_dict = {}

my_dict["Alice"] = 25
my_dict["Bob"] = 30
my_dict["Charlie"] = 35
```

**Q4**: What must be unique in a Python dictionary?

**Solution**:

- The keys.
- Values can repeat, but keys cannot.

**Q5**: What happens if you assign a new value to an existing key ? 

**Solution**:

The old value is overwritten 

```python
my_dict = {"a": 1, "b": 2, "c": 3}

print(my_dict["a"]) # Output: 1

my_dict["a"] = 4

print(my_dict["a"]) # Output: 4


```

**Q6**: What types can dictionary values have ? 

**Solution**: 

any type 

```python
my_dict = {"a": [1, 2, 3], "b": {4, 5, 6}, "c": {"x": 7, "y": 8, "z": 9}}

print(my_dict["a"]) # Output: [1, 2, 3]
print(my_dict["b"]) # Output: {4, 5, 6}
print(my_dict["c"]) # Output: {"x": 7, "y": 8, "z": 9}
```

**Q7**: How do you check if a dictionary contains a key ? 

**Solution**:

use the `in` keyword 

```python
my_dict = {"a": 1, "b": 2, "c": 3}

print("a" in my_dict) # Output: True
print("d" in my_dict) # Output: False
```

**Q8**: Are dictionaries ordered in Python ? 

**Solution**:

- Yes, they preserve insertion order.

- Items appear in the order they were added.

**Q9**: How can we get the number of key-value pairs in a dictionary ? 

**Solution**:

use the `len()` function 

```python
my_dict = {"a": 1, "b": 2, "c": 3}

print(len(my_dict)) # Output: 3
```

**Q10**: What does looping with `for key in my_dict` give you ? 

**Solution**:

It gives you each key 

We can then access the value with my_dict[key]

```python
my_dict = {"a": 1, "b": 2, "c": 3}

for key in my_dict:
    value = my_dict[key]
    print(key, value)


```

 

**Q11**: What does looping with `for key,value i n my_dict.items()` give you ? 

**Solution**:

Key-value pairs 

```python
my_dict = {"a": 1, "b": 2, "c": 3}

for key, value in my_dict.items():
    print(key, value)
```

**Q12**:  Given a list `[1, 2, 3, 1, 2, 3, 1, 2, 3]`, count the quantity of each element in the list using a dictionary.The result would be a dictionary like this : 

```python
count = {
    1: 3,
    2: 3,
    3: 3
}
```

**Solution**:

```python
from typing import Dict # this adds type hinting for Dict

def count_characters(word: str) -> Dict[str, int]:
	count ={}
    for char in word:
      if char not in count:
					count[char]= 1
        else:
          count[char]+=1
      return count
```

**Q13**: What does `pop(key)` do in a dictionary?

**Solution**:

Removes the key-value pair for that key.

It raises a `KeyError` if the key doesn't exist.

```python
my_dict = {"a": 1, "b": 2, "c": 3}

my_dict.pop("a")

print(my_dict) # Output: {"b": 2, "c": 3}

my_dict.pop("d") # Raises KeyError
```

**Q14**: How can we avoid a `KeyError` when using `pop()` ? 

**Solution**:

Provide a default value: `dict.pop(key, default)`.

If the key is missing, the default is returned instead of an error.

```python
my_dict = {"a": 1, "b": 2, "c": 3}

value = my_dict.pop("d", 0) # Returns 0, no error occurs
```

**Q15**: What does the `del` keyword do in a dictionary ? 

**Solution**:

Deletes a key-value pair.

```python
my_dict = {"a": 1, "b": 2, "c": 3}

del my_dict["a"]
```

**Q16**: How do you loop over only the values in a dictionary ? 

**Solution**:

Use `my_dict.values()`

```python
my_dict = {"a": 1, "b": 2, "c": 3}

for value in my_dict.values():
    print(value)
```

**Q17**: How do you convert all dictionary values into a list ? 

**Solution**:

Use `list(my_dict.values())`.

```python
my_dict = {"a": 1, "b": 2, "c": 3}

values = list(my_dict.values())

print(values) # Output: [1, 2, 3]
```

