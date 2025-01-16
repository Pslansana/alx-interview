# 0x09. Island Perimeter

## Project Overview

The **Island Perimeter** project focuses on solving a geometric problem using algorithms, data structures, and Python programming. You are required to calculate the perimeter of an island represented within a 2D grid. In this grid, cells are either land (`1`) or water (`0`). The task involves iterating through the grid, identifying land cells, and applying logic to determine their contribution to the total perimeter.

This project ran from **Dec 2, 2024, 3:00 AM to Dec 6, 2024, 3:00 AM**, with an automatic review scheduled at the deadline.

---

## Learning Objectives

By the end of this project, you should be able to explain:

### 1. **2D Arrays (Matrices)**
   - How to create and work with 2D arrays (lists of lists) in Python.
   - Techniques for accessing and iterating over elements in a 2D array.
   - Navigating adjacent cells horizontally and vertically.

### 2. **Conditional Logic**
   - Applying conditions to determine whether a cell contributes to the perimeter.
   - Identifying the boundaries of the grid and handling edge cases where cells are at the border.

### 3. **Counting Techniques**
   - Developing a systematic method to count the number of edges contributing to the perimeter.
   - Accounting for shared edges between adjacent land cells, which reduces the perimeter count.

### 4. **Problem-Solving Strategies**
   - Breaking down a complex problem into smaller, manageable tasks:
     1. Identify land cells.
     2. Check adjacent cells (up, down, left, right).
     3. Count edges contributing to the perimeter.
   - Combining iteration, condition checking, and counting in an efficient manner.

### 5. **Python Programming**
   - Using nested loops to iterate over grid cells.
   - Writing conditional statements to check the status of adjacent cells.
   - Ensuring code follows the **PEP 8** style guide.
   - Documenting modules and functions for clarity and maintainability.

---

## Requirements

### General

- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted/compiled on **Ubuntu 20.04 LTS** using Python 3 (version 3.4.3).
- All files should end with a new line.
- The first line of all Python files must be:
  ```bash
  #!/usr/bin/python3
