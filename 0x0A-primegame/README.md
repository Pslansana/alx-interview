# 0x0A. Prime Game

## Overview

This project involves solving a competitive game scenario using algorithms, prime numbers, and game theory. Maria and Ben play multiple rounds of a game where they take turns picking a prime number and removing it, along with its multiples, from a set of consecutive integers. The player who cannot make a move loses the game.

The objective is to determine the winner for each round and identify the player who wins the most rounds.

---

## Learning Objectives

By completing this project, you will learn how to:
- Implement an API in Python to determine game outcomes.
- Use efficient algorithms to generate prime numbers (e.g., Sieve of Eratosthenes).
- Apply game theory principles to simulate optimal play.
- Optimize performance using dynamic programming and memoization.

---

## Requirements

- **Environment**: Ubuntu 20.04 LTS
- **Python Version**: Python 3.4.3
- **Style Guide**: PEP 8 (version 1.7.x)
- **Mandatory Files**:
  - `README.md`: Documentation for the project.
  - `0-prime_game.py`: Implementation of the solution.
- **Execution**: All scripts must be executable.
- **Shebang**: The first line of all Python files must be `#!/usr/bin/python3`.

---

## Tasks

### 0. Prime Game
**Mandatory**

**Prototype**: `def isWinner(x, nums):`
- `x` (int): Number of rounds.
- `nums` (list of int): List of integers where each integer represents the size of the set for that round.

**Return**: The name of the player with the most wins (`"Maria"` or `"Ben"`), or `None` if there is no winner.

**Constraints**:
- `1 <= x <= 10000`
- `1 <= nums[i] <= 10000`

---

## Example

```python
#!/usr/bin/python3
isWinner = __import__('0-prime_game').isWinner

print("Winner: {}".format(isWinner(5, [2, 5, 1, 4, 3])))

