# 🐍 Python Variables — Complete Guide

## 📌 Overview

Variables are fundamental elements in programming used to store data that can be referenced and manipulated in a program. In Python, variables are created when you assign a value to them, and they do not need explicit declaration to reserve memory space. The declaration happens automatically when you assign a value to a variable.

---

## 📖 Table of Contents

- [Introduction to Variables](#introduction-to-variables)
- [Declaring and Assigning Variables](#declaring-and-assigning-variables)
- [Naming Conventions](#naming-conventions)
- [Understanding Variable Types](#understanding-variable-types)
- [Type Checking and Conversion](#type-checking-and-conversion)
- [Dynamic Typing](#dynamic-typing)
- [Practical Examples](#practical-examples)
- [Common Errors](#common-errors)

---

## 1️⃣ Introduction to Variables

Variables are containers for storing data values. Unlike other programming languages, Python has no command for declaring a variable. A variable is created the moment you first assign a value to it.

---

## 2️⃣ Declaring and Assigning Variables

In Python, you can assign values to variables directly without declaring their type.

```python
# Simple variable assignment
a = 100

# Multiple variable declarations
age = 32
height = 6.1
name = "Krish"
is_student = True

# Printing the variables
print("age :", age)
print("Height:", height)
print("Name:", name)
```

**Output:**
```
age : 32
Height: 6.1
Name: Krish
```

---

## 3️⃣ Naming Conventions

### ✅ Rules for Variable Names

1. Variable names should be **descriptive**
2. Must start with a **letter** or an **underscore (_)**
3. Can contain letters, numbers, and underscores
4. Variable names are **case-sensitive**
5. Cannot use Python reserved keywords

### Valid Variable Names ✔

```python
first_name = "Krish"
last_name = "Naik"
age_2 = 30
_private_var = "hidden"
```

### Invalid Variable Names ❌

```python
# These will cause SyntaxError
2age = 30              # Cannot start with a number
first-name = "Krish"   # Cannot use hyphens
@name = "Krish"        # Cannot use special characters
```

### Case Sensitivity

```python
name = "Krish"
Name = "Naik"

# These are TWO different variables!
print(name)  # Output: Krish
print(Name)  # Output: Naik
```

---

## 4️⃣ Understanding Variable Types

Python is **dynamically typed**, meaning the type of a variable is determined at runtime.

### Common Data Types

```python
age = 25              # int (Integer)
height = 6.1          # float (Floating-point number)
name = "Krish"        # str (String)
is_student = True     # bool (Boolean)

# Check the type of a variable
print(type(name))     # Output: <class 'str'>
print(type(age))      # Output: <class 'int'>
print(type(height))   # Output: <class 'float'>
print(type(is_student))  # Output: <class 'bool'>
```

---

## 5️⃣ Type Checking and Conversion

### Type Checking

```python
height = 6.1
print(type(height))  # Output: <class 'float'>
```

### Type Conversion (Type Casting)

You can convert variables from one type to another.

#### Converting Integer to String

```python
age = 25
print(type(age))       # Output: <class 'int'>

# Convert to string
age_str = str(age)
print(age_str)         # Output: 25
print(type(age_str))   # Output: <class 'str'>
```

#### Converting String to Integer

```python
age = '25'
print(type(int(age)))  # Output: <class 'int'>
```

#### Invalid Conversion ❌

```python
name = "Krish"
int(name)  # ValueError: invalid literal for int() with base 10: 'Krish'
```

You cannot convert non-numeric strings to integers!

#### Converting Float to Integer and Back

```python
height = 5.11
print(type(height))         # Output: <class 'float'>

# Convert to int (loses decimal part)
height_int = int(height)    # 5

# Convert back to float
float(int(height))          # Output: 5.0
```

---

## 6️⃣ Dynamic Typing

Python allows the type of a variable to **change** as the program executes.

```python
# Start as an integer
var = 10
print(var, type(var))  # Output: 10 <class 'int'>

# Change to a string
var = "Hello"
print(var, type(var))  # Output: Hello <class 'str'>

# Change to a float
var = 3.14
print(var, type(var))  # Output: 3.14 <class 'float'>
```

---

## 7️⃣ Practical Examples

### Example 1: User Input

```python
# Taking user input (always returns a string by default)
age = int(input("What is the age? "))
print(age, type(age))
```

**Note:** The `input()` function always returns a **string**. Use `int()` or `float()` to convert it to a number.

### Example 2: Simple Calculator

```python
# Simple calculator
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

sum = num1 + num2
difference = num1 - num2
product = num1 * num2
quotient = num1 / num2

print("Sum:", sum)
print("Difference:", difference)
print("Product:", product)
print("Quotient:", quotient)
```

**Sample Output:**
```
Enter first number: 56
Enter second number: 10
Sum: 66.0
Difference: 46.0
Product: 560.0
Quotient: 5.6
```

---

## 8️⃣ Common Errors

### 1. SyntaxError - Invalid Variable Name

```python
@name = "Krish"  # SyntaxError: invalid syntax
```

### 2. ValueError - Invalid Type Conversion

```python
name = "Krish"
int(name)  # ValueError: invalid literal for int()
```

### 3. NameError - Using Undefined Variable

```python
print(undefined_variable)  # NameError: name 'undefined_variable' is not defined
```

---

## 🎯 Key Takeaways

- ✅ Variables store data and don't require explicit type declaration
- ✅ Variable names must follow specific naming rules
- ✅ Python is case-sensitive (`name` ≠ `Name`)
- ✅ Use `type()` to check variable type
- ✅ Use `int()`, `float()`, `str()` for type conversion
- ✅ Python supports dynamic typing (variables can change types)
- ✅ `input()` always returns a string—convert as needed

---

## 📚 Summary

Variables are essential in Python programming for storing and manipulating data. Understanding how to declare, assign, and use variables effectively is crucial for writing functional and efficient code. Following proper naming conventions and understanding variable types will help in maintaining readability and consistency in your code.

---

## 🤝 Contributing

Feel free to contribute to this guide by submitting pull requests or opening issues for improvements.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

**Happy Coding! 🚀**
