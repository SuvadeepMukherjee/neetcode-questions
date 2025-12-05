# Python For Beginners Anki Deck

Anki ➡️ 01-introduction

**Q1**: using a ___ before each quote character tells the python interpreter we want to interpret the quote `"` as a character inside the string , not as a quote that ends the string

**Solution**:

using a backslash `\` aka the escape charcter before each quote character inside a string tells the python interpreter we want to interpret the quote `"` as a charcter inside the string , not as a quote that ends the string

```python
print("They said, \"Hello, world!\"")
```

**Q2**: in python comments are created using the `____`character , any text after the` ___`  character on a line is considered a comment 

**Solution**:

In python comments are created using the # character , any text after the # character on a line is considered a comment

```python
# This is a comment
```

---

Anki ➡️02-variables

**Q1**: How to do multiple assignments in python ? 

**Solution**:

```python
msg1,msg2 = "Hello","World"

print(msg1,msg2)
```

**Q2**: How can we swap 2 variables in python ?
**Solution**:

```python
a,b=10,20 
a,b = b,a
print(a,b)
```

**Q3**: What is Type Casting ? 

**Solution**:

- A variable in python can be converted to a different type using type casting

```python
variable = 10.9 
print(int(variable))
```

**Q4**: You have to print 10 with the variable number 

```python
number = 10.9
```

**Solution**:

```python
number = 10.9

print(int(number))
```

**Q5**: Can we always convert a string to an integer 

**Solution**:

- We can't convert a string to an integer unless the string is a number 

**Q6**: How to declare an empty variable ? 

**Solution**:

If we want to declare a variable without any value we can use the `None` keyword

```python
hello =None
```

---

Anki Tag ➡️ 03-math

**Q1**:If we divide y by x , what will be the result ? 

**Solution**:

If we divide `y` by `x` , the result will be 2.0 and not 2 .This is because the result of division is always a float in python

**Q2**: For arithmatic operators like addition , substraction , multiplication the result will be an  if both operands are `___` . If one of the operands is a ` ___` the result will be a `____`

**Solution**:

For  arithmetic operators (like addition ,substraction , multiplication) the result will be an integer if both operands are integers. If one of the operands is a float, the result will be a float.

**Q3**: What does Floor divsion do ? 

**Solution**:

- divides the first operand by the second and rounds down the result to an integer 

  ```
  x, y = 7, 2
  
  print(x // y) # Output: 3  (7 divided by 2 is 3.5, after rounding down we get 3)
  ```

**Q4**: What does Modulas do ? 

**Solution**:

- returns the remainder of the division of the first operand by the second 

  ```python
  print(x % y)  # Output: 1  (7 divided by 2 is 3, with a remainder of 1)
  ```

**Q5**: What does exponentian do ? 

**Solution**:

- raises the first operand to the power of the second operand

```
print(x ** y) # Output: 49 (7 raised to the power of 2 is 49, 7*7 = 49)
```

**Q6**: Explain Shorthand operators 

**Solution**:

- `+=` is shorthand for `count = count +`
- `-=` is shorthand for `count = count -`
- `*=` is shorthand for `count = count *`
- `/=` is shorthand for `count = count /`
- `%=` is shorthand for `count = count %`
- `//=` is shorthand for `count = count //`
- `**=` is shorthand for `count = count **`

**Q7**: Explain Boolean or , Boolean and and Booleab not ? 

**Solution**:

| Logical Operator | Result                                                       |
| ---------------- | ------------------------------------------------------------ |
| Boolean OR       | The OR operation returns  `True` if at least one of the operands is `True` |
| Boolean and      | The `and` operation returns `True` if all the operands are `True` |
| Boolean and      | It simply inverts the value of the operand. If the operand is `True`, the result is `False`. If the operand is `False`, the result is `True`. |

---

Anki Tag ➡️ 04-functions

**Q1**: How are functions defined in Python ? 

**Solution**:

- Functions are defined using the `def` keyword followed by the function name and parentheses with a colon `():`

- The code that belongs to the function *must* be indented with whitespace

  ```python
  def greet():
      print("Hello, world!")
  ```

