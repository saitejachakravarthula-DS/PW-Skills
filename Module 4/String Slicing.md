# String Slicing in Python
String slicing in Python is a powerful feature that allows you to extract parts of a string using a specific syntax. The basic syntax for slicing a string is:

```python
string[start:end:step]
```

Here's a breakdown of each part:
- `start`: The starting index of the slice (inclusive). If omitted, it defaults to the beginning of the string.
- `end`: The ending index of the slice (exclusive). If omitted, it defaults to the end of the string.
- `step`: The step or stride, which determines how many characters to skip. If omitted, it defaults to 1.

### Basic Examples

1. **Extracting a Substring**

```python
s = "Hello, World!"
substring = s[0:5]  # Extracts from index 0 to 4
print(substring)  # Output: Hello
```

2. **Skipping Characters**

```python
s = "Hello, World!"
substring = s[::2]  # Skips every second character
print(substring)  # Output: Hlo ol!
```

3. **Reversing a String**

```python
s = "Hello, World!"
reversed_s = s[::-1]  # Step is -1, which reverses the string
print(reversed_s)  # Output: !dlroW ,olleH
```

4. **Slicing with Negative Indices**

Negative indices allow you to count from the end of the string.

```python
s = "Hello, World!"
substring = s[-6:-1]  # Extracts from index -6 to -2 (last index is -1, but exclusive)
print(substring)  # Output: World
```

5. **Omitting Start or End**

If you omit the `start` or `end`, the slice will take everything up to that point.

```python
s = "Hello, World!"
substring_from_start = s[:5]  # From start to index 4
print(substring_from_start)  # Output: Hello

substring_to_end = s[7:]  # From index 7 to the end
print(substring_to_end)  # Output: World!
```

6. **Step with Negative Slicing**

Using a negative step to reverse a portion of the string:

```python
s = "Hello, World!"
reversed_substring = s[11:6:-1]  # Reverse the substring from index 11 to 7
print(reversed_substring)  # Output: dlroW
```

### Examples in Context

1. **Extracting the Domain from an Email Address**

```python
email = "user@example.com"
domain = email[email.index("@")+1:]  # Extract from the character after '@' to the end
print(domain)  # Output: example.com
```

2. **Extracting Filename and Extension**

```python
file = "document.pdf"
filename = file[:file.index(".")]  # Extract from start to the character before '.'
extension = file[file.index(".")+1:]  # Extract from the character after '.' to the end
print(filename)  # Output: document
print(extension)  # Output: pdf
```

### Combining Slices

Slices can be combined or nested to achieve more complex manipulations.

```python
s = "The quick brown fox jumps over the lazy dog"
words_reversed = " ".join([word[::-1] for word in s.split()])
print(words_reversed)  # Output: ehT kciuq nworb xof spmuj revo eht yzal god
```

In this example, we split the string into words, reverse each word, and then join them back into a single string.

String slicing is a versatile tool in Python, enabling you to manipulate and access string data in efficient and expressive ways.
