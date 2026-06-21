# Dictionary-using-python-in-internship-5
# Documentation: Data Structures in Python

# Objective

This program demonstrates the four commonly used data structures in Python:

1. Lists
2. Tuples
3. Sets
4. Dictionaries

It also illustrates basic operations and methods associated with each data structure.

## 1. Lists

### Definition

A **list** is an ordered, mutable collection that can store elements of different data types and allows duplicate values.

### Example

```python
L = ["Python", 2, 8, 2, 9, 8, "Java"]
print(L)
```

### List Operations

#### `append()`

Adds an element to the end of the list.

```python
L.append("C")
print(L)
```

#### `count()`

Returns the number of times a specified element appears in the list.

```python
L.count(2)
```

#### `remove()`

Removes the first occurrence of the specified element.

```python
L.remove("Java")
print(L)
```

### Sample Output

```
['python', 2, 8, 2, 9, 8, 'Java']
['python', 2, 8, 2, 9, 8, 'Java', 'C']
['python', 2, 8, 2, 9, 8, 'Java', 'C']
['python', 2, 8, 2, 9, 8, 'C']
```

---

## 2. Tuples

### Definition

A **tuple** is an ordered and immutable collection. Once created, its elements cannot be modified.

### Example

```python
t = ()
print(type(t))

t = (1, 2, 3)
print(t)
```

### Built-in Functions

```python
print(max(t))
print(min(t))
print(sum(t))
```

### Tuple Operations

#### Concatenation

Combines two tuples.

```python
t1 = (1, 2)
t2 = (3, 4)
print(t1 + t2)
```

#### Repetition

Repeats the tuple elements.

```python
t = (3, 5)
print(t * 2)
```

### Sample Output

```
<class 'tuple'>
(1, 2, 3)
3
1
6
(1, 2, 3, 4)
(3, 5, 3, 5)
```

---

## 3. Sets

### Definition

A **set** is an unordered collection of unique elements. Duplicate values are automatically removed.

### Example

```python
s = {1, 5, 4, 2, 3, 9, 6, 4, 2, 10}
print(s)
```

### Note

```python
s = {}
```

creates an empty **dictionary**, not a set. To create an empty set, use:

```python
s = set()
```

### Set Methods

#### `add()`

Adds a new element to the set.

```python
s.add(19)
```

#### `remove()`

Removes the specified element.

```python
s.remove(5)
```

### Set Operations

#### Union

Returns all unique elements from both sets.

```python
print(s1.union(s2))
```

#### Intersection

Returns elements common to both sets.

```python
print(s1.intersection(s2))
```

#### Difference

Returns elements present in the first set but not in the second.

```python
print(s1.difference(s2))
```

### Sample Output

```
{1, 2, 3, 4, 5, 6, 9, 10}
{1, 2, 3, 4, 9, 10, 19}
{1, 2, 3, 4, 9, 10, 19}
{1, 2, 3, 4}
{2, 3}
{1}
```

---

## 4. Dictionaries

### Definition

A **dictionary** stores data as key-value pairs. Keys must be unique, while values may be duplicated.

### Example

```python
d = {1: 'python', 2: 'java', 'value': 'c'}
print(d)
```

### Dictionary Methods

#### `get()`

Retrieves the value associated with a given key.

```python
print(d.get(1))
```

#### `keys()`

Returns all keys in the dictionary.

```python
print(d.keys())
```

### Sample Output

```
<class 'dict'>
{1: 'python', 2: 'java', 'value': 'c'}
python
dict_keys([1, 2, 'value'])
```

---

# Summary Table

| Data Structure | Ordered                   | Mutable | Allows Duplicates     | Example            |
| -------------- | ------------------------- | ------- | --------------------- | ------------------ |
| List           | Yes                       | Yes     | Yes                   | `[1, 2, 3]`        |
| Tuple          | Yes                       | No      | Yes                   | `(1, 2, 3)`        |
| Set            | No                        | Yes     | No                    | `{1, 2, 3}`        |
| Dictionary     | Preserves insertion order | Yes     | Keys: No, Values: Yes | `{'a': 1, 'b': 2}` |

# Conclusion

Python provides several built-in data structures to organize and manipulate data efficiently. Lists are flexible and mutable, tuples provide immutable sequences, sets store unique elements and support mathematical operations, and dictionaries map unique keys to values for fast data retrieval.
