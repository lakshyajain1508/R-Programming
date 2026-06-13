# Operators in R

Operators are special symbols that tell R to perform a specific operation.

Think of operators as the **action words** of programming.

For example:

```r
5 + 3
```

Here:

* `5` and `3` are operands
* `+` is the operator

R performs the addition and returns:

```text
8
```

---

# Types of Operators in R

There are mainly 5 types of operators:

1. Arithmetic Operators
2. Relational Operators
3. Logical Operators
4. Assignment Operators
5. Miscellaneous Operators

---

# 1. Arithmetic Operators

Used for mathematical calculations.

| Operator | Meaning          | Example  |
| -------- | ---------------- | -------- |
| +        | Addition         | 5 + 3    |
| -        | Subtraction      | 5 - 3    |
| *        | Multiplication   | 5 * 3    |
| /        | Division         | 10 / 2   |
| ^        | Power            | 2 ^ 3    |
| %%       | Modulus          | 10 %% 3  |
| %/%      | Integer Division | 10 %/% 3 |

---

## Addition (+)

```r
num1 <- 10
num2 <- 20

result <- num1 + num2

print(result)
```

### Output

```text
30
```

### Practical Example: Student Marks

```r
math <- 90
science <- 85

total <- math + science

print(total)
```

### Output

```text
175
```

---

## Subtraction (-)

```r
salary <- 50000
expenses <- 15000

savings <- salary - expenses

print(savings)
```

### Output

```text
35000
```

### Practical Example: Monthly Budget

```r
income <- 40000
rent <- 12000

remaining <- income - rent

print(remaining)
```

### Output

```text
28000
```

---

## Multiplication (*)

```r
price <- 500
quantity <- 4

total <- price * quantity

print(total)
```

### Output

```text
2000
```

### Practical Example: Shopping Cart

```r
book_price <- 250
books <- 5

bill <- book_price * books

print(bill)
```

### Output

```text
1250
```

---

## Division (/)

```r
total_marks <- 450
subjects <- 5

average <- total_marks / subjects

print(average)
```

### Output

```text
90
```

### Practical Example: Calculate Average

```r
marks <- 360
subjects <- 4

avg <- marks / subjects

print(avg)
```

### Output

```text
90
```

---

## Power (^)

Used to calculate exponents.

```r
2 ^ 3
```

### Output

```text
8
```

### Practical Example: Square Area Formula

```r
side <- 5

area <- side ^ 2

print(area)
```

### Output

```text
25
```

---

## Modulus (%%)

Returns the remainder.

```r
10 %% 3
```

### Output

```text
1
```

### Practical Example: Check Even or Odd

```r
number <- 12

number %% 2
```

### Output

```text
0
```

Since the remainder is `0`, the number is even.

---

## Integer Division (%/%)

Returns only the whole number part.

```r
10 %/% 3
```

### Output

```text
3
```

Because:

```text
10 ÷ 3 = 3.33
```

Integer division removes the decimal part.

---

# Mini Project: Student Percentage Calculator

```r
math <- 85
science <- 90
english <- 80

total <- math + science + english

percentage <- total / 3

print(total)
print(percentage)
```

### Output

```text
255
85
```

---

# 2. Relational Operators

Used to compare values.

The result is always:

```text
TRUE
```

or

```text
FALSE
```

| Operator | Meaning               |
| -------- | --------------------- |
| >        | Greater Than          |
| <        | Less Than             |
| >=       | Greater Than or Equal |
| <=       | Less Than or Equal    |
| ==       | Equal To              |
| !=       | Not Equal To          |

---

## Greater Than (>)

```r
10 > 5
```

### Output

```text
TRUE
```

---

## Less Than (<)

```r
5 < 10
```

### Output

```text
TRUE
```

---

## Equal To (==)

```r
10 == 10
```

### Output

```text
TRUE
```

### Important

```r
=
```

is assignment.

```r
==
```

is comparison.

---

## Not Equal To (!=)

```r
10 != 5
```

### Output

```text
TRUE
```

---

### Practical Example: Voting Eligibility

```r
age <- 20

age >= 18
```

### Output

```text
TRUE
```

---

### Practical Example: Exam Result

```r
marks <- 35

marks >= 40
```

### Output

```text
FALSE
```

Student failed.

---

# 3. Logical Operators

Used when multiple conditions are involved.

| Operator | Meaning |
| -------- | ------- |
| &        | AND     |
| |        | OR      |
| !        | NOT     |

---

## AND (&)

Both conditions must be TRUE.

```r
TRUE & TRUE
```

### Output

```text
TRUE
```

```r
TRUE & FALSE
```

### Output

```text
FALSE
```

### Practical Example: College Admission

```r
marks <- 85
attendance <- 80

marks >= 75 & attendance >= 75
```

### Output

```text
TRUE
```

---

## OR (|)

At least one condition must be TRUE.

```r
TRUE | FALSE
```

### Output

```text
TRUE
```

### Practical Example: Scholarship Eligibility

```r
marks <- 90
sports <- FALSE

marks >= 85 | sports
```

### Output

```text
TRUE
```

---

## NOT (!)

Reverses the result.

```r
!TRUE
```

### Output

```text
FALSE
```

### Practical Example

```r
is_logged_in <- TRUE

!is_logged_in
```

### Output

```text
FALSE
```

---

# 4. Assignment Operators

Used to assign values.

## Left Assignment

```r
x <- 10
```

Most commonly used.

---

## Equal Sign

```r
x = 10
```

Also valid.

---

## Right Assignment

```r
10 -> x
```

Rarely used.

---

# 5. Miscellaneous Operators

## Colon Operator (:)

Creates sequences.

```r
1:10
```

### Output

```text
1 2 3 4 5 6 7 8 9 10
```

### Practical Example: Print Numbers

```r
for(i in 1:5){
  print(i)
}
```

### Output

```text
1
2
3
4
5
```

---

## Membership Operator (%in%)

Checks if a value exists.

```r
5 %in% c(1,2,3,4,5)
```

### Output

```text
TRUE
```

### Practical Example: Check Student Roll Number

```r
roll_numbers <- c(101,102,103,104)

102 %in% roll_numbers
```

### Output

```text
TRUE
```

---

# Real-World Mini Project

## Online Shopping Bill Calculator

```r
product_price <- 1500
quantity <- 3

subtotal <- product_price * quantity

gst <- subtotal * 0.18

final_bill <- subtotal + gst

print(subtotal)
print(gst)
print(final_bill)
```

### Output

```text
4500
810
5310
```

---

# Interview Questions

### What is the difference between `=` and `==`?

```r
=
```

Assigns values.

```r
==
```

Compares values.

---

### Which operator returns the remainder?

```r
%%
```

---

### Which operator checks membership?

```r
%in%
```

---

### Which operator performs exponentiation?

```r
^
```

---

# Practice Exercises

## Exercise 1

Calculate:

```r
50 + 20
50 - 20
50 * 20
50 / 20
```

---

## Exercise 2

Check whether:

```r
25 > 18
```

---

## Exercise 3

Check if:

```r
105 %in% c(101,102,103,104,105)
```

---

## Exercise 4

Create a Shopping Bill Calculator

Input:

```r
price <- 200
quantity <- 5
```

Calculate:

* Subtotal
* GST (18%)
* Final Bill

---

# Key Takeaways

* Arithmetic operators perform calculations.
* Relational operators compare values and return TRUE/FALSE.
* Logical operators combine conditions.
* Assignment operators store values.
* Miscellaneous operators help create sequences and search values.
* Operators are used in almost every R program.