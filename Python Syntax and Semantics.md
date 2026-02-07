# 🐍 Python for Data Analytics — Basics

## 📌 Topic: Syntax & Semantics

---

## 1️⃣ What is Python?

Python is a high-level, interpreted, dynamically typed programming language widely used in:

- Data Analytics
- Data Science
- Machine Learning
- Automation
- Web Development

---

## 2️⃣ Comments in Python

Comments are used to explain code and are not executed by Python.

### 🔹 Single-Line Comment
Used for short explanations.

```python
# This is a single-line comment
print("Hello World")
```

**➡️ Works in:**
- `.py` files
- Jupyter Notebook (`.ipynb`)

### 🔹 Multi-Line Comment
Used when comments span multiple lines.

```python
"""
This is a multi-line comment
Used for explanations
or documentation
"""
```

**⚠️ Note:**
- Mostly used in `.py` files
- Not commonly used as comments in Jupyter Notebook

---

## 3️⃣ Syntax vs Semantics

### 🔸 Syntax
**Definition:** Syntax refers to the rules of writing code correctly.

👉 Think of syntax like grammar in English.

**✔ Correct syntax:**
```python
age = 32
```

**❌ Incorrect syntax:**
```python
age ==
```

### 🔸 Semantics
**Definition:** Semantics refers to the meaning of the code — what the code does when it runs.

👉 Think of semantics like meaning of a sentence.

**Example:**
```python
age = 32
print(age)
```

**➡️ Meaning:** Store 32 in `age` and print it.

---

## 4️⃣ Basic Syntax Rules in Python

### ✅ Rule 1: Python is Case-Sensitive

```python
name = "Vaish"
Name = "Rao"

print(name)
print(Name)
```

**📌 Output:**
```
Vaish
Rao
```

✔ `name` and `Name` are different variables

### ✅ Rule 2: Indentation (VERY IMPORTANT)
Python uses indentation instead of curly braces `{}`.

📌 Indentation defines blocks of code

```python
age = 32

if age > 30:
    print("Age is greater than 30")
```

- ✔ Indentation usually uses 4 spaces
- ❌ Without indentation → IndentationError

### 🔹 Why Indentation Matters

**Other languages:**
```javascript
if(age > 30) {
   print(age);
}
```

**Python:**
```python
if age > 30:
    print(age)
```

---

## 5️⃣ Indentation Example

```python
if True:
    print("Correct indentation")

    if False:
        print("This will not print")

print("Outside the if block")
```

**📌 Output:**
```
Correct indentation
Outside the if block
```

---

## 6️⃣ Line Continuation

Used when a statement is too long.

### 🔹 Using Backslash `\`

```python
total = 1 + 2 + 3 + \
        4 + 5 + 6

print(total)
```

**📌 Output:**
```
21
```

---

## 7️⃣ Multiple Statements in One Line

Use semicolon `;`

```python
x = 5; y = 10; z = x + y
print(z)
```

**📌 Output:**
```
15
```

⚠️ Use this sparingly (not recommended for clean code).

---

## 8️⃣ Semantics in Python

### 🔹 Variable Assignment

```python
age = 32
name = "Chris"
```

- ✔ Python automatically detects data type
- ✔ No need to declare `int`, `float`, etc.

### 🔹 Type Inference
Python decides the variable type at runtime.

```python
age = 32
print(type(age))
```

**Output:**
```
<class 'int'>
```

```python
name = "Chris"
print(type(name))
```

**Output:**
```
<class 'str'>
```

### 🔹 Dynamic Typing
Same variable can change its type.

```python
var = 10
print(type(var))

var = "Chris"
print(type(var))
```

**📌 Output:**
```
<class 'int'>
<class 'str'>
```

---

## 9️⃣ Common Errors

### ❌ Indentation Error

```python
if age > 30:
print(age)
```

**📌 Error:**
```
IndentationError: expected an indented block
```

**✔ Fix:**
```python
if age > 30:
    print(age)
```

### ❌ Name Error (Undefined Variable)

```python
a = b
```

**📌 Error:**
```
NameError: name 'b' is not defined
```

✔ Always define variables before using them.

---

## 🔟 Summary of What You Learned

- ✔ Single-line & multi-line comments
- ✔ Syntax vs Semantics
- ✔ Case sensitivity
- ✔ Indentation
- ✔ Line continuation
- ✔ Multiple statements
- ✔ Variable assignment
- ✔ Type inference
- ✔ Common syntax errors

---

## 🤝 Contributing

Feel free to contribute to this guide by submitting pull requests or opening issues for improvements.

---

**Happy Learning! 🚀**
