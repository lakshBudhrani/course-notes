---
title: "Lecture 14 — Variables & Arithmetic Review Project"
weight: 14
math: true
---

# Lecture 14 — Variables & Arithmetic Review Project  
Instructor: Laksh Budhrani

---

## Recall

### Data Types

| Data Type | Meaning        | Example   |
| --------- | -------------- | --------- |
| `int`     | Whole number   | `16`      |
| `float`   | Decimal number | `16.5`    |
| `str`     | Text           | `"Hello"` |
| `bool`    | True or False  | `True`    |

### Arithmetic Operators

| Operator | Meaning             | Example   |
| -------- | ------------------- | --------- |
| `+`      | Addition            | `10 + 5`  |
| `-`      | Subtraction         | `10 - 5`  |
| `*`      | Multiplication      | `10 * 5`  |
| `/`      | Division            | `10 / 5`  |
| `**`     | Exponent            | `2 ** 3`  |
| `//`     | Floor Division      | `17 // 5` |
| `%`      | Modulus / Remainder | `17 % 5`  |

**Remember:**

* `//` gives the number of complete groups.
* `%` gives the remainder.
* `**` is used for powers.
* Python follows the order of operations when evaluating expressions.

---

## Instructions

Write a Python program for each problem.

Your programs should:

* Use variables to store values.
* Use `input()` to get information from the user.
* Convert input to the appropriate data type when necessary.
* Use arithmetic operators to perform the calculations.
* Display the final results clearly.

**Do not use conditionals, loops, lists, or functions.**

---

## 1. Movie Theater Revenue — 4 points

Write a program that accepts the following information:

* Price of an adult ticket
* Number of adult tickets
* Price of a child ticket
* Number of child tickets

Calculate and display the **total revenue** from the ticket sales.

---

## 2. Car Trip Calculator — 4 points

Write a program that accepts:

* Distance of a trip in miles
* Car's miles per gallon (MPG)
* Price of gasoline per gallon

Calculate and display:

* Number of gallons of gasoline needed
* Total cost of gasoline for the trip

Use:

$$\text{Gallons} = \frac{\text{Distance}}{\text{MPG}}$$

$$\text{Cost} = \text{Gallons} \times \text{Price}$$

---

## 3. Number Reversal — 4 points

Write a program that accepts a **three-digit integer** and displays the number with its digits reversed.

For example:

```text
Input: 472
Output: 274
```

Use `//` and `%` to separate the digits.

**Do not convert the number to a string.**

---

## 4. Kinetic Energy — 4 points

Write a program that accepts the **mass of an object in kilograms** and its **velocity in meters per second**.

Calculate and display the object's **kinetic energy in joules**.

$$KE = \frac{1}{2}mv^2$$

---

## 5. Square and Cube Calculator — 4 points

Write a program that accepts a number from the user.

Calculate and display:

* The square of the number
* The cube of the number
* The fourth power of the number

Use the exponent operator `**`.

---

## Bonus: Time Conversion — 2 points

Write a program that accepts a total number of **seconds**.

Convert the value into:

* Hours
* Remaining minutes
* Remaining seconds

Use `//` and `%`.

For example:

```text
Input: 7384

Output:
Hours: 2
Minutes: 3
Seconds: 4
```

---

## Submission Instructions

Submit your work in Google Classroom by:

1. Creating a **Google Doc**
2. Pasting your code into the document
3. Adding a screenshot of your output
4. Turning in the Google Doc to the appropriate assignment

---