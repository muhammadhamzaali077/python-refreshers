# Python Dictionaries

This repository provides a comprehensive overview of Python dictionaries, including their syntax, key and value types, methods, and practical examples.

## Overview

A dictionary in Python is a mutable, unordered collection of key-value pairs. Keys must be unique and immutable (e.g., strings, numbers, or tuples), while values can be of any data type.

### Syntax

```python
from typing import Dict

data: Dict[str, str] = {
    "key": "value",
    "key_1": "value_1"
}
```

### Key Types

- `str`
- `int`
- `float`
- `tuple`
- `bool`

### Example Usage

#### Creating a Dictionary

```python
data: Dict[str, str] = {
    "name": "Hamza",
    "father_name": "Muhammad Aslam",
}
```

#### Accessing and Modifying Values

```python
data["name"] = "Muhammad Hamza"
data["age"] = "19"
```

#### Common Methods

- `clear()`: Removes all items from the dictionary.
- `copy()`: Returns a shallow copy of the dictionary.
- `get(key, default)`: Returns the value for the specified key, or `default` if the key is not found.
- `items()`: Returns a view object that displays a list of dictionary's key-value tuple pairs.
- `keys()`: Returns a view object that displays a list of all the keys in the dictionary.
- `values()`: Returns a view object that displays a list of all the values in the dictionary.
- `pop(key)`: Removes the specified key and returns the corresponding value.
- `popitem()`: Removes and returns the last inserted key-value pair.
- `setdefault(key, default)`: Returns the value of the specified key. If the key does not exist, insert the key with the specified default value.
- `update()`: Updates the dictionary with elements from another dictionary or from an iterable of key-value pairs.

### Advanced Example

You can also create dictionaries with various data types for keys and values:

```python
from typing import Dict, Union, List, Tuple

key = Union[str, int, float, Tuple, bool]
value = Union[str, int, float, Tuple, bool, set, Dict, List]

data: Dict[key, value] = {
    "name": "Hamza",
    "father_name": "Muhammad Aslam",
    "id": 51,
    "percentage": 94.6,
}

for k, v in data.items():
    print(f"{k}: {v}")
```

### Zip and Unzip Example

You can also swap variable values easily:

```python
a = 5
b = 9
a, b = b, a  # Swaps values
```

## Conclusion

This repository serves as a reference for understanding and using dictionaries in Python. You can explore various examples and try them out in your own Python projects.