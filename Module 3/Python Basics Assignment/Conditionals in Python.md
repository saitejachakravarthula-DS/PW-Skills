# How do conditional statements work in Python? Illustrate with examples
Conditional statements in Python allow you to execute specific blocks of code based on certain conditions. The main conditional statements in Python are `if`, `elif`, and `else`. Here’s a detailed look at how these statements work, along with examples:

### `if` Statement

The `if` statement allows you to test a condition and execute a block of code if the condition is true.

**Syntax:**
```python
if condition:
    # code to execute if condition is true
```

**Example:**
```python
x = 10

if x > 5:
    print("x is greater than 5")
```

**Output:**
```
x is greater than 5
```

### `if-else` Statement

The `if-else` statement allows you to execute one block of code if the condition is true and another block of code if the condition is false.

**Syntax:**
```python
if condition:
    # code to execute if condition is true
else:
    # code to execute if condition is false
```

**Example:**
```python
x = 3

if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

**Output:**
```
x is not greater than 5
```

### `if-elif-else` Statement

The `if-elif-else` statement allows you to check multiple conditions. The first block of code that has a true condition is executed.

**Syntax:**
```python
if condition1:
    # code to execute if condition1 is true
elif condition2:
    # code to execute if condition2 is true
else:
    # code to execute if none of the above conditions are true
```

**Example:**
```python
x = 7

if x > 10:
    print("x is greater than 10")
elif x > 5:
    print("x is greater than 5 but not greater than 10")
else:
    print("x is 5 or less")
```

**Output:**
```
x is greater than 5 but not greater than 10
```

### Nested `if` Statements

You can nest `if` statements inside other `if` statements to check multiple conditions.

**Syntax:**
```python
if condition1:
    if condition2:
        # code to execute if both condition1 and condition2 are true
```

**Example:**
```python
x = 15

if x > 10:
    print("x is greater than 10")
    if x > 20:
        print("x is also greater than 20")
    else:
        print("x is not greater than 20")
```

**Output:**
```
x is greater than 10
x is not greater than 20
```

### Conditional Expressions (Ternary Operator)

Python supports a shorthand for `if-else` statements, known as a conditional expression or ternary operator.

**Syntax:**
```python
value_if_true if condition else value_if_false
```

**Example:**
```python
x = 4

result = "x is even" if x % 2 == 0 else "x is odd"
print(result)
```

**Output:**
```
x is even
```

### Examples with Multiple Conditions

You can combine multiple conditions using logical operators `and`, `or`, and `not`.

**Example:**
```python
x = 8
y = 3

if x > 5 and y < 5:
    print("x is greater than 5 and y is less than 5")

if x > 5 or y > 5:
    print("Either x is greater than 5 or y is greater than 5")

if not y == 3:
    print("y is not equal to 3")
else:
    print("y is equal to 3")
```

**Output:**
```
x is greater than 5 and y is less than 5
Either x is greater than 5 or y is greater than 5
y is equal to 3
```

### Summary

Conditional statements in Python (`if`, `elif`, `else`) allow you to execute code based on certain conditions, and you can nest them or use logical operators for complex conditions. These control structures are fundamental for directing the flow of your program.
