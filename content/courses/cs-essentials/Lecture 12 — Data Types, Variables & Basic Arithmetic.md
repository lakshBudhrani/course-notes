---
title: "Lecture 12 — Data Types, Variables & Basic Arithmetic"
weight: 12
---

# Lecture 12 — Data Types, Variables & Basic Arithmetic  
Instructor: Laksh Budhrani

---

# Lecture 12 — Data Types, Variables & Basic Arithmetic  
Instructor: Laksh Budhrani

## Objectives

1. Learn the basic Python **data types**
2. Understand how to store different types of data in **variables**
3. Learn the four basic **arithmetic operators**
4. Use variables and arithmetic operators to solve simple problems

---

## Objective 1 — Basic Data Types

### Simple Definition

A **data type** tells Python what kind of data a value is.

The four basic data types we will use are:

| Data Type | Meaning        | Example   |
| --------- | -------------- | --------- |
| `int`     | Whole number   | `16`      |
| `float`   | Decimal number | `16.5`    |
| `str`     | Text           | `"Hello"` |
| `bool`    | True or False  | `True`    |

### Examples

```python
age = 16
price = 12.50
name = "John"
is_student = True
```

In this example:

* `age` stores an **integer**
* `price` stores a **float**
* `name` stores a **string**
* `is_student` stores a **boolean**

---

## Objective 2 — Variables

### Simple Definition

A **variable** is a name used to store a value.

```python
age = 16
```

Here:

* `age` is the variable
* `16` is the value stored in the variable

We can use the variable later in our program:

```python
age = 16

print(age)
print(age + 1)
```

Output:

```text
16
17
```

### Variables Can Store Different Data Types

```python
student_name = "Alex"
student_age = 16
student_gpa = 3.5
is_present = True
```

The value stored in a variable determines its data type.

---

## Objective 3 — Basic Arithmetic Operators

Python can be used as a calculator.

The four basic arithmetic operators are:

| Operator | Meaning        | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | `10 + 5` |
| `-`      | Subtraction    | `10 - 5` |
| `*`      | Multiplication | `10 * 5` |
| `/`      | Division       | `10 / 5` |

### Examples

```python
a = 10
b = 5

print(a + b)
print(a - b)
print(a * b)
print(a / b)
```

Output:

```text
15
5
50
2.0
```

---

## Order of Operations

Python follows the normal mathematical order of operations.

We can remember this as **DMAS**:

* **D** — Division
* **M** — Multiplication
* **A** — Addition
* **S** — Subtraction

For example:

```python
result = 10 + 5 * 2
print(result)
```

Output:

```text
20
```

Multiplication happens before addition.

We can use parentheses when we want a calculation to happen first:

```python
result = (10 + 5) * 2
print(result)
```

Output:

```text
30
```

---

## Objective 4 — Using Variables for Calculations

Variables can be used in mathematical expressions.

For example:

```python
price = 25
quantity = 4

total = price * quantity

print(total)
```

Output:

```text
100
```

We can also use the result of one calculation in another calculation:

```python
length = 10
width = 4

area = length * width
cost = area * 2

print(area)
print(cost)
```

Output:

```text
40
80
```

This allows us to solve real-world problems by storing information in variables and using mathematical formulas.

---

## Check Your Knowledge

### 1. Which data type is used to store a whole number?

* A. `float`
* B. `int`
* C. `str`
* D. `bool`

### 2. Which data type is used to store text?

* A. `int`
* B. `float`
* C. `str`
* D. `bool`

### 3. What is the value of `10 + 5 * 2`?

* A. `30`
* B. `25`
* C. `20`
* D. `15`

### 4. Which operator is used for multiplication in Python?

* A. `x`
* B. `×`
* C. `*`
* D. `%`

### 5. What type of value is stored in `price = 12.50`?

* A. `int`
* B. `float`
* C. `str`
* D. `bool`

### 6. What is the purpose of a variable?

* A. To repeat a program
* B. To store a value
* C. To stop a program
* D. To create a loop

---

# Guided Practice

## Question 1 — Rectangle

Write a program that calculates the **area** and **perimeter** of a rectangle.

The program should accept the length and width as input.

$$
A = lw
$$

$$
P = 2(l+w)
$$

---

## Question 2 — Circle

Write a program that calculates the **diameter**, **circumference**, and **area** of a circle.

The program should accept the radius as input.

Use $\pi = 3.14159$.

$$
d = 2r
$$

$$
C = 2\pi r
$$

$$
A = \pi r^2
$$

---

## Question 3 — Five Student Scores

Write a program that accepts the scores of **five students** and calculates their **sum, average, and product**.

$$
Average = \frac{S_1+S_2+S_3+S_4+S_5}{5}
$$

---

# Independent Practice

## Question 1 — Temperature Conversion

Write a program that converts a temperature from **Fahrenheit to Celsius**.

$$
C = (F-32)\times\frac{5}{9}
$$

---

## Question 2 — Simple Interest

Write a program that calculates the **simple interest** and **total amount** for a given principal, annual interest rate, and number of years.

$$
SI = \frac{PRT}{100}
$$

$$
A = P + SI
$$

---

## Question 3 — Shopping Receipt

Write a program that calculates the **subtotal, sales tax, and final total** for an item.

The program should accept the item price, quantity, and sales tax rate.

$$
Subtotal = Price \times Quantity
$$

$$
Tax = Subtotal \times \frac{Rate}{100}
$$

$$
Total = Subtotal + Tax
$$

---

## Notes

* Use variables to store values.
* Use `input()` to get information from the user.
* Remember that `input()` returns a string.
* Use `int()` or `float()` when necessary.
* Use `+`, `-`, `*`, and `/` for basic arithmetic.
* Use parentheses to control the order of operations.
* Use meaningful variable names.

---

## Submission Instructions

Submit your work in Google Classroom by:

1. Creating a **Google Doc**
2. Pasting your code into the document
3. Adding a screenshot of your output
4. Turning in the Google Doc to the appropriate assignment

---