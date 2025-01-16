# 0x04. UTF-8 Validation

## Overview

This project focuses on validating UTF-8 encoded data using Python. You will use bitwise operations to determine whether a given dataset represents a valid UTF-8 encoding. Understanding the UTF-8 encoding scheme and how to manipulate bits in Python is essential for this task.

---

## Learning Objectives

By the end of this project, you should be able to:

- Apply bitwise operations in Python to manipulate and interpret binary data.
- Understand the UTF-8 encoding scheme, including how characters are encoded across multiple bytes.
- Recognize valid patterns for UTF-8 encoding.
- Implement Python logic to validate UTF-8 encoded data.

---

## Requirements

- **Environment**: Ubuntu 20.04 LTS
- **Python Version**: 3.4.3
- **Style Guide**: PEP 8 (version 1.7.x)
- **File Format**: All files should:
  - Start with `#!/usr/bin/python3`.
  - End with a new line.
  - Be executable.
- **Allowed Editors**: `vi`, `vim`, `emacs`.
- A `README.md` file is mandatory at the root of the project.

---

## Concepts and Resources

### Concepts

1. **Bitwise Operations in Python**:
   - Use bitwise operators (`&`, `|`, `^`, `~`, `<<`, `>>`) to manipulate bits.
   - Learn how to extract specific bits from an integer using masks and shifts.
   - [Python Bitwise Operators](https://wiki.python.org/moin/BitwiseOperators)

2. **UTF-8 Encoding Scheme**:
   - Understand how UTF-8 encodes characters into 1 to 4 bytes.
   - Learn the patterns for each type of UTF-8 encoded character:
     - 1-byte character: `0xxxxxxx`
     - 2-byte character: `110xxxxx 10xxxxxx`
     - 3-byte character: `1110xxxx 10xxxxxx 10xxxxxx`
     - 4-byte character: `11110xxx 10xxxxxx 10xxxxxx 10xxxxxx`
   - [UTF-8 Wikipedia](https://en.wikipedia.org/wiki/UTF-8)
   - [The Absolute Minimum Every Software Developer Must Know About Unicode and Character Sets](https://www.joelonsoftware.com/2003/10/08/the-absolute-minimum-every-software-developer-absolutely-positively-must-know-about-unicode-and-character-sets-no-excuses/)

3. **Data Representation**:
   - Learn how to handle data at the byte level using Python.
   - Use Python’s `int` type to represent and manipulate byte data.

4. **List Manipulation in Python**:
   - Iterate through lists and use indexing to access elements.
   - Use list comprehensions to create and transform lists.
   - [Python Lists](https://docs.python.org/3/tutorial/datastructures.html)

5. **Boolean Logic**:
   - Apply logical operations (`and`, `or`, `not`) to make decisions.

---

## Task Description

### Task 0: UTF-8 Validation

- **Objective**: Write a Python function that determines if a given dataset represents a valid UTF-8 encoding.
- **Prototype**:
  ```python
  def validUTF8(data):
      """
      Determines if a given data set is a valid UTF-8 encoding.
      
      Args:
      data: List of integers, where each integer represents a byte (0-255).
      
      Returns:
      True if data is valid UTF-8 encoding, False otherwise.
      """

