# CSV File Consistency Checker

## Overview

This Python script is designed to check the consistency of CSV files in a specified directory. The script verifies that each line in the file contains exactly five comma-separated values (CSV format). If any file contains lines with a different number of values, it is flagged as inconsistent. Additionally, the script can automatically repair these inconsistent files by removing lines that do not meet the criteria.

## Features

- **Check File Consistency**: Validates that every line in a file contains exactly five comma-separated values.
- **List Inconsistent Files**: Identifies and lists files that do not meet the consistency criteria.
- **Repair Inconsistent Files**: Automatically removes inconsistent lines from flagged files.

## Usage

### 1. Update Directory Path

Modify the `directory_path` variable in the script to reflect the path to your directory containing CSV files.

```python
directory_path = r"C:\machine learning\datasets"  # Replace with your actual directory path
```
### 2. Run the Script

- Execute the script using a Python interpreter:
```bash
python script_name.py
```

### 3. Script Output

- If all files are consistent, the script outputs:
```
All files are consistent.
```
- If inconsistent files are found, their names are listed, and the script attempts to repair them.

### 4. Repair Process

- The script repairs files by removing lines that do not contain exactly five comma-separated values.
```bash
directory_path = r"C:\machine learning\datasets"  # Update with your directory path
```

## Error Handling

- The script includes basic error handling to manage issues that may occur during file reading and writing. Errors are printed to the console.

## Dependencies

- The script is self-contained and does not require any external Python packages.
- It is compatible with Python 3.x.