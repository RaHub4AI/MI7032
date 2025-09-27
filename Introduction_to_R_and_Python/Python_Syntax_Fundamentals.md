# Python Syntax Fundamentals

## What is Syntax?
*Syntax* refers to the rules that determine how programs must be structured in a programming language.  
Every language has its own syntax, and Python is no exception. Following these rules ensures that your program runs without errors.

---

## Comments
Comments are notes you add to code to explain what it does. They are **ignored** by the Python interpreter, so they don’t affect program execution.  
Good comments make your code easier to read - not just for others, but also for yourself.  
Trust me: when you return to a piece of code you wrote six months ago, you’ll be grateful for every helpful comment you left behind.

```python
# This is a single-line comment

'''
This is a multi-line comment.
You can explain more details here.
'''
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

## Strings
Strings in Python can be written using either double quotes `" "` or single quotes `' '`.  
Both forms are valid and equivalent:

```python
name1 = "River"
name2 = 'Forest'

print(name1)   # River
print(name2)   # Forest
```
However:
- It is best to choose one style and stick to it for consistency in a project.
- Using both can be helpful when your string contains quotes:
```python
sentence1 = "It's a sunny day"          # easier with double quotes outside
sentence2 = 'He said: "Welcome to Python!"'  # easier with single quotes outside
```
Python also supports multi-line strings using triple quotes:
```python
paragraph = """This is a
multi-line string
spanning several lines."""
print(paragraph)
```
#### f-Strings (Formatted Strings)
Python 3.6+ introduced f-strings, a powerful and readable way to embed variables or expressions inside strings.
Prefix the string with `f` and use `{}` to insert values:
```python
temperature = 22
print(f"The temperature today is {temperature} °C")
# Output: The temperature today is 22 °C

# You can also use expressions inside {}
print(f"In five years: {temperature + 5} °C")
# Output: In five years: 27 °C
```

---

## Variables
Variables are **named containers** used to store data.  
We define a name and attach a value to it - the variable then acts as a reference to that data.  
You can think of variables as **boxes** that can hold different kinds of information: text, numbers, logical values, or even complex data structures.
Python is a **dynamically typed language**. This means you don’t need to declare the type of a variable explicitly.  
Instead, Python figures it out automatically when you assign a value.  
You can also change the value later, and Python will keep track of the type for you.  
*However, be mindful when reassigning variables - changing the value may cause unintended results if done carelessly.*

```python
# Assigning a string
location = "Stockholm"

# Assigning a boolean (truth value)
raining_outside = True

# Assigning an integer
n_trees = 52
```
Python variable names must follow these rules:
- Allowed characters: letters, digits, and underscores (`_`).
- Must start with a letter or an underscore, not a digit.
- Cannot contain spaces or hyphens (`-`).
- Cannot use [Python reserved keywords](#reserved-keywords).

To avoid mistakes, Python follows a naming convention from the [PEP 8 style guide](https://peps.python.org/pep-0008/):
- `snake_case` → recommended for variables and functions. All the words are in lowercase, and different words are joined together by an underscore.
- `PascalCase` → typically used for class names. The words are joined together without spaces between them, and every first letter of every word is capitalized.
- `camelCase` → rarely used in Python, but common in other languages. The words are joined together without spaces between them; the first word is all lowercase, and all the first letters of all subsequent words are in uppercase.

#### Constants
Constants are like variables, but their values are not supposed to change during program execution.
Technically, Python does not enforce immutability - you can reassign a constant - but by convention, programmers treat them as fixed values.
Based on Python style guide:
- Constants are written in all uppercase letters.
- Use underscores _ to separate words if needed.
```python
E = 2.71828
PI = 3.14159
LENGTH = 100
WIDTH = 50
LOCAL_MINIMUM = 0.5
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
