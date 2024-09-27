# Python Loops and Input Handling

This notebook demonstrates examples of different types of loops (`for` and `while`) and handling user inputs in Python. The primary focus is on:

- Iterating over sequences using `for` loops.
- Using `while` loops where conditions are checked before each iteration.
- Accepting user inputs during runtime and processing them.

## Table of Contents
1. [For Loop](#for-loop)
2. [While Loop](#while-loop)
3. [User Input](#user-input)
4. [Additional Examples](#additional-examples)

### For Loop
A `for` loop is used to iterate over a sequence (such as a list, tuple, set, or dictionary). The loop executes once for each item in the sequence.

**Syntax**:
```python
for item in sequence:
    logic
```

**Example**:
```python
from typing import List
students: List[str] = ["hamza", "usama", "hunain"]
for student in students:
    print(student)
```

Output:
```
hamza
usama
hunain
```

### While Loop
A `while` loop is used when you do not know in advance how many times the loop should run. It continues until the condition becomes `False`.

**Syntax**:
```python
while condition:
    logic
```

**Example**:
```python
start_count = 0
while start_count <= 5:
    print(start_count)
    start_count += 1
```

Output:
```
0
1
2
3
4
5
```

### User Input
You can prompt the user for input during runtime using the `input()` function. The input received is treated as a string.

**Example**:
```python
user_input: str = input("Enter city name: ")
print(type(user_input))
print(user_input)
```

### Additional Examples
- Repeatedly asking for input until a user enters 'quit':
```python
prompt = "Tell me something, and I will repeat it back to you:\nEnter 'quit' to end the program."
message = ""
while message != 'quit':
    message = input(prompt)
    print(message)
```

- Checking user height to determine eligibility for a ride:
```python
prompt = "Enter your height: "
user_height = int(input(prompt))

if user_height >= 48:
    print("You can ride")
else:
    print("You can't ride")
```

Output:
```
You can't ride
```