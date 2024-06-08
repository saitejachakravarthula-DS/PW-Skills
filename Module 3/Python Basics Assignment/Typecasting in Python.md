# Explain the concept of type casting in Python with examples ?
Type casting in Python refers to converting one data type into another. This is useful when you need to perform operations that require a specific data type or when you're dealing with input/output operations where data types need to be consistent. Python supports several built-in functions for type casting.

### Types of Type Casting

1. **Implicit Type Casting**
2. **Explicit Type Casting**

### 1. Implicit Type Casting

In implicit type casting, Python automatically converts one data type to another without the need for explicit instructions. This usually happens in operations involving mixed data types, where Python promotes one type to another to avoid data loss.

**Example:**
```python
# Implicit type casting
a = 5        # int
b = 2.5      # float

# a is automatically converted to float before addition
result = a + b

print(result)        # Output: 7.5
print(type(result))  # Output: <class 'float'>
```

In this example, the integer `a` is implicitly converted to a float to match the type of `b` before performing the addition.

### 2. Explicit Type Casting

Explicit type casting, also known as type conversion, requires you to manually convert a value from one data type to another using Python’s built-in functions.

**Common Type Casting Functions:**
- `int()`: Converts a value to an integer.
- `float()`: Converts a value to a float.
- `str()`: Converts a value to a string.
- `bool()`: Converts a value to a boolean.

#### Examples of Explicit Type Casting

**Converting to Integer:**
```python
# Convert float to int
a = 2.8
b = int(a)
print(b)            # Output: 2
print(type(b))      # Output: <class 'int'>

# Convert string to int
s = "123"
i = int(s)
print(i)            # Output: 123
print(type(i))      # Output: <class 'int'>
```

**Converting to Float:**
```python
# Convert int to float
a = 10
b = float(a)
print(b)            # Output: 10.0
print(type(b))      # Output: <class 'float'>

# Convert string to float
s = "3.14"
f = float(s)
print(f)            # Output: 3.14
print(type(f))      # Output: <class 'float'>
```

**Converting to String:**
```python
# Convert int to string
a = 10
s = str(a)
print(s)            # Output: '10'
print(type(s))      # Output: <class 'str'>

# Convert float to string
f = 2.5
s = str(f)
print(s)            # Output: '2.5'
print(type(s))      # Output: <class 'str'>
```

**Converting to Boolean:**
```python
# Convert int to boolean
a = 1
b = 0
print(bool(a))      # Output: True
print(bool(b))      # Output: False

# Convert string to boolean
s1 = "hello"
s2 = ""
print(bool(s1))     # Output: True
print(bool(s2))     # Output: False
```

### Use Cases of Type Casting

1. **Mathematical Operations:**
   Ensure numbers are in the correct type (int, float) before performing operations.
   ```python
   a = "10"
   b = "20"
   result = int(a) + int(b)
   print(result)  # Output: 30
   ```

2. **User Input:**
   Convert string input from users to the appropriate type for further processing.
   ```python
   age = input("Enter your age: ")
   age = int(age)
   print(f"Next year you will be {age + 1}")
   ```

3. **Data Conversion:**
   Convert data types when reading from files or databases where data is often stored as strings.
   ```python
   data = "100.5"
   value = float(data)
   print(value)  # Output: 100.5
   ```

4. **Conditional Checks:**
   Convert types for proper evaluation in conditions.
   ```python
   is_active = "True"
   if bool(is_active):
       print("The status is active.")
   ```

### Summary

Type casting is a fundamental concept in Python that allows you to convert one data type to another, either implicitly or explicitly. It ensures that operations are performed correctly and efficiently, depending on the types involved. Understanding and effectively using type casting can prevent errors and enhance the robustness of your code.
