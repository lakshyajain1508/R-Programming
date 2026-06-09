# Comments in R

Comments are used to **explain code**, **add notes**, and **make programs easier to understand**. Comments are ignored by the R interpreter.

---

## What Are Comments?

A comment is text written inside your code that is meant for humans, not for R.

```r
# This is a comment
print("Hello World")
```

### Output

```text
Hello World
```

---

## Why Use Comments?

Without comments:

```r
a <- 50000
b <- 0.18
c <- a * b
```

With comments:

```r
# Principal Amount
a <- 50000

# Interest Rate
b <- 0.18

# Calculate Interest
c <- a * b
```

---

## Single-Line Comments

R uses `#`.

```r
# Store student name
name <- "Laksh"

print(name)
```

Output:

```text
Laksh
```

---

## Comments After Code

```r
age <- 20   # Student age
print(age)
```

Output:

```text
20
```

---

## Multi-Line Comments

R does not support true multi-line comments.

❌ Invalid:

```r
/*
Not valid in R
*/
```

✅ Use:

```r
# Line 1
# Line 2
# Line 3
```

---

## Disable Blocks Temporarily

```r
if(FALSE){
print("Line 1")
print("Line 2")
}
```

Output:

```text
(No Output)
```

---

## Practical Example

```r
# Student obtained marks
marks <- 90

# Bonus
bonus <- 5

# Final marks
total <- marks + bonus

print(total)
```

Output:

```text
95
```
