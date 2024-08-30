# Intro

**SF1, Aug 23**

## Topics

- What is a programming language
- What is Python
- Basics of Python

## What is a Programming Language (PL)

- **Computer speak:** The opposite of a natural or human language.
- **Characteristics:**
  - Same as natural languages: syntax and grammar.
  - Very rigid: One wrong move can lead to bugs and errors.
- **Every software** is made via a programming language.
- There are many programming languages:
  - Java
  - C
  - JavaScript
  - Assembly
  - Machine language (binary)

### Types of Programming Languages

1. **Compiled Languages:**
   - Uses a compiler to output a new program in binary.
   - **INPUT:** A program in the given PL (e.g., "myprogram.java").
   - **OUTPUT:** An executable, a new program that is in binary.
   - **Examples:** Java, C, C++, C#

2. **Interpreted Languages:**
   - Reads each line one at a time and converts it into binary, sending it to the CPU.
   - **Examples:** Python, JavaScript

### Questions

- **How are compiled and interpreted processes different?**
  - **Compiler:** Translates code from a high-level programming language into machine code before the program runs.
  - **Interpreter:** Translates code from a high-level programming language into machine code line-by-line as the code runs.

- **Will compiling run a program? Will interpreting run a program?**
  - Compiling produces an executable that does not run the program immediately.
  - Interpreting runs the program immediately.

- **Why would you use one over the other? What are the advantages of either?**
  - **Compiled Languages:** Easier to share code. Generally faster to run.
  - **Interpreted Languages:** Faster to develop code. Different versions (e.g., Python 3.1.7 vs. 3.1.5) will run the same binary code on the CPU.

## What is Python

- **Free and Open Source Software (FOSS, FLOSS):**
  - Always free.
  - Anyone can view and contribute to the source code.
  - **Contrast with:** Closed source, proprietary software like Microsoft products.
  - Python is FOSS but also supported by a company.

- **Python Versions:**
  - Updated over the years.
  - Started with v1, v2 in the 2000s, and v3 today.
  - Differences between versions can be significant, so be cautious.

- **Applications of Python:**
  - Science
  - Data science
  - Industry applications
  - AI
  - Health studies
  - Big pros: Easier to learn, less complex syntax compared to some other languages.

- **Python as a Calculator:**
  - Can perform simple math operations.
  - Uses parentheses to enforce order of operations (PEMDAS).
 
## Expressions and Tracing

- **Expression:** A line of code that can be simplified.
  - **Example:** `4 + 4 * 2`
    1. Evaluate `4 + 8` (one step in the evaluation)
    2. Result: `12` (final value)

- **Expression Evaluation:** An expression is evaluated one step at a time until a final value is reached.

- **Tracing:** The process of manually stepping through the evaluation of an expression to see how it is simplified step-by-step.
  - **Example:** Tracing `x = x + x` where `x = 4`
    1. **Substitute:** Replace variables with their values only on the right side.
       - `x = 4 + 4`
    2. **Result:** `x = 8`


## Order of Operations (OOO)

To evaluate expressions correctly in Python, follow these steps:

1. **Substitution:** Replace variables with their current values.
2. **PEMDAS:** Apply the order of operations:
   - **Parentheses**
   - **Exponents**
   - **Multiplication and Division** (from left to right)
   - **Addition and Subtraction** (from left to right)
3. **Assignment:** Update the variable's value in the lookup table.

---

## Topics

### Review

- **Terms:**
  - **exp** (expression)
  - **eval** (evaluate)
  - **trace** (track)
  - **lookup table** (variable storage)
- **Python as a Calculator:** Python functions similarly to a calculator but with added support for variables.

### New Concepts

- **Data:**
  - **Types:** Classification of data (e.g., integers, floats).
  - **Values:** The actual data being stored (e.g., `4`, `2.0`).
- **Type Function and Print Function:**
  - **`type()`:** Use this function to determine the data type of a value.
  - **`print()`:** Use this function to display the value.
- **Floats and Strings:**
  - **Floats:** Decimal numbers (e.g., `2.0`).
  - **Strings:** Text data (e.g., `"hello"`).

---

## Type

All data in a computer, whether text, numbers, or images, has two fundamental elements:

- **VALUE** || **TYPE**

  Examples:
  - `4`: **Type:** `int`, **Value:** `4`
  - `2.0`: **Type:** `float`, **Value:** `2.0`

Python supports both whole numbers (integers) and decimal numbers (floats), similar to how a calculator works.

### Identifying Value and Type

To identify the type and value of data in Python:

- **Get the Type:** Use the `type()` function.
- **Get the Value:** Use the `print()` function.

  ```python
  number = 4
  print(type(number))  # Output: <class 'int'>
  print(number)        # Output: 4

  decimal = 2.0
  print(type(decimal)) # Output: <class 'float'>
  print(decimal)       # Output: 2.0


# Type Conversion in Python

## Overview

Type conversion allows you to change data from one type to another. While this can be useful, it's important to be aware that some conversions might result in data loss. This section covers the basics of type conversion and provides examples of how to perform conversions using built-in Python functions.

## Why Type Conversion?

Converting data types can be necessary for various operations, but it's essential to understand that:

- **Data Loss:** Some conversions may lead to loss of precision or information. For example:
  - Converting an integer (`3`) to a float (`3.0`) is straightforward and preserves the value.
  - Converting a float (`3.1`) to an integer (`3`) can lead to data loss, as the decimal part is discarded.

## Built-in Functions for Type Conversion

Python provides built-in functions to convert data between types:

- **`int()`**: Converts a value to an integer.
- **`float()`**: Converts a value to a float.
- **`str()`**: Converts a value to a string.

### Examples

#### Converting an Integer to a Float

- **Developer Way:**
  ```python
  x = 4
  x = float(x)  # Converts int 4 to float 4.0
  print(x)      # Output: 4.0
  

- **Hack Way:**
```python
x = 4
x = x + 0.0  # Adding 0.0 to an integer results in a float
print(x)     # Output: 4.0


- **Hack Way:**
- **float** -> int always rounds down
!!BE CAREFUL DATA LOSS

The operation of turning one step to another is called casting. 

new Type string
Python is better than a calculator in that it can opetrate on strings
Strings are texts, words. they "strings" characters together. str for short 





