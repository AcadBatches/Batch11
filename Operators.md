# Operators: Pre-Assignment and Overview

## Overview

Operators are fundamental building blocks in programming that enable us to perform operations on variables and values. They are classified into different types based on their functionality, such as arithmetic, comparison, logical, and more. Understanding operators is crucial for solving problems efficiently and writing optimized code.

---

### Types of Operators

1. **Arithmetic Operators**: Perform mathematical operations.
   - Examples: `+`, `-`, `*`, `/`, `%`

2. **Comparison (Relational) Operators**: Compare two values and return a Boolean result.
   - Examples: `==`, `!=`, `>`, `<`, `>=`, `<=`

3. **Logical Operators**: Combine or invert Boolean values.
   - Examples: `&&`, `||`, `!`

4. **Bitwise Operators**: Operate on binary representations of numbers.
   - Examples: `&`, `|`, `^`, `~`, `<<`, `>>`

5. **Assignment Operators**: Assign values to variables.
   - Examples: `=`, `+=`, `-=`, `*=`, `/=`, `%=` 

6. **Ternary Operator**: Short-hand for `if-else`.
   - Syntax: `condition ? value_if_true : value_if_false`

7. **Unary Operators**: Operate on a single operand.
   - Examples: `+`, `-`, `++`, `--`

8. **Special Operators**: Operators like `typeof`, `instanceof` (specific to some languages).

---

## Pre-Assignment Task

### Task: Temperature Conversion and Comparison

Create a program that utilizes **arithmetic**, **comparison**, and **logical operators** to perform the following:

1. **Input**:  
   - Accept a temperature value in **Celsius** (`C`).  
   - Accept another temperature value in **Fahrenheit** (`F`).  

2. **Conversion**:  
   - Convert the Celsius value to Fahrenheit using the formula:  
     \[
     F_{\text{converted}} = (C \times \frac{9}{5}) + 32
     \]

3. **Comparison**:  
   - Compare the converted Fahrenheit value (`F_converted`) with the input Fahrenheit value (`F`) using **comparison operators**.  
   - Print whether the converted temperature is:
     - Equal to the input Fahrenheit.
     - Higher than the input Fahrenheit.
     - Lower than the input Fahrenheit.

4. **Logical Check**:  
   - Check if both temperatures (`F` and `F_converted`) fall within a **comfortable room temperature range** of **60°F to 80°F** using **logical operators**.  
   - Print a message indicating whether both temperatures are within the range.

---


#### Input:
- Enter temperature in Celsius: 25
- Enter temperature in Fahrenheit: 77

#### Output
- Converted Celsius to Fahrenheit: 77.0
