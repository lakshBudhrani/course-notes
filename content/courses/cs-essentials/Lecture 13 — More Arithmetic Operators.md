---
title: "Lecture 13 — More Arithmetic Operators"
weight: 13
math: true
---

# Lecture 13 — More Arithmetic Operators  
Instructor: Laksh Budhrani

---

## Recall

### Basic Data Types

| Data Type | Meaning        | Example   |
| --------- | -------------- | --------- |
| `int`     | Whole number   | `16`      |
| `float`   | Decimal number | `16.5`    |
| `str`     | Text           | `"Hello"` |
| `bool`    | True or False  | `True`    |

### Basic Arithmetic Operators

| Operator | Meaning        | Example  |
| -------- | -------------- | -------- |
| `+`      | Addition       | `10 + 5` |
| `-`      | Subtraction    | `10 - 5` |
| `*`      | Multiplication | `10 * 5` |
| `/`      | Division       | `10 / 5` |

---

## Objectives

1. Learn the **exponent** operator
2. Learn **floor division**
3. Learn the **modulus** operator
4. Use these operators to solve mathematical and real-world problems

---

## Objective 1 — Exponent

### Simple Definition

The exponent operator `**` is used to raise a number to a power.

```python
result = 2 ** 3
print(result)
```

Output:

```text
8
```

Mathematically:

$$2^3 = 8$$

---

## Objective 2 — Floor Division

### Simple Definition

The floor division operator `//` divides two numbers and returns the **whole-number part** of the result.

```python
result = 17 // 5
print(result)
```

Output:

```text
3
```

Because:

$$17 \div 5 = 3 \quad \text{remainder } 2$$

`//` gives us the number of **complete groups**.

---

## Objective 3 — Modulus

### Simple Definition

The modulus operator `%` gives us the **remainder** after division.

```python
result = 17 % 5
print(result)
```

Output:

```text
2
```

Because:

$$17 \div 5 = 3 \quad \text{remainder } 2$$

So:

- `//` → complete groups
- `%` → remainder

These two operators are especially useful when working with **digits, groups, and time**.

---

## Check Your Knowledge

### 1. Which operator is used to raise a number to a power?

* A. `//`
* B. `%`
* C. `**`
* D. `/`

### 2. What is the result of `17 // 5`?

* A. `2`
* B. `3`
* C. `3.4`
* D. `5`

### 3. What is the result of `17 % 5`?

* A. `2`
* B. `3`
* C. `3.4`
* D. `5`

### 4. What does the `%` operator return?

* A. The quotient
* B. The decimal portion
* C. The remainder
* D. The power

### 5. Which operator would be most useful for finding the number of complete groups?

* A. `/`
* B. `%`
* C. `//`
* D. `**`

### 6. What is the result of the following?

```python
result = 2 ** 4
```

* A. `6`
* B. `8`
* C. `16`
* D. `24`

---

# Guided Practice

## Question 1 — Pythagorean Theorem

Write a program that calculates the **hypotenuse** of a right triangle.

The program should accept the lengths of the two shorter sides of the triangle.

$$
c = \sqrt{a^2 + b^2}
$$

---

## Question 2 — Separating Digits

Write a program that accepts a **five-digit integer** and displays its:

* Ten-thousands digit
* Thousands digit
* Hundreds digit
* Tens digit
* Ones digit

Use arithmetic operators, `//`, and `%`.

---

# Independent Practice

## Question 1 — Distance Between Two Points

Write a program that accepts the coordinates of two points and calculates the distance between them.

$$
d = \sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}
$$

---

## Question 2 — Three-Digit Number Manipulation

Write a program that accepts a **three-digit integer**.

Separate the number into its three digits and calculate:

* Sum of the digits
* Product of the digits

Use arithmetic operators, `//`, and `%`.

---

## Notes

* `**` → exponent
* `//` → whole-number division
* `%` → remainder
* `//` and `%` are useful for separating digits.
* Use `**` when a calculation involves a power.

---

## Submission Instructions

Submit your work in Google Classroom by:

1. Creating a **Google Doc**
2. Pasting your code into the document
3. Adding a screenshot of your output
4. Turning in the Google Doc to the appropriate assignment

---