# Lecture 5 — Turtle Circles, Arcs & Polygons  
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

---

## Objectives

1. Learn how to draw circles  
2. Learn how to draw arcs  
3. Learn how to draw polygon‑style circles  

---

## Objective 1 — Full Circle: `circle(r)`

### Simple Definition
- **`circle(r)`** — Draw a full circle with radius **r**.

### Example

```python
p.circle(80)
```

![Turtle Circle](/images/turtle_circle.png)

---

## Objective 2 — Arc: `circle(r, a)`

### Simple Definition
- **`circle(r, a)`** — Draw an **arc** of angle **a** degrees.

### Example

```python
p.circle(100, 180)  
```

![Turtle Arc](/images/turtle_arc.png)

---

## Objective 3 — Polygon Circle: `circle(r, a, s)`

### Simple Definition
- **`circle(r, a, s)`** — Draw a circle or arc using **s straight-line steps**, creating a polygon.

### Example

```python
p.circle(60, 360, 6)  
```

![Turtle Polygon](/images/turtle_polygon.png)

---

## Quick MCQ Check — Circle Syntax & Logic

### **1. What does `p.circle(50)` draw?**
A. A square  
B. A full circle of radius 50  
C. A half circle  
D. A polygon  

---

### **2. What does `p.circle(80, 90)` draw?**
A. A full circle  
B. A 90‑degree arc  
C. A polygon  
D. A straight line  

---

### **3. What does the third parameter in `circle(r, a, s)` control?**
A. Color  
B. Speed  
C. Number of straight‑line steps  
D. Radius  

---

### **4. Which command draws a triangle using circle syntax?**
A. `p.circle(50, 360, 3)`  
B. `p.circle(50)`  
C. `p.circle(50, 180)`  
D. `p.circle(50, 360, 10)`  

---

### **5. What does `p.circle(30, 180)` draw?**
A. A full circle  
B. A 180‑degree arc  
C. A square  
D. A hexagon  

---

### **6. Which one draws a polygon with 8 sides?**
A. `p.circle(60, 360, 8)`  
B. `p.circle(60, 180, 8)`  
C. `p.circle(60)`  
D. `p.circle(60, 360)`  

---

### **7. What happens if you write `p.circle(100, 360, 4)`?**
A. A perfect circle  
B. A square  
C. A triangle  
D. A straight line  

---

### **8. Which command draws a quarter circle?**
A. `p.circle(80, 360)`  
B. `p.circle(80, 90)`  
C. `p.circle(80, 180)`  
D. `p.circle(80, 45, 4)`  

---

## Car Drawing Activity (Guided)

Create a new Python file in VS Code named:  
`turtle_class5.py`

### Car Image
![Turtle Car](/images/turtle_car.png)

---

### Explain in Plain English
Write a short explanation (3–5 sentences) describing **how you think we can draw this car** using:

- `circle()`  
- `circle(r, a)`  
- `circle(r, a, s)`  
- `pencolor()`  
- `pensize()`  
- `goto()`  
- `setheading()`  
- `penup()`  
- `pendown()`  
- `hideturtle()`

Explain the steps in **simple English**, as if you are telling a friend how to draw it.

---

### Boilerplate Code

```python
import turtle as trtl

p = trtl.Turtle()
p.speed(0)

# --- ENTER YOUR CODE HERE ---
# (Use circles, arcs, and polygon circles to draw the car)



# --------------------------------------------------------------
# (Stop writing code above this line)

wn = trtl.Screen()
wn.mainloop()
```

---

### Notes
- Use polygon circles for the car body.  
- Use full circles for wheels.  
- Use arcs for the headlight.  
- Use `goto()` to place each part correctly.  
- Use `hideturtle()` at the end for a clean final look.  

---

## Independent Activity — Smiley Face Drawing

### Smiley Face Image
<img src="/course-notes/images/turtle_smiley.png" width="240">

---

### Your Task
Look at the image above and **draw it independently** using:

- `circle(r)`  
- `circle(r, a)`  
- `pencolor()`  
- `pensize()`  
- `goto(x, y)`  
- `penup()`  
- `pendown()`  
- `hideturtle()`

Use the **Turtle boilerplate code** provided earlier in this lecture.

---

### Create Your Own File
Create a new Python file in VS Code named:

`turtle_class5_independent.py`

Inside that file, use the boilerplate and write your smiley‑face code in the section marked:

`# --- ENTER YOUR CODE HERE ---`

---

### Submission Instructions
Submit your work in Google Classroom by:

1. Creating a **Google Doc**  
2. Pasting your **code** into the document  
3. Adding a **screenshot** of the output window showing your drawing  
4. Turn in the Google Doc to the assignment titled **In‑Class Exercise 5**

---
