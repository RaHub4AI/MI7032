# R Syntax Fundamentals

## What is Syntax?
*Syntax* refers to the set of rules that define how code must be written so that the R interpreter can understand it.  
Correct syntax ensures that code runs as expected, while incorrect syntax produces errors.

---

## Comments
Comments are notes you add to code to explain what it does. They are **ignored** by the R interpreter, so they don’t affect program execution.  
Good comments make your code easier to read - not just for others, but also for yourself.  
Trust me: when you return to a piece of code you wrote six months ago, you’ll be grateful for every helpful comment you left behind.

```r
# This is a single-line comment
x <- 5   # Assign 5 to variable x
```
*R does not have built-in multi-line comments. If you need longer notes, prefix each line with `#`.*

---

## Strings

Strings can be written using either double quotes `" "` or single quotes `' '`.  
Both forms are valid and equivalent:

```r
name1 <- "River"
name2 <- 'Forest'

print(name1)
# [1] "River"

print(name2)
# [1] "Forest"
```
However:
- It is recommended to stick to one style consistently within a project for readability.
- Mixing them can be useful when a string contains quotes inside it:
```r
sentence1 <- "It's a sunny day"   # easier with double quotes outside
sentence2 <- 'He said: "Welcome to R!"'   # easier with single quotes outside
```
So in practice, `" "` is more common in R code, but `' '` works just as well.
---

## Variables and Their Assignment
A **variable** is a named storage location used to hold values that a program can manipulate.
In R, the most common assignment operator is `<-`, although `=` can also be used in some contexts.
The `<-` operator is considered idiomatic R style.
```r
temperature <- 20   # Assign value 20 to variable 'temperature'
rainfall = 15       # Works too, but less common
```
Variable names in R must follow certain rules:
- They may contain letters, numbers, dots (`.`), and underscores (`_`).  
- They **cannot start** with a number or with an underscore.  
- They **must start** with a letter, or with a dot that is *not* followed by a number.

```r
# Valid variable names
temp <- 25
rainfall_amount <- 120
data.2024 <- c(1, 2, 3)
.data1 <- 5

# Invalid variable names
2day <- 50       # cannot start with a number
_data <- 10      # cannot start with an underscore
.1data <- 5      # cannot start with dot followed by a number
```

---

## Indentation and Whitespace

Unlike Python, R does not rely on indentation to define code blocks.
Instead, blocks are enclosed with curly braces `{}`. Indentation and whitespace are used mainly for readability.

```r
if (temperature > 25) {
  print("It's hot today")
} else {
  print("The temperature is moderate")
}
```
Extra whitespace generally does not affect execution:
```r
a <- 2 + 7
b <- 8+9
```

---

## Reserved Words in R

R has a set of reserved (words)[https://rdrr.io/r/base/Reserved.html] that cannot be used as variable or function names.
These include:
`if`, `else`, `repeat`, `while`, `function`, `for`, `in`, `next`, `break`, `TRUE`, `FALSE`, `NULL`, `Inf`, `NaN`, `NA`, `NA_integer_`, `NA_real_`, `NA_complex_`, `NA_character_`, `...`, and `..1`, `..2` etc.
The special argument `...` (ellipsis) allows you to pass an arbitrary number of arguments into a function.  
It is very common in R, especially in plotting functions and packages that forward arguments.
```r
# A simple function that adds up any number of values
my_sum <- function(...){
  numbers <- c(...)     # collect all arguments into a vector
  sum(numbers)
}

my_sum(1, 2, 3, 4, 5)
# [1] 15
```
Here, `...` collects the arguments `1, 2, 3, 4, 5` and passes them into `c()`.
This makes the function flexible, since it works with any number of inputs.

Another common pattern is forwarding extra arguments to another function:

```r
# A wrapper around plot() that always uses blue points
my_plot <- function(x, y, ...){
  plot(x, y, col = "blue", ...)   # forward additional arguments to plot()
}

my_plot(1:5, 1:5, main = "Custom Plot", pch = 19)
```
Here, `...` passes `main = "Custom Plot"` and `pch = 19` down to `plot()`.
This way, the wrapper stays flexible without redefining every possible option.

**So always avoid naming your variables, functions, or classes using any of these keywords.**
