# Discuss the different types of operators in Python and provide examples of how they are used ?

Python supports various types of operators that allow you to perform operations on variables and values. Here is a comprehensive list of different types of operators in Python along with examples of how they are used:

### 1. **Arithmetic Operators**
These operators are used to perform basic mathematical operations.

| **Operator** | **Description**           | **Example**        |
|--------------|---------------------------|--------------------|
| `+`          | Addition                  | `a + b`            |
| `-`          | Subtraction               | `a - b`            |
| `*`          | Multiplication            | `a * b`            |
| `/`          | Division                  | `a / b`            |
| `%`          | Modulus (remainder)       | `a % b`            |
| `**`         | Exponentiation            | `a ** b`           |
| `//`         | Floor division            | `a // b`           |

**Examples:**
```python
a = 10
b = 3

print(a + b)   # Output: 13
print(a - b)   # Output: 7
print(a * b)   # Output: 30
print(a / b)   # Output: 3.3333333333333335
print(a % b)   # Output: 1
print(a ** b)  # Output: 1000
print(a // b)  # Output: 3
```

### 2. **Comparison Operators**
These operators compare two values and return a boolean result.

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `==`         | Equal to                  | `a == b`          |
| `!=`         | Not equal to              | `a != b`          |
| `>`          | Greater than              | `a > b`           |
| `<`          | Less than                 | `a < b`           |
| `>=`         | Greater than or equal to  | `a >= b`          |
| `<=`         | Less than or equal to     | `a <= b`          |

**Examples:**
```python
a = 5
b = 10

print(a == b)  # Output: False
print(a != b)  # Output: True
print(a > b)   # Output: False
print(a < b)   # Output: True
print(a >= b)  # Output: False
print(a <= b)  # Output: True
```

### 3. **Logical Operators**
These operators are used to combine conditional statements.

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `and`        | Logical AND               | `a and b`         |
| `or`         | Logical OR                | `a or b`          |
| `not`        | Logical NOT               | `not a`           |

**Examples:**
```python
a = True
b = False

print(a and b)  # Output: False
print(a or b)   # Output: True
print(not a)    # Output: False
```

### 4. **Bitwise Operators**
These operators perform bit-level operations.

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `&`          | AND                       | `a & b`           |
| `|`          | OR                        | `a | b`           |
| `^`          | XOR                       | `a ^ b`           |
| `~`          | NOT                       | `~a`              |
| `<<`         | Left shift                | `a << b`          |
| `>>`         | Right shift               | `a >> b`          |

**Examples:**
```python
a = 10  # 1010 in binary
b = 4   # 0100 in binary

print(a & b)   # Output: 0  (0000 in binary)
print(a | b)   # Output: 14 (1110 in binary)
print(a ^ b)   # Output: 14 (1110 in binary)
print(~a)      # Output: -11 (inverse of 1010 is -1011 in binary)
print(a << 2)  # Output: 40 (101000 in binary)
print(a >> 2)  # Output: 2  (10 in binary)
```

### 5. **Assignment Operators**
These operators are used to assign values to variables.

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `=`          | Assign                    | `a = 5`           |
| `+=`         | Add and assign            | `a += 3`          |
| `-=`         | Subtract and assign       | `a -= 2`          |
| `*=`         | Multiply and assign       | `a *= 3`          |
| `/=`         | Divide and assign         | `a /= 2`          |
| `%=`         | Modulus and assign        | `a %= 3`          |
| `**=`        | Exponentiate and assign   | `a **= 2`         |
| `//=`        | Floor divide and assign   | `a //= 2`         |

**Examples:**
```python
a = 5

a += 3  # a is now 8
a -= 2  # a is now 6
a *= 3  # a is now 18
a /= 2  # a is now 9.0
a %= 3  # a is now 0.0
a **= 2 # a is now 0.0
a //= 2 # a is now 0.0
```

### 6. **Membership Operators**
These operators test for membership in a sequence (e.g., strings, lists, or tuples).

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `in`         | True if value is found    | `'a' in list`     |
| `not in`     | True if value is not found| `'a' not in list` |

**Examples:**
```python
my_list = [1, 2, 3, 4, 5]

print(3 in my_list)       # Output: True
print(6 not in my_list)   # Output: True
```

### 7. **Identity Operators**
These operators compare the memory locations of two objects.

| **Operator** | **Description**           | **Example**       |
|--------------|---------------------------|-------------------|
| `is`         | True if the objects are identical | `a is b`         |
| `is not`     | True if the objects are not identical | `a is not b`    |

**Examples:**
```python
a = [1, 2, 3]
b = a
c = [1, 2, 3]

print(a is b)      # Output: True (same object in memory)
print(a is c)      # Output: False (different objects in memory)
print(a is not c)  # Output: True
```

These are the fundamental types of operators in Python along with examples demonstrating how they are used.
