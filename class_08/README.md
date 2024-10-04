
# Python Function Examples - Class 08

This repository contains Python examples illustrating basic and advanced function usage, including type hints, lambda expressions, and handling various types of arguments (positional, keyword, and variable-length arguments). These examples are extracted from the `class_08.ipynb` Jupyter notebook, which serves as an educational resource for understanding Python functions.


## Code Overview

### 1. Simple Addition
Demonstrates basic arithmetic operations.
```python
a: int = 5
b: int = 10
sum: int = a + b
print(sum)
```
This snippet calculates the sum of `a` and `b` and prints the result.

### 2. Basic Functions

#### `hello()`
A simple function that prints a greeting.
```python
def hello() -> None:
    print("hello")
hello()
```

#### `sum()`
A function that takes two integers and prints their sum.
```python
def sum(a: int, b: int) -> None:
    print(a + b)
sum(6, 7)
```

### 3. Returning Values from Functions
Functions that return values rather than just printing them.
```python
def sum(a: int, b: int) -> int:
    return a + b
result: int = sum(9, 15)
print(result)
```
This version of the `sum()` function returns the result of adding `a` and `b`.

### 4. Using Default and Optional Parameters

#### `prod()`
Demonstrates the use of default values for parameters.
```python
def prod(c: int, d: int = 1) -> None:
    print(c * d)
prod(5)
prod(5, 8)
```
You can call `prod()` with one or two arguments. If the second argument is omitted, it defaults to `1`.

### 5. Lambda Expressions
Lambda functions are one-liners used for small, simple operations.
```python
product = lambda a, b: a * b
print(product(8, 5))
```
This lambda function multiplies two numbers.

### 6. Using `map()` for List Transformations
Applies a function to each item in a list using the `map()` function.
```python
from typing import List
numbers: List[int] = [1, 2, 3, 4, 5]
result = list(map(lambda x: x**2, numbers))
print(result)
```
This code squares each number in the list.

### 7. Working with Variable-Length Arguments

#### `*args` - Positional Variable-Length Arguments
```python
def data_base(*students: tuple[str, ...]) -> None:
    print(students)
data_base("Hamza", "Ali", "Umar", "Humaiyon", "Abdullah")
```
This function accepts a variable number of positional arguments and prints them as a tuple.

#### `**kwargs` - Keyword Variable-Length Arguments
```python
from typing import Dict
def data_base(**students: Dict[str, str]) -> None:
    print(students)
data_base(name="Hamza", institute="PIAIC")
```
This function accepts a variable number of keyword arguments and prints them as a dictionary.

### 8. Advanced Function with Mixed Arguments
A combination of positional arguments, `*args`, and `**kwargs` to handle flexible input.
```python
def result(a: int, b: int, *c: tuple[str, ...], **d: Dict[str, str]) -> None:
    print(a, b, c, d)
result(2, 3, "hello", "bye", name="Hamza", institute="PIAIC")
```
This function demonstrates handling a mix of argument types, including fixed positional arguments, variable-length positional arguments, and keyword arguments.