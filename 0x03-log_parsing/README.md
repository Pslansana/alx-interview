# 0x03. Log Parsing

## Description
The **"0x03. Log Parsing"** project focuses on developing a Python script that reads log data from standard input (stdin), processes it in real-time, and outputs specific metrics based on the input. The goal is to practice working with file I/O, real-time data processing, and signal handling in Python.

The log entries follow a specific format, and the script must:
- Parse the log entries.
- Compute the total file size.
- Count occurrences of different HTTP status codes.
- Handle keyboard interruptions (CTRL + C) gracefully, ensuring partial results are displayed before termination.

---

## Requirements
- Allowed editors: `vi`, `vim`, `emacs`
- Files will be interpreted/compiled on **Ubuntu 20.04 LTS** using `python3` (version 3.4.3)
- All files should end with a new line
- The first line of all Python files should be exactly `#!/usr/bin/python3`
- A `README.md` file at the root of the project folder is mandatory
- Code should follow the **PEP 8** style guide (version 1.7.x)
- All files must be executable
- The length of the files will be tested using `wc`

---

## Concepts
### Key Concepts to Understand
1. **File I/O in Python**  
   Learn how to read input line by line using `sys.stdin`. The script should continuously read log data until interrupted.

2. **Signal Handling**  
   Handle keyboard interruptions using `try/except` and display the computed metrics when the program is interrupted by `CTRL + C`.

3. **Data Processing**  
   - Parse each line to extract the file size and HTTP status code.
   - Use regular expressions to validate the format of log entries.
   - Accumulate the total file size and maintain a count of occurrences of each status code.

4. **Dictionaries in Python**  
   Use a dictionary to keep track of the count of each HTTP status code.

5. **Exception Handling**  
   Properly handle exceptions during input processing to prevent the program from crashing due to malformed input.

---

## Log Entry Format
Each log entry is expected to follow this format:


- `<IP Address>`: String representing the IP address.
- `<date>`: Date in the specified format.
- `"GET /projects/260 HTTP/1.1"`: Request line.
- `<status code>`: Integer representing the HTTP status code (e.g., 200, 404).
- `<file size>`: Integer representing the size of the file in bytes.

---

## Script Behavior
1. **Reading Input**  
   The script reads log entries line by line from `stdin`.

2. **Metrics Computation**  
   - The total file size is accumulated across all log entries.
   - The script keeps a count of occurrences of the following status codes:
     - `200`, `301`, `400`, `401`, `403`, `404`, `405`, `500`

3. **Output**  
   Every 10 lines, or upon receiving a keyboard interruption (`CTRL + C`), the script prints the following metrics:
   - Total file size.
   - Count of occurrences for each status code (only codes that appear are printed).

---

## Example Usage
```bash
$ cat logs.txt | ./0-stats.py
Total file size: 2390
200: 5
301: 2
404: 1

