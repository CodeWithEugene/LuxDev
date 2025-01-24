# Day 2 Assignment

## 1. Difference Between `while` and `do...while` Loops

- **`while` loop**: The condition is checked before the execution of the loop's body. If the condition is false initially, the loop body will not execute at all.
    ```python
    while (condition) {
            // code to be executed
    }
    ```

- **`do...while` loop**: The loop's body is executed at least once before the condition is checked. The condition is checked after the execution of the loop's body.
    ```python
    do {
            // code to be executed
    } while (condition);
    ```

## 2. Nested Loops

Nested loops are loops within loops. The inner loop runs completely every time the outer loop runs once. They are useful for iterating over multi-dimensional data structures like matrices.
```python
for (int i = 0; i < outerLimit; i++) {
        for (int j = 0; j < innerLimit; j++) {
                // code to be executed
        }
}
```

## 3. Difference Between `return` Statement and `print` Statement

- **`return` statement**: Used to exit a function and optionally pass back a value to the caller.
    ```python
    def add(a, b):
            return a + b
    ```

- **`print` statement**: Used to output data to the console.
    ```python
    print("Hello, World!")
    ```

## 4. Functions, Files, and Classes

### Functions

Functions are reusable blocks of code that perform a specific task. They can take inputs (parameters) and return outputs.
```python
def greet(name):
        return f"Hello, {name}!"
```

### Files

- **Reading a file**:
    ```python
    with open('file.txt', 'r') as file:
            content = file.read()
    ```

- **Writing to a file**:
    ```python
    with open('file.txt', 'w') as file:
            file.write("Hello, World!")
    ```

### Classes

Classes are blueprints for creating objects. They encapsulate data and functions that operate on the data.
```python
class Person:
        def __init__(self, name, age):
                self.name = name
                self.age = age

        def greet(self):
                return f"Hello, my name is {self.name} and I am {self.age} years old."
```