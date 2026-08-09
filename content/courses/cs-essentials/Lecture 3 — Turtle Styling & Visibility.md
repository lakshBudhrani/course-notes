---
title: "Lecture 3 — Turtle Styling & Visibility"
weight: 3
---
# Lecture 3 — Turtle Styling & Visibility  
Instructor: Laksh Budhrani

---

## Review / Recap

### Basic Commands from Previous Lectures

| Command             | Meaning (Simple)                      |
| ------------------- | ------------------------------------- |
| `p.forward(steps)`  | Move the turtle **straight ahead**    |
| `p.backward(steps)` | Move the turtle **straight backward** |
| `p.left(angle)`     | Turn the turtle **left**              |
| `p.right(angle)`    | Turn the turtle **right**             |
| `p.penup()`         | Move **without drawing**              |
| `p.pendown()`       | Start **drawing again**               |

---

## Objectives

1. Learn how to change pen color using `pencolor()`  
2. Learn how to change line thickness using `pensize()`  
3. Learn how to hide the turtle using `hideturtle()`  
4. Learn how to show the turtle using `showturtle()`  

---

## Objective 1 — `pencolor()`

### Simple Definition
- **`pencolor()`** — Change the **color** of the turtle’s pen.

---

### Example: Change Pen Color

```python
p.pencolor("red")
p.forward(100)
```

![Turtle Pen Color](/images/turtle_pencolor.png)

---

## Objective 2 — `pensize()`

### Simple Definition
- **`pensize()`** — Change the **thickness** of the line.

---

### Example: Change Pen Size

```python
p.pensize(10)
p.forward(100)
```

![Turtle Pen Size](/images/turtle_pensize.png)

---

## Objective 3 — `hideturtle()`

### Simple Definition
- **`hideturtle()`** — Hide the turtle icon from the screen.

---

### Example: Hide Turtle

```python
p.hideturtle()
p.forward(100)
```

![Turtle Hidden](/images/turtle_hidden.png)

---

## Objective 4 — `showturtle()`

### Simple Definition
- **`showturtle()`** — Show the turtle icon again.

---

### Example: Show Turtle

```python
p.showturtle()
p.forward(100)
```

![Turtle Shown](/images/turtle_shown.png)

---

## CS Drawing Activity (Guided)

Create a new Python file in VS Code named:  
`turtle_class3.py`

### CS Image
![Turtle CS](/images/turtle_cs.png)

---

### Explain in Plain English
Write a short explanation (3–5 sentences) describing **how you think we can draw the letters “C” and “S”** using:

- `forward()`
- `left()`
- `right()`
- `penup()`
- `pendown()`
- `pencolor()`
- `pensize()`
- `hideturtle()`

Explain the steps in **simple English**, as if you are telling a friend how to draw it.

---

### Boilerplate Code

```python
import turtle as trtl

p = trtl.Turtle()
p.speed(0)

# --- ENTER YOUR CODE HERE ---
# (Write your CS drawing steps using the new styling commands)



# --------------------------------------------------------------
# (Stop writing code above this line)

wn = trtl.Screen()
wn.mainloop()
```

---

### Notes
- Use **different colors** for the C and S.  
- Use **pensize(30)** to make the letters bold.  
- Use `penup()` to move without drawing.  
- Use `pendown()` to start drawing again.  
- Use `hideturtle()` at the end for a clean final look.  

---

## Independent Activity — Color Stairs Drawing

### Stairs Image
![Color Stairs](/images/turtle_stairs.png)

---

### Your Task
Look at the image above and **draw it independently** using:

- `forward(distance)`
- `left(angle)`
- `right(angle)`
- `pencolor()`
- `pensize()`
- `hideturtle()`

Use the **Turtle boilerplate code** provided earlier in this lecture.

---

### Create Your Own File
Create a new Python file in VS Code named:

`turtle_class3_independent.py`

Inside that file, use the boilerplate and write your stairs‑drawing code in the section marked:

`# --- ENTER YOUR CODE HERE ---`

---

### Submission Instructions
Submit your work in Google Classroom by:

1. Creating a **Google Doc**  
2. Pasting your **code** into the document  
3. Adding a **screenshot** of the output window showing your drawing  
4. Turn in the Google Doc to the assignment titled **In‑Class Exercise 3**

---
