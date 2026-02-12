# Real-World Examples Using Lists in Python

A practical guide demonstrating how to use Python lists through real-world scenarios. This repository contains a Jupyter notebook with hands-on examples that showcase the versatility and power of Python lists in everyday programming tasks.

## Overview

Lists are one of the most commonly used data structures in Python, thanks to their versatility and ease of use. This tutorial provides practical examples that you can apply to real-world programming challenges.

## Examples Included

### 1. Managing a To-Do List
Learn how to create and manage a task list with operations like:
- Adding new tasks
- Removing completed tasks
- Checking for specific tasks
- Iterating through remaining tasks

```python
to_do_list = ["Buy Groceries", "Clean the house", "Pay bills"]

# Adding new tasks
to_do_list.append("Schedule meeting")
to_do_list.append("Go For a Run")

# Removing a completed task
to_do_list.remove("Clean the house")

# Checking if a task is in the list
if "Pay bills" in to_do_list:
    print("Don't forget to pay the utility bills")

print("To Do List remaining")
for task in to_do_list:
    print(f"-{task}")
```

**Output:**
```
Don't forget to pay the utility bills
To Do List remaining
-Buy Groceries
-Pay bills
-Schedule meeting
-Go For a Run
```

### 2. Organizing Student Grades
Work with numerical data to:
- Store and manage student grades
- Calculate average grades
- Find highest and lowest grades
- Perform statistical operations

```python
# Organizing student grades
grades = [85, 92, 78, 90, 88]

# Adding a new grade
grades.append(95)

# Calculating the average grade
average_grade = sum(grades) / len(grades)
print(f"Average Grade: {average_grade:.2f}")

# Finding the highest and lowest grades
highest_grade = max(grades)
lowest_grade = min(grades)
print(f"Highest Grade: {highest_grade}")
print(f"Lowest Grade: {lowest_grade}")
```

**Output:**
```
Average Grade: 88.00
Highest Grade: 95
Lowest Grade: 78
```

### 3. Managing an Inventory
Implement a simple inventory system to:
- Track items in stock
- Add new inventory items
- Remove out-of-stock items
- Check item availability

```python
# Managing an inventory
inventory = ["apples", "bananas", "oranges", "grapes"]

# Adding a new item
inventory.append("strawberries")

# Removing an item that is out of stock
inventory.remove("bananas")

# Checking if an item is in stock
item = "oranges"
if item in inventory:
    print(f"{item} are in stock.")
else:
    print(f"{item} are out of stock.")

# Printing the inventory
print("Inventory List:")
for item in inventory:
    print(f"- {item}")
```

**Output:**
```
oranges are in stock.
Inventory List:
- apples
- oranges
- grapes
- strawberries
```

### 4. Collecting User Feedback
Analyze user feedback by:
- Storing user comments
- Counting positive feedback
- Processing and displaying feedback data
- Performing sentiment analysis

```python
# Collecting user feedback
feedback = ["Great service!", "Very satisfied", "Could be better", "Excellent experience"]

# Adding new feedback
feedback.append("Not happy with the service")

# Counting specific feedback
positive_feedback_count = sum(1 for comment in feedback if "great" in comment.lower() or "excellent" in comment.lower())
print(f"Positive Feedback Count: {positive_feedback_count}")

# Printing all feedback
print("User Feedback:")
for comment in feedback:
    print(f"- {comment}")
```

**Output:**
```
Positive Feedback Count: 2
User Feedback:
- Great service!
- Very satisfied
- Could be better
- Excellent experience
- Not happy with the service
```

## Learning Outcomes

After working through these examples, you'll be able to:
- Create and manipulate lists effectively
- Use common list methods (append, remove, etc.)
- Iterate through lists using for loops
- Apply list operations to solve practical problems
- Understand when to use lists in your programs


