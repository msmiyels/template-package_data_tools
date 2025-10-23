# Python Data Tools Environment Template

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Python Version](https://img.shields.io/badge/python-3.12%2B-blue.svg)](https://www.python.org/downloads/)
[![Status: Alpha](https://img.shields.io/badge/status-alpha-orange.svg)]()

## Overview ✨

This repository provides a modern, ready-to-use environment template for data analysis and geospatial projects in Python. It is designed to help you start your own data science or research project with minimal setup effort. **This repository is intended to be used as a GitHub template when creating a new repository, not for direct cloning.**

Simply use this template when creating your own GitHub repository, then rename the package and folder from `package_name` to your desired project name, and you are ready to go. 🚀<p>
**Keywords:** data science, geospatial, pandas, numpy, scikit-learn

## How to Use This Template 🛠️

1. **Create your new repository using this template on GitHub.**
2. **Rename all occurrences of `package_name`** in the codebase and folder structure to your desired package name.
   
   <details>
   <summary>Where to replace <code>package_name</code>? 🔍</summary>
   
   - <strong>src/package_name/</strong> (folder name)
   - <strong>src/package_name/__init__.py</strong> (file name)
   - <strong>pyproject.toml</strong> (in the <code>packages</code> list and optional dependencies)
   
   </details>
3. **Customize the code and documentation** as needed for your project. 🎨

## Installation

### Using uv (recommended for flexibility and speed) 🚀
- Install [uv](https://docs.astral.sh/uv/) with one of the available methods explained in the docs.

- Install core dependencies:
  ```bash
  uv pip install -e .
  ```
- Install optional groups (e.g., for development or testing):
  ```bash
  uv pip install -e .[dev,test]
  ```
- Install everything (all groups):
  ```bash
  uv pip install -e .[all]
  ```
  (Check `pyproject.toml` for available groups.)

> **Note:** With uv, you can install only the groups you need, keeping your environment lean and fast. ✨

### Using Conda (for compatibility) 🐍
The provided `environment.yml` installs the full environment with all dependencies. Use this only if you require strict Conda compatibility or need all packages at once.
```bash
conda env create -f environment.yml
conda activate data_tools
```

## Usage

The main module is located in `src/package_name` (replace `package_name` with your own project name). Example:
```python
import your_package_name  # Replace with your actual package name
# Continue with your own implementation
```

### Example: Run a Python file using uv 🏃‍♂️

Suppose you have a script called `app.py` in your project root:

1. Navigate to the project root (contains the environment) and open a terminal
2. Run the file :
    ```bash
    uv run main.py
    ```

## Project Structure 🗂️
```
├── environment.yml         # Conda environment (full, for compatibility)
├── pyproject.toml          # Package metadata and pip/uv dependencies
├── src/package_name/       # Main module (rename to your package name)
├── docs/                   # Documentation (placeholder)
├── notebooks/              # Example notebooks (placeholder)
├── tests/                  # Tests (placeholder)
```

The folders `docs/`, `notebooks/`, and `tests/` are provided as placeholders for documentation, example notebooks, and tests. 📚🧪
