# Python Syntax Fundamentals

## What is Syntax?
*Syntax* refers to the rules that determine how programs must be structured in a programming language.  
Every language has its own syntax, and Python is no exception. Following these rules ensures that your program runs without errors.

---

## Comments
Comments are notes you add to code to explain what it does. They are **ignored** by the Python interpreter, so they don’t affect program execution.  
Good comments make your code easier to read — not just for others, but also for yourself.  
Trust me: when you return to a piece of code you wrote six months ago, you’ll be grateful for every helpful comment you left behind.

```python
# This is a single-line comment

'''
This is a multi-line comment.
You can explain more details here.
'''
```
---

## Indentation
Unlike many other languages, Python uses indentation to define code blocks.
That means spaces (or tabs) at the beginning of lines are not just style — they are part of the syntax.
```python
# Checking CO2 levels in ppm (parts per million)
co2_levels = [380, 410, 450]

for level in co2_levels:
    if level > 400:
        print("Warning: CO2 above safe threshold!")
    else:
        print("CO2 level is within safe range.")
```
**Indentation must be consistent. Mixing tabs and spaces, or misaligning blocks, will cause errors.**

---

## Whitespace
Extra whitespace within or between lines doesn’t change how Python runs the code.
Its main purpose is readability.

```python
# All of these are equivalent

# Number of trees in two sample plots
trees = 120 + 30

# Total rainfall from two days (mm)
rainfall = 80 + 15

# We can remove the whitespace between the two expressions too
trees = 150+20
rainfall = 95+10
```

---
## The print() Function
The `print()` function is one of the most common built-ins.
It outputs information to the console and always requires parentheses.

```python
print("Welcome to Environmental Data Science!")
# Output: Welcome to Environmental Data Science!
```

---

## Reserved Keywords
Python reserves certain [words](https://docs.python.org/3/library/keyword.html?utm_source=chatgpt.com) that have built-in, special roles in the language - they cannot be used as names for your variables, functions, or classes.  

Here are some of the **hard keywords** (must always be used for their language role):  
`False`, `None`, `True`, `and`, `as`, `assert`, `async`, `await`, `break`, `class`, `continue`, `def`, `del`, `elif`, `else`, `except`, `finally`, `for`, `from`, `global`, `if`, `import`, `in`, `is`, `lambda`, `nonlocal`, `not`, `or`, `pass`, `raise`, `return`, `try`, `while`, `with`, `yield`

Python 3.12 also introduces **soft keywords**:  
`match`, `case`, `_`, `type`

Soft keywords are only keywords in specific contexts; in other contexts, Python might allow them as identifiers.

*Example of what happens if you try to use a reserved keyword:*
```python
class = "forest"
# SyntaxError: invalid syntax
```
**So always avoid naming your variables, functions, or classes using any of these keywords.**
