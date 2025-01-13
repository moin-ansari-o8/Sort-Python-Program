# Sort-Python-Program

## Overview
This Python script is a utility for organizing and sorting the content of Python files. Specifically, it:

- Sorts methods within classes alphabetically.
- Sorts the keys of dictionaries alphabetically.
- Sorts the elements of lists alphabetically.

The script uses the `ast` (Abstract Syntax Tree) module to parse and modify Python code programmatically, ensuring the integrity of the code structure. It also employs the `os` module to handle file operations.

---

## Features

- **Alphabetical Sorting**:
  - Methods inside classes are reordered alphabetically by their names.
  - Dictionary keys are sorted alphabetically.
  - List elements are sorted alphabetically.
- **Non-Destructive Editing**: The original file remains untouched. A new file with the suffix `_sorted` is created.

---

## Installation

Nothing...just need a python in a pc

---

## Usage

1. **Prepare the File**: Place the Python file you want to sort in a directory.
2. **Modify the Script**: Update the `file_path` variable in the script to point to your Python file. For example:
   ```python
   file_path = "z:\\GIT_PROJECTS\\SortPythonProgram.py"
   ```
3. **Run the Script**: Execute the script in your Python environment:
   ```bash
   python sort_methods_and_dicts_in_file.py
   ```
4. **Check Output**: A new file will be created in the same directory as the original file, with `_sorted` appended to its name.

---

## Example

### Input File (`example.py`):
```python
class SampleClass:
    def beta_method(self):
        pass

    def alpha_method(self):
        pass

my_dict = {"b": 2, "a": 1}
my_list = ["z", "y", "x"]
```

### Output File (`example_sorted.py`):
```python
class SampleClass:
    def alpha_method(self):
        pass

    def beta_method(self):
        pass

my_dict = {"a": 1, "b": 2}
my_list = ["x", "y", "z"]
```

---

## How It Works

1. **Parsing the File**: The script reads the target Python file and parses it into an Abstract Syntax Tree (AST).
2. **Sorting Classes and Methods**:
   - Class methods are identified and reordered alphabetically.
3. **Sorting Data Structures**:
   - Dictionaries and lists within the code are sorted alphabetically.
4. **Writing the Output**: The modified AST is written to a new file.

---

## Contributing

Contributions are welcome! If you have ideas for improving the script, feel free to fork the repository and submit a pull request.

---

## License

This project is licensed under the MIT License. See the LICENSE file for more details.

---

## Author

Developed by **Moin Ansari**. Feel free to connect with me on [LinkedIn](https://www.linkedin.com/in/moin-ansari1817/)!

---

