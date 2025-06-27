

# Python Functions Notebook

This repository/notebook demonstrates various Python function concepts with examples, including:

- Basic functions and lambda expressions
- Generator functions
- File handling using generators
- Functional programming using `map`, `filter`, `reduce`

---

## 🔧 File Overview

- **Functions.ipynb**: The main Jupyter Notebook containing Python code for:
  - Checking if a number is prime (1–200)
  - Sorting tuples using lambda functions
  - Using `reduce()` to perform a sum operation (step-by-step explanation)
  - Generator function to read a file line-by-line
  - Usage of `map()`, `filter()`, and `reduce()`

---

## 📂 Generator: Reading a File Line-by-Line

```python
def read_lines(filepath):
    with open(filepath, 'r') as file:
        for line in file:
            yield line.rstrip('\n')
