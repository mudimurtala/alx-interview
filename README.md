# Pascal's Triangle

This project involves implementing a Python function to generate Pascal's Triangle, a mathematical concept that forms a triangular array where each number is the sum of the two numbers directly above it. The task requires applying several Python programming concepts, including lists, loops, and arithmetic operations.

## Project Overview

The goal of this project is to create a function `def pascal_triangle(n):` that returns a list of lists of integers representing Pascal's Triangle for a given integer `n`. If `n` is less than or equal to 0, the function should return an empty list.

### Example Output

For `n = 5`, the Pascal's Triangle should look like this:

[
[1],
[1, 1],
[1, 2, 1],
[1, 3, 3, 1],
[1, 4, 6, 4, 1]
]


## Concepts to Master

To complete this project successfully, the following Python concepts are essential:

- **Lists and List Comprehensions**: Learn to create, access, modify, and iterate over lists. Use list comprehensions to generate rows of Pascal's Triangle.
- **Functions**: Define and call functions that pass parameters and return values, particularly a list of lists representing Pascal's Triangle.
- **Loops**: Use `for` and `while` loops to iterate through sequences. Nested loops may be necessary for generating each row of Pascal's Triangle.
- **Conditional Statements**: Apply `if`, `elif`, and `else` conditions to implement logic based on the position within Pascal's Triangle.
- **Arithmetic Operations**: Perform addition to calculate each element of Pascal's Triangle as the sum of the two elements directly above it.
- **Indexing and Slicing**: Access elements and slices of lists to identify and sum the correct elements when constructing each row of the triangle.
- **Memory Management**: Be mindful of how lists are stored and copied, especially when creating new rows based on the values of the previous row.
- **Efficiency and Optimization**: Consider the time and space complexity of different approaches to generating Pascal's Triangle and apply optimizations to improve performance.

## Implementation

### Function Definition

```python
def pascal_triangle(n):
    if n <= 0:
        return []
    
    triangle = [[1]]  # Initialize the first row of Pascal's Triangle

    for i in range(1, n):
        row = [1]  # Every row starts with a '1'
        for j in range(1, i):
            # Calculate the value by summing two elements above the current position
            row.append(triangle[i-1][j-1] + triangle[i-1][j])
        row.append(1)  # Every row ends with a '1'
        triangle.append(row)
    
    return triangle

Usage Example
You can test the function with the following code:

if __name__ == "__main__":
    pascal_triangle = __import__('0-pascal_triangle').pascal_triangle
    
    def print_triangle(triangle):
        for row in triangle:
            print("[{}]".format(",".join([str(x) for x in row])))

    print_triangle(pascal_triangle(5))

Running the above code should produce the following output:

[1]
[1,1]
[1,2,1]
[1,3,3,1]
[1,4,6,4,1]

Repository Structure
GitHub repository: alx-interview
Directory: 0x00-pascal_triangle
File: 0-pascal_triangle.py

License
This project is licensed under the ALX Program.

