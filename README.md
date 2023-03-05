# Learn Basics Of Python3
Every programmer has a story about how they learned to write their first program.

This repository serves as both a playground and cheatsheet for Python programming. The code examples are available for modification, enabling interactive learning and testing via assertions. The repository provides the option to lint the code and verify it follows the Python code style guide, improving code quality from the start.

Each Python script in the repository follows a similar structure, consisting of a descriptive comment, followed by a test function that provides examples of sub-topics related to the primary topic. Assertions accompany each example, detailing the expected function/statement output.

To use the repository effectively, one should locate the desired topic in the table of contents and review the comments and documentation provided in each script's docstring. The code examples and assertions can then be modified to investigate how things work. Running tests and linting the code provide a final check to ensure the code works correctly and is written appropriately.

The table of contents is organized by topic and provides links to the corresponding scripts. Topics include Getting Started, Operators, Data Types, Control Flow, Functions, and Classes. Each topic is divided into relevant sub-topics, allowing for a more targeted review of concepts.


## How to Use This Repository

Each Python script in this repository has the following structure:

```python
"""Lists  <--- Name of the topic here

# @see: https://www.learnpython.org/en/Lists  <-- Link to further readings goes here

Here might go more detailed explanation of the current topic (i.e. general info about Lists).
"""


def test_list_type():
    """Explanation of sub-topic goes here.
    
    Each file contains test functions that illustrate sub-topics (i.e. lists type, lists methods).
    """
    
    # Here is an example of how to build a list.  <-- Comments here explain the action
    squares = [1, 4, 9, 16, 25]
    
    # Lists can be indexed and sliced. 
    # Indexing returns the item.
    assert squares[0] == 1  # <-- Assertions here illustrate the result.
    # Slicing returns a new list.
    assert squares[-3:] == [9, 16, 25]  # <-- Assertions here illustrate the result.
```

So normally you might want to do the following:

- [Find the topic](#table-of-contents) you want to learn or recap.
- Read comments and/or documentation that is linked in each script's docstring (as in example above). 
- Look at code examples and assertions to see usage examples and expected output.
- Change code or add new assertions to see how things work.
- [Run tests](#testing-the-code) and [lint the code](#linting-the-code) to see if it work and is 
written correctly.

## Table of Contents

1. **Getting Started**
    - [What is Python](src/getting_started/what_is_python.md)
    - [Python Syntax](src/getting_started/python_syntax.md)
    - [Variables](src/getting_started/test_variables.py)
2. **Operators**
    - [Arithmetic Operators](src/operators/test_arithmetic.py) (`+`, `-`, `*`, `/`, `//`, `%`, `**`)
    - [Bitwise Operators](src/operators/test_bitwise.py) (`&`, `|`, `^`, `>>`, `<<`, `~`)
    - [Assignment Operators](src/operators/test_assigment.py) (`=`, `+=`, `-=`, `/=`, `//=` etc.)
    - [Comparison Operator](src/operators/test_comparison.py) (`==`, `!=`, `>`, `<`, `>=`, `<=`)
    - [Logical Operators](src/operators/test_logical.py) (`and`, `or`, `not`)
    - [Identity Operators](src/operators/test_identity.py) (`is`, `is not`)
    - [Membership Operators](src/operators/test_membership.py) (`in`, `not in`)
3. **Data Types**
    - [Numbers](src/data_types/test_numbers.py) (including booleans)
    - [Strings](src/data_types/test_strings.py) and their methods
    - [Lists](src/data_types/test_lists.py) and their methods (including list comprehensions)
    - [Tuples](src/data_types/test_tuples.py)
    - [Sets](src/data_types/test_sets.py) and their methods
    - [Dictionaries](src/data_types/test_dictionaries.py)
    - [Type Casting](src/data_types/test_type_casting.py)
4. **Control Flow**
    - [The `if` statement](src/control_flow/test_if.py)
    - [The `for` statement](src/control_flow/test_for.py) (and `range()` function)
    - [The `while` statement](src/control_flow/test_while.py)
    - [The `try` statements](src/control_flow/test_try.py)
    - [The `break` statement](src/control_flow/test_break.py)
    - [The `continue` statement](src/control_flow/test_continue.py)
5. **Functions**
    - [Function Definition](src/functions/test_function_definition.py) (`def` and `return` statements)
    - [Scopes of Variables Inside Functions](src/functions/test_function_scopes.py) (`global` and `nonlocal` statements)
    - [Default Argument Values](src/functions/test_function_default_arguments.py)
    - [Keyword Arguments](src/functions/test_function_keyword_arguments.py)
    - [Arbitrary Argument Lists](src/functions/test_function_arbitrary_arguments.py)
    - [Unpacking Argument Lists](src/functions/test_function_unpacking_arguments.py) (`*` and `**` statements)
    - [Lambda Expressions](src/functions/test_lambda_expressions.py) (`lambda` statement)
    - [Documentation Strings](src/functions/test_function_documentation_string.py)
    - [Function Annotations](src/functions/test_function_annotations.py)
    - [Function Decorators](src/functions/test_function_decorators.py)
6. **Classes**
    - [Class Definition](src/classes/test_class_definition.py) (`class` statement)
    - [Class Objects](src/classes/test_class_objects.py)
    - [Instance Objects](src/classes/test_instance_objects.py)
    - [Method Objects](src/classes/test_method_objects.py)
    - [Class and Instance Variables](src/classes/test_class_and_instance_variables.py)
    - [Inheritance](src/classes/test_inheritance.py)
    - [Multiple Inheritance](src/classes/test_multiple_inheritance.py)
7. **Modules**
    - [Modules](src/modules/test_modules.py) (`import` statement)
    - [Packages](src/modules/test_packages.py)
8. **Errors and Exceptions**
    - [Handling Exceptions](src/exceptions/test_handle_exceptions.py) (`try` statement)
    - [Raising Exceptions](src/exceptions/test_raise_exceptions.py) (`raise` statement)
9. **Files**
    - [Reading and Writing](src/files/test_file_reading.py) (`with` statement)
    - [Methods of File Objects](src/files/test_file_methods.py)
10. **Additions**
    - [The `pass` statement](src/additions/test_pass.py)
    - [Generators](src/additions/test_generators.py) (`yield` statement)
11. **Brief Tour of the Standard Libraries**
    - [Serialization](src/standard_libraries/test_json.py) (`json` library)
    - [File Wildcards](src/standard_libraries/test_glob.py) (`glob` library)
    - [String Pattern Matching](src/standard_libraries/test_re.py) (`re` library)
    - [Mathematics](src/standard_libraries/test_math.py) (`math`, `random`, `statistics` libraries)
    - [Dates and Times](src/standard_libraries/test_datetime.py) (`datetime` library)
    - [Data Compression](src/standard_libraries/test_zlib.py) (`zlib` library)
12. **User input**
    - [Terminal input](src/user_input/test_input.py) (`input` statement)

## Prerequisites

**Installing Python**

Make sure that you have [Python3 installed](https://realpython.com/installing-python/) on your machine.

You might want to use [venv](https://docs.python.org/3/library/venv.html) standard Python library
to create virtual environments and have Python, pip and all dependent packages to be installed and 
served from the local project directory to avoid messing with system wide packages and their 
versions.

Depending on your installation you might have access to Python3 interpreter either by
running `python` or `python3`. The same goes for pip package manager - it may be accessible either
by running `pip` or `pip3`.

You may check your Python version by running:

```bash
python --version
```

Note that in this repository whenever you see `python` it will be assumed that it is Python **3**.

**Installing dependencies**

Install all dependencies that are required for the project by running:

```bash
pip install -r requirements.txt
```

## Testing the Code

Tests are made using [pytest](https://docs.pytest.org/en/latest/) framework.

You may add new tests for yourself by adding files and functions with `test_` prefix
(i.e. `test_topic.py` with `def test_sub_topic()` function inside).

To run all the tests please execute the following command from the project root folder:

```bash
pytest
```

To run specific tests please execute:

```bash
pytest ./path/to/the/test_file.py
```

## Linting the Code

Linting is done using [pylint](http://pylint.pycqa.org/) and [flake8](http://flake8.pycqa.org/en/latest/) libraries.

### PyLint

To check if the code is written with respect
to [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide please run:

```bash
pylint ./src/
```

In case if linter will detect error (i.e. `missing-docstring`) you may want to read more about 
specific error by running:

```bash
pylint --help-msg=missing-docstring
```

[More about PyLint](http://pylint.pycqa.org/)

### Flake8

To check if the code is written with respect
to [PEP 8](https://www.python.org/dev/peps/pep-0008/) style guide please run:

```bash
flake8 ./src
```

Or if you want to have more detailed output you may run:

```bash
flake8 ./src --statistics --show-source --count
```

[More about Flake8](http://flake8.pycqa.org/en/latest/)

