# Variables and Data Types in R

Variables are the **foundation of programming**.

Think of a variable as a **container** that stores information.

---

## What is a Variable?

A variable is a named location in memory used to store data.

```r
name <- "Laksh"
```

- `name` = Variable Name
- `"Laksh"` = Value
- `<-` = Assignment Operator

---

## Creating Variables

```r
name <- "Laksh"
age <- 20
salary <- 50000

print(name)
print(age)
print(salary)
```

---

## Assignment Operators

```r
x <- 10
x = 10
10 -> x
```

---

## Variable Naming Rules

Valid:

```r
student_age <- 20
salary2026 <- 50000
```

Invalid:

```r
2name <- "Laksh"
student age <- 20
if <- 10
```

---

## Data Types in R

| Data Type | Example |
|----------|---------|
| Numeric | 10.5 |
| Integer | 10L |
| Character | "Laksh" |
| Logical | TRUE |
| Complex | 2+3i |

---

## Numeric

```r
price <- 99.99
class(price)
```

Output:

```text
numeric
```

---

## Integer

```r
age <- 20L
class(age)
```

Output:

```text
integer
```

---

## Character

```r
name <- "Laksh"
class(name)
```

Output:

```text
character
```

---

## Logical

```r
is_student <- TRUE
class(is_student)
```

Output:

```text
logical
```

---

## Complex

```r
x <- 2 + 3i
class(x)
```

Output:

```text
complex
```

---

## Type Conversion

```r
as.character(20)
as.numeric("20")
as.integer(10)
as.logical(1)
```

---

## Practical Example

```r
student_name <- "Laksh"
student_age <- 20L
student_marks <- 92.5
is_passed <- TRUE
```


