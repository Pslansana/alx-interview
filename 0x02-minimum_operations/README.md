# 0x02. Minimum Operations

## Description
In this project, the goal is to write an efficient algorithm to determine the minimum number of operations required to achieve exactly `n` characters in a text file, starting with a single character `H`. The operations available are:

1. **Copy All**: Copies the entire content of the text file.
2. **Paste**: Pastes the previously copied content.

The challenge is to calculate the minimum number of operations needed to get exactly `n` characters using these operations.

---

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- All files will be interpreted/compiled on **Ubuntu 20.04 LTS** using `python3` (version 3.4.3)
- All files should end with a new line
- The first line of all Python files should be exactly `#!/usr/bin/python3`
- Code should be documented
- Code should follow the **PEP 8** style guide (version 1.7.x)
- All files must be executable
- A `README.md` file at the root of the project folder is mandatory

---

## Concepts
### Key Concepts to Understand
1. **Prime Factorization**  
   The solution can be derived by reducing the problem to finding the sum of the prime factors of the given number `n`. Each prime factor corresponds to a "Copy All" operation followed by a series of "Paste" operations.

2. **Dynamic Programming**  
   Dynamic programming can help solve the problem by breaking it into subproblems and building up a solution incrementally.

3. **Greedy Algorithms**  
   A greedy approach can also be employed by choosing the optimal action (Copy All or Paste) at each step to minimize the number of operations.

---

## Prototype
```python
def minOperations(n):
    """
    Calculate the minimum number of operations to get exactly n 'H' characters.
    
    Parameters:
        n (int): The target number of characters
        
    Returns:
        int: Minimum number of operations required to reach n characters, or 0 if impossible
    """

