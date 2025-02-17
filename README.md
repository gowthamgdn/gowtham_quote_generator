# gowtham_quote_generator

## Overview
gowtham_quote_generatore is a simple Python package that provides motivational quotes. It includes a single function `get_quote()` that returns a random inspirational message.

## Project Structure
```
my_package/
│── gowtham_quote_generator/
│   ├── __init__.py  # Initializes the package
│   ├── main.py      # Contains the get_quote function
│── testing/
│   ├── main.py  # Contains test cases for the package
│── setup.py
│── requirements.txt  # Lists package dependencies
│── README.md
```

- `__init__.py`: Initializes the package.
- `main.py`: Contains the `get_quote()` function.
- `testing/main.py`: Contains test cases for the package.
- `setup.py`: Defines package metadata and dependencies.
- `requirements.txt`: Contains necessary dependencies for installation.
- `README.md`: Documentation for the package.

## Installation
To install the package, use:
```bash
pip install .
```

To install dependencies from `requirements.txt`, run:
```bash
pip install -r requirements.txt
```

To create a distributable package, run:
```bash
python setup.py sdist bdist_wheel
```
This will generate a package file in the `dist/` directory.

## Usage
After installation, you can use the package as follows:
```python
from my_package.main import get_quote

print(get_quote())
```
This will print a random motivational quote.

## Testing
To test the installation, you can run:
```bash
python -c "from my_package.main import get_quote; print(get_quote())"
```
This should output a random quote from the list.

To run automated tests:
```bash
python -m unittest discover -s testing
```
This will execute all test cases in the `testing/` directory.

## Requirements
This package requires:
- Python 3.x

## Notes
- Ensure `setup.py` contains the correct `packages` and `install_requires` fields.
- Always install dependencies using `requirements.txt` to avoid version conflicts.
- If issues occur, check dependencies and Python version.

## Author
Gowtham Tadavarthy

## License
This project is licensed under the MIT License.

