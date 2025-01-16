# 0x01. Lockboxes

## Algorithm | Python

### Description
In this project, you are presented with `n` locked boxes, each numbered from `0` to `n - 1`. Each box may contain keys that unlock other boxes. The goal is to determine if all the boxes can be opened, starting with the first box (`boxes[0]`), which is initially unlocked.

### Requirements
- You need to implement a Python function `canUnlockAll` that checks if all boxes can be opened.
- Each key is represented by a positive integer, where the key `k` unlocks the box with index `k`.
- Some keys may not correspond to any box.
- All keys are assumed to be positive integers.

### Prototype
```python
def canUnlockAll(boxes):
    """
    Determines if all boxes can be unlocked given a list of lists of keys.
    
    Args:
    - boxes (list of list of int): The list where each element is a list of keys in a box.
    
    Returns:
    - bool: True if all boxes can be opened, False otherwise.
    """

