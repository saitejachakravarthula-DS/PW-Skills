# Access , Modify and Delete elements in a list

### Accessing Elements in a List

You can access elements in a list using indexing and slicing.

1. **Indexing**
   - Lists are zero-indexed, meaning the first element is at index 0.

```python
fruits = ['apple', 'banana', 'cherry']
print(fruits[0])  # Output: apple
print(fruits[1])  # Output: banana
print(fruits[2])  # Output: cherry
```

   - Negative indices count from the end of the list.

```python
print(fruits[-1])  # Output: cherry
print(fruits[-2])  # Output: banana
print(fruits[-3])  # Output: apple
```

2. **Slicing**
   - Slicing allows you to access a range of elements.

```python
print(fruits[1:3])  # Output: ['banana', 'cherry']
print(fruits[:2])   # Output: ['apple', 'banana']
print(fruits[1:])   # Output: ['banana', 'cherry']
print(fruits[:])    # Output: ['apple', 'banana', 'cherry']
```

### Modifying Elements in a List

You can modify elements by accessing them directly via their index or using list methods.

1. **Changing an Element**
   - Assign a new value to a specific index.

```python
fruits[1] = 'blueberry'
print(fruits)  # Output: ['apple', 'blueberry', 'cherry']
```

2. **Adding Elements**
   - `append()`: Adds an element to the end of the list.

```python
fruits.append('date')
print(fruits)  # Output: ['apple', 'blueberry', 'cherry', 'date']
```

   - `insert()`: Inserts an element at a specified position.

```python
fruits.insert(1, 'banana')
print(fruits)  # Output: ['apple', 'banana', 'blueberry', 'cherry', 'date']
```

   - `extend()`: Adds elements from another list to the end.

```python
fruits.extend(['elderberry', 'fig'])
print(fruits)  # Output: ['apple', 'banana', 'blueberry', 'cherry', 'date', 'elderberry', 'fig']
```

### Deleting Elements from a List

You can delete elements using various methods, including `remove()`, `pop()`, and `del`.

1. **Using `remove()`**
   - Removes the first occurrence of a value.

```python
fruits.remove('banana')
print(fruits)  # Output: ['apple', 'blueberry', 'cherry', 'date', 'elderberry', 'fig']
```

2. **Using `pop()`**
   - Removes and returns the element at the specified position (or the last element if no index is specified).

```python
last_fruit = fruits.pop()
print(last_fruit)  # Output: fig
print(fruits)      # Output: ['apple', 'blueberry', 'cherry', 'date', 'elderberry']

second_fruit = fruits.pop(1)
print(second_fruit)  # Output: blueberry
print(fruits)        # Output: ['apple', 'cherry', 'date', 'elderberry']
```

3. **Using `del`**
   - Deletes an element at a specific index or a slice of elements.

```python
del fruits[0]
print(fruits)  # Output: ['cherry', 'date', 'elderberry']

del fruits[1:3]
print(fruits)  # Output: ['cherry']
```

4. **Using `clear()`**
   - Removes all elements from the list.

```python
fruits.clear()
print(fruits)  # Output: []
```

### Examples

1. **Accessing Nested Lists**

```python
matrix = [[1, 2, 3], [4, 5, 6], [7, 8, 9]]
print(matrix[1][2])  # Output: 6
```

2. **Combining Multiple Operations**

```python
numbers = [1, 2, 3, 4, 5]
numbers[2] = 10          # Modify element at index 2
numbers.append(6)        # Add element to the end
numbers.insert(1, 0)     # Insert element at index 1
removed = numbers.pop(3) # Remove and return element at index 3
print(numbers)           # Output: [1, 0, 2, 10, 4, 5, 6]
print(removed)           # Output: 3
```

In summary, accessing, modifying, and deleting elements in a Python list can be done using straightforward and flexible operations, which make lists a highly useful and versatile data structure in Python.