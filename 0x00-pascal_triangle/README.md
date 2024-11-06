# Pascal's Triangle in Python

## Project Overview
This project involves implementing Pascal's Triangle in Python. Pascal's Triangle is a mathematical concept where each row represents the coefficients of the binomial expansion. Each element is the sum of the two elements directly above it. This exercise is a great way to reinforce foundational Python concepts such as lists, loops, functions, and conditional statements.

- **Project Start**: September 30, 2024
- **Project Deadline**: October 4, 2024

## Learning Objectives
By completing this project, you will:
1. Understand the structure of Pascal's Triangle.
2. Gain experience with Python algorithms and their efficiency.
3. Use lists, list comprehensions, functions, loops, and conditional statements effectively.

## Prerequisites
To successfully complete this project, it is recommended that you have a solid understanding of the following Python concepts:

- **Lists and List Comprehensions**
  - How to create, access, and modify lists.
  - Using list comprehensions for concise and readable code.

- **Functions**
  - Defining and calling functions.
  - Working with parameters and return values.

- **Loops and Conditional Statements**
  - Using `for` and `while` loops for iteration.
  - Applying `if`, `elif`, and `else` for condition-based logic.

- **Indexing and Arithmetic Operations**
  - Performing basic arithmetic for generating triangle values.
  - Using list indexing to access specific elements.

## Project Requirements
- Implement a function that generates Pascal's Triangle up to a specified number of rows.
- The function should return a list of lists, where each sublist represents a row in Pascal's Triangle.
- Each row begins and ends with `1`, and each interior element is the sum of the two elements directly above it from the previous row.

## Example Usage
```python
def pascal_triangle(n):
    # Function implementation
    pass

# Example: Generating 5 rows of Pascal's Triangle
print(pascal_triangle(5))
# Expected Output:
# [
#   [1],
#   [1, 1],
#   [1, 2, 1],
#   [1, 3, 3, 1],
#   [1, 4, 6, 4, 1]
# ]

