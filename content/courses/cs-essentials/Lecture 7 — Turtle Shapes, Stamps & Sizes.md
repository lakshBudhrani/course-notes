---
title: "Lecture 7 — Turtle Shapes, Stamps & Sizes"
weight: 7
---
# Lecture 7 — Turtle Shapes, Stamps & Sizes  
Instructor: Laksh Budhrani

---

## Review / Recap

### Commands You Already Know

| Command               | Meaning (Simple)                         |
| --------------------- | ---------------------------------------- |
| `p.forward(steps)`    | Move the turtle **straight ahead**       |
| `p.backward(steps)`   | Move the turtle **straight backward**    |
| `p.left(angle)`       | Turn the turtle **left**                 |
| `p.right(angle)`      | Turn the turtle **right**                |
| `p.penup()`           | Move **without drawing**                 |
| `p.pendown()`         | Start **drawing again**                  |
| `p.pencolor(color)`   | Change the **pen color**                 |
| `p.pensize(size)`     | Change the **line thickness**            |
| `p.hideturtle()`      | Hide the turtle icon                     |
| `p.showturtle()`      | Show the turtle icon again               |
| `p.goto(x, y)`        | Teleport the turtle to a coordinate      |
| `p.setheading(angle)` | Point the turtle in a specific direction |
| `p.circle(r)`         | Draw a **full circle**                   |
| `p.circle(r, a)`      | Draw an **arc**                          |
| `p.circle(r, a, s)`   | Draw a **polygon circle**                |
| `p.begin_fill()`      | Start filling a shape                    |
| `p.end_fill()`        | Finish filling a shape                   |
| `p.fillcolor()`       | Set fill color                           |

---

## Objectives 

1. Learn how to change turtle **shape**  
2. Learn how to **stamp** turtle shapes  
3. Learn how to change turtle **size** using `turtlesize()`  
4. Learn how to change turtle **speed**  
5. Learn how to draw dots using `dot()`  

---

## Objective 1 — `shape()`

### Simple Definition
- **`shape()`** — Change the turtle’s appearance.

### Available Shapes
- `"arrow"`  
- `"turtle"`  
- `"circle"`  
- `"square"`  
- `"triangle"`  
- `"classic"`

### Example

```python
p.shape("turtle")
p.forward(100)
```

![Turtle Shape](/images/turtle_shape.png)

---

## Objective 2 — `stamp()`

### Simple Definition
- **`stamp()`** — Leave a **copy** of the turtle shape on the screen.

### Example

```python
p.shape("arrow")
p.stamp()
p.forward(30)
p.shape("turtle")
p.stamp()
p.forward(30)
p.shape("circle")
p.stamp()
```

![Turtle Stamp](/images/turtle_stamp.png)

---

## Objective 3 — `turtlesize()`

### Simple Definition
- **`turtlesize()`** — Make the turtle icon **bigger or smaller**.

### Example

```python
p.shape("circle")
p.turtlesize(1)
p.stamp()
p.forward(70)
p.turtlesize(2)
p.stamp()
p.forward(70)
p.turtlesize(3)
p.stamp()
```

![Turtle Size](/images/turtle_size.png)

---

## Objective 4 — `speed()`

### Simple Definition
- **`speed()`** — Change how fast the turtle moves.

### Speed Levels (Short & Simple)
- `speed(0)` → **fastest** (no animation)  
- `speed(1)` → **slowest**  
- `speed(3)` → **slow**  
- `speed(6)` → **normal**  
- `speed(10)` → **fast**

### Example

```python
p.speed(0)   # fastest drawing
```

---

## Objective 5 — `dot()`

### Simple Definition
- **`dot(size, color)`** — Draw a filled circle (dot).

### Example

```python
p.dot(30, "red")
p.forward(40)
p.dot(15, "purple")
p.forward(40)
p.dot(25, "green")
```

![Turtle Dot](/images/turtle_dot.png)

---

## Solar System Activity (Guided)

Create a new Python file in VS Code named:  
`turtle_class7.py`

### Solar System Image
![Solar System](/images/turtle_solar.png)

---

### Explain in Plain English
Write a short explanation (3–5 sentences) describing **how you think we can draw this solar system** using:

- `shape()`  
- `turtlesize()`  
- `stamp()`  
- `speed()`  
- `dot()`  
- `pencolor()`  
- `fillcolor()`  
- `goto()`  
- `penup()`  
- `pendown()`  

Explain the steps in **simple English**, as if you are telling a friend how to draw it.

---

### Boilerplate Code

```python
import turtle as trtl

p = trtl.Turtle()
p.speed(0)

# --- ENTER YOUR CODE HERE ---
# (Use shape, turtlesize, stamp, speed, and dot to draw the solar system)



# --------------------------------------------------------------
# (Stop writing code above this line)

wn = trtl.Screen()
wn.mainloop()
```

---

### Notes
- Use `shape("triangle")` and `stamp()` for stars  
- Use `dot()` for planets  
- Use `turtlesize()` to make stars bigger  
- Use `goto()` to place each planet  
- Use `bgcolor()` to make space look nice  
- Use `hideturtle()` at the end for a clean final look  

---

## Independent Activity — Ladybug Drawing

### Ladybug Image
![Ladybug](/images/turtle_ladybug.png)

---

### Your Task
Look at the image above and **draw it independently** using:

- `shape()`  
- `turtlesize()`  
- `stamp()`  
- `dot()`  
- `fillcolor()`  
- `pencolor()`  
- `goto(x, y)`  
- `penup()`  
- `pendown()`  
- `hideturtle()`

Use the **Turtle boilerplate code** provided earlier in this lecture.

---

### Create Your Own File
Create a new Python file in VS Code named:

`turtle_class7_independent.py`

Inside that file, use the boilerplate and write your ladybug code in the section marked:

`# --- ENTER YOUR CODE HERE ---`

---

### Submission Instructions
Submit your work in Google Classroom by:

1. Creating a **Google Doc**  
2. Pasting your **code** into the document  
3. Adding a **screenshot** of the output window showing your drawing  
4. Turn in the Google Doc to the assignment titled **In‑Class Exercise 7**

---
