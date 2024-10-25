# Python Basic Operations

This README demonstrates some fundamental Python code examples, including greeting functions, looping structures, factorial calculations using recursion and iteration, and basic condition handling. 

## Code Overview

### Greeting Function

The function `greeting` takes a `name` as an argument and prints a personalized greeting.

```python
def greeting(name: str) -> None:
    print(f"Hello {name}")

# Example usage
greeting("Hamza")  # Output: Hello Hamza
```

### Odd Numbers with `for` Loop

A simple `for` loop iterates from 1 to 10 in steps of 2 to print all odd numbers within this range.

```python
for n in range(1, 10+1, 2):
    print(n)
```

### Factorial Calculation Using Recursion

The recursive `fact` function calculates the factorial of a given number `n`. 

**Explanation:** 
- Base case: The factorial of 0 or 1 is 1.
- Recursive step: Multiply `n` by the factorial of `n-1`.

```python
def fact(n):
    if n == 0 or n == 1:
        return 1
    else:
        result = n * fact(n - 1)
        return result

# Example usage
print(fact(5))  # Output: 120 (1 x 2 x 3 x 4 x 5)
```

### Factorial Calculation Using a `for` Loop

The factorial of 5 is calculated iteratively using a `for` loop, without defining a function.

```python
factorial = 1
for i in range(1, 6):
    factorial *= i

print(factorial)  # Output: 120
```

### Conditional Example

This simple conditional checks if the `condi` variable is `True` or `False` and prints a corresponding message.

```python
condi = False
if condi:
    print("hello")
else:
    print("by")  # Output: by
```

### Summary

- **Greeting Function**: Uses `print` to display a greeting with the provided name.
- **Odd Numbers Loop**: Demonstrates a `for` loop with a step.
- **Factorial Calculation**: Shows both recursive and iterative methods for calculating factorial.
- **Condition Handling**: Demonstrates a basic `if-else` statement. 
