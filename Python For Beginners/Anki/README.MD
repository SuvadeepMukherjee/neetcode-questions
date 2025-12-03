# Python For Beginners Anki Deck

**Q**: using a ___ before each quote character tells the python interpreter we want to interpret the quote `"` as a character inside the string , not as a quote that ends the string

**Solution**:

using a backslash `\` aka the escape charcter before each quote character inside a string tells the python interpreter we want to interpret the quote `"` as a charcter inside the string , not as a quote that ends the string

```python
print("They said, \"Hello, world!\"")
```

**Q**: in python comments are created using the `____`character , any text after the` ___`  character on a line is considered a comment 

**Solution**:

In python comments are created using the # character , any text after the # character on a line is considered a comment

```python
# This is a comment
```

**Q**: How to do multiple assignments in python ? 

**Solution**:

```python
msg1,msg2 = "Hello","World"

print(msg1,msg2)
```

**Q**: How can we swap 2 variables in python ?
**Solution**:

```python
a,b=10,20 
a,b = b,a
print(a,b)
```

**Q**: What is Type Casting ? 

**Solution**:

- A variable in python can be converted to a different type using type casting

```python
variable = 10.9 
print(int(variable))
```

**Q**: You have to print 10 with the variable number 

```python
number = 10.9
```

**Solution**:

```python
number = 10.9

print(int(number))
```

**Q**: Can we always convert a string to an integer 

**Solution**:

- We can't convert a string to an integer unless the string is a number 

**Q**: How to declare an empty variable ? 

**Solution**:

If we want to declare a variable without any value we can use the `None` keyword

```python
hello =None
```

