---
title: Lecture 15 - Screen Wrapping & The Modulo Operator
weight: 15
Instructor: Laksh Budhrani
---

# Lecture 15 — Screen Wrapping & The Modulator Operator
Instructor: Laksh Budhrani

------------------------------------------------------------------------

## Objectives

1.  Understand how the modulo operator (`%`) works and calculates remainders.
2.  Use the modulo operator to create infinite screen-wrapping animations.

------------------------------------------------------------------------

## The Problem: Objects Disappearing Off-Screen

When an object moves across the screen (for example, from left to right), its position value keeps increasing forever. Once its X-coordinate exceeds the edge of the screen, the object disappears from view completely.

To make an animation loop continuously—so that when an object exits the right side, it reappears on the left side—we use a mathematical tool called the **modulo operator**.

------------------------------------------------------------------------

## How the Modulo Operator (`%`) Works

The modulo operator looks like a percent sign (`%`), but in programming, it has nothing to do with percentages. **It returns the remainder of a division problem.**

*   `10 % 3 = 1` (Because 3 goes into 10 three times with a remainder of 1)
*   `5 % 6 = 5` (Because 6 goes into 5 zero times with a remainder of 5)
*   `600 % 600 = 0` (Because 600 goes into 600 exactly once with a remainder of 0)

### Why Use It for Animation?

As our position variable increases frame by frame, passing it through a modulo operation with the screen width (e.g., `600`) restricts the number so it automatically resets back to `0` the exact moment it hits `600`.

```python
bug_position = (bug_position + 3) % 600
```
This ensures `bug_position` counts up from `0` to `599`, and the moment it hits `600`, it wraps back around to `0` instantly!

------------------------------------------------------------------------

## Knowledge Check --- Quick MCQs

Answer the following questions to test your understanding of the modulo operator:

**Question 1:** What is the result of `12 % 5`?

A) 2  
B) 5  
C) 7  
D) 60  

<br>

**Question 2:** If a screen width is `600` pixels and our position formula is `(position + 3) % 600`, what happens to the position value the moment it reaches `600`?

A) It stays at 600 forever  
B) It resets back to 0  
C) It crashes the program  
D) It starts counting backwards  

------------------------------------------------------------------------

## Guided Activity --- Wrapping Ladybug

We will write the looping ladybug animation code together in class.

Create a new Python file named `animation_bug.py`.

### Ladybug Animation Video

<video width="100%" controls preload="metadata">
  <source src="/videos/bug_animation.mp4#t=0.001" type="video/mp4">
  Your browser does not support the video tag.
</video>

### Starter Template

Copy this template into `animation_bug.py`. We will fill in the code together.

```python
from animation import run_sketch

def draw(p):
    pass
    # Write the car drawing code here


    # Update the car's position here


run_sketch(draw, bgcolor="lightblue")
```

------------------------------------------------------------------------

## Independent Activity --- Swimming Fish

Create a new Python file named `animation_fish.py`.

### Fish Animation Video

<video width="100%" controls preload="metadata">
  <source src="/videos/fish_animation.mp4#t=0.001" type="video/mp4">
  Your browser does not support the video tag.
</video>

### Your Task

Create a swimming fish that moves across the screen from left to right and wraps around infinitely using the modulo operator.

Your animation should:

-   Draw a fish structure including a body, tail fins, and an eye.
-   Use a position variable starting at `0`.
-   Apply the modulo operator (`% 600`) so that when the fish swims off the right side of the screen, it loops back to the left side seamlessly.

Use the ladybug animation as a guide, but write the fish code yourself.

### Submission Instructions

Submit your work in Google Classroom by:

1.  Creating a Google Doc.
2.  Pasting your code into the document.
3.  Adding a screenshot of the animation window.
4.  Turning in the Google Doc to the assigned activity.

------------------------------------------------------------------------