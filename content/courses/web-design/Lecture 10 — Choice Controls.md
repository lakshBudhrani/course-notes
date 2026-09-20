---
title: "Lecture 10 — Choice Controls: Radio Buttons & Checkboxes"
weight: 10
---
# Lecture 10 — Choice Controls: Radio Buttons & Checkboxes  
Instructor: **Laksh Budhrani**

---

## Quick Recall: Lecture 9 Summary

Last class, we learned how to collect information from website visitors by building interactive HTML forms! Here is a review of all the new tags and attributes we mastered:

| Tag / Attribute       | Type            | Purpose                                                  | Example                   |
| :-------------------- | :-------------- | :------------------------------------------------------- | :------------------------ |
| **`<form>`**          | Paired Tag      | Main wrapper container for all form controls             | `<form>...</form>`        |
| **`<label>`**         | Paired Tag      | Displays text labeling a specific input field            | `<label>Name:</label>`    |
| **`<input>`**         | Unpaired Tag    | Creates an interactive input field                       | `<input type="text">`     |
| **`type="text"`**     | Attribute Value | Creates a standard single-line text box                  | `<input type="text">`     |
| **`type="email"`**    | Attribute Value | Creates an input box tuned for email addresses           | `<input type="email">`    |
| **`type="password"`** | Attribute Value | Creates a masked text box that hides typed characters    | `<input type="password">` |
| **`name="..."`**      | Attribute       | Column header/label for saving field data in the backend | `name="user_name"`        |
| **`value="..."`**     | Attribute       | Text stored or pre-filled inside the input box           | `value="Peter"`           |

> **Class Check-In:** Why give choices instead of text boxes? Choice controls make forms faster to fill out and prevent spelling errors!

---

## The Story Continues...

<img src="/images/sahil_choice_controls.jpg" alt="Sahil Choice Controls Image" width="350">

> **Sahil's Week 10 Update!**
> 
> Sahil's contact form is looking great, but now he wants to organize his study group sign-ups! 
> 
> He needs to ask his classmates two specific questions on his page **`sahil_day10.html`**:
> 1. **"What is your current class standing?"** (Freshman, Sophomore, Junior, or Senior — *Must pick exactly ONE*)
> 2. **"Which subjects do you want to study together?"** (Web Design, Python, Math, Physics — *Can pick MULTIPLE*)
> 
> Let's help Sahil build these choice options using Radio Buttons and Checkboxes!

---

## Sahil's Request for Today

> *"Hey! I want to make my study group form super easy to fill out with quick clickable options!"*
>
> *"Here is what I need you to help me build in `sahil_day10.html`:"*
>
> 1. **Single-Choice Group (Radio Buttons):** A question where classmates select their grade level. Selecting one should uncheck any other!
> 2. **Multi-Choice Group (Checkboxes):** A question where classmates can check off all subjects they want to study.
> 3. **Proper Grouping (`name` attribute):** Group radio buttons together correctly so only one can be picked at a time!

---

## Objectives

1. Master single-choice selection using **`<input type="radio">`**.
2. Group radio buttons using matching **`name`** attributes.
3. Master multi-choice selection using **`<input type="checkbox">`**.
4. Use pre-defined **`value`** attributes so the computer knows which option was clicked.

---

## Objective 1 & 2 — Radio Buttons (`type="radio"`)

Radio buttons are used when a user must choose **exactly one** option out of a list.

### Grouping with `name`
To make radio buttons work as a team, **all radio buttons in the same question MUST share the exact same `name` attribute**!

```html
<label>Grade Level:</label><br>

<input type="radio" name="grade" value="freshman">
<label>Freshman</label><br>

<input type="radio" name="grade" value="sophomore">
<label>Sophomore</label>
```

![Step 1 Radio Example](/images/step1_radio_example.png)

> **Important Rule:** If radio buttons have different `name` attributes, the browser will let you select all of them at once!

---

## Objective 3 — Checkboxes (`type="checkbox"`)

Checkboxes are used when a user can select **zero, one, or multiple** options. Checking one box does **NOT** uncheck the others!

![Step 2 Checkbox Example](/images/step2_checkbox_example.png)

```html
<label>Interests:</label><br>

<input type="checkbox" name="interest" value="coding">
<label>Coding</label><br>

<input type="checkbox" name="interest" value="gaming">
<label>Gaming</label>
```

---

## Objective 4 — Why `value` is Mandatory for Choice Controls!

When users type into a text box, the computer saves whatever text they typed. 

With radio buttons and checkboxes, **users don't type anything**—they just click a button!

Because of this, **you must write `value="..."` in your HTML** so the computer knows what text to save when an option is clicked.

```html
<input type="radio" name="grade" value="Freshman">
```

| `grade` *(from name)*                     |
| :---------------------------------------- |
| **Freshman** *(value saved when clicked)* |

---

## Guided Activity — Building Sahil’s Choice Form

### PART 1 — Project Setup

1. Open **VS Code**.
2. Go to **File → Open Folder** and select your `Sahil_Project` folder.
3. Create a new file named: `sahil_day10.html`.

---

### PART 2 — Expected Browser Output

Here is what Sahil's completed choice form will look like once we write the HTML together:

![Sahil Day 10 Browser Preview](/images/sahil_day10_preview.png)

---

### PART 3 — Starter Code (We will write the content together live!)

Paste this starter boilerplate into `sahil_day10.html`. We will fill in the `<body>` together in class!

```html
<!DOCTYPE html>
<html>

<head>
    <title>Sahil's Study Preferences</title>
</head>

<body>
	<!-- START WRITING HERE -->



	<!-- STOP WRITING HERE -->
</body>

</html>
```

---

## Independent Activity — Portfolio Survey Page!

Now it's your turn! Add a quick feedback or survey section to your portfolio site using choice controls.

### Instructions:
1. Open your `Portfolio` folder in **VS Code**.
2. Create a new file named `portfolio_day10.html`.
3. Copy the starter template above into your file and build your page using `<form>`, radio buttons, and checkboxes.

---

### Your Portfolio Prompt

Your page must include the following **4 requirements**:

1. **Form Setup:** Set up **1 main `<form>` container** with a descriptive `<h1>` title above it.
2. **Text Field:** Include at least **1 text input** (Name or Email).
3. **Radio Button Group (Pick 1):** Create a group of at least **3 radio buttons** with matching `name` attributes and clear `value` attributes.
4. **Checkbox Group (Pick Multiple):** Create a group of at least **3 checkboxes** with clear `value` attributes.

---

### Example Solution
![Portfolio Day 10 Example Image](/images/portfolio_day10.png)

---

## Submission Instructions

Submit your work in Google Classroom under **In‑Class Exercise 10** by:

1. Opening your **Google Doc** from previous lectures.
2. Pasting your HTML code from **both** `sahil_day10.html` and `portfolio_day10.html`.
3. Adding **screenshots** of both rendered pages from your browser.
4. Turning in the document!

---

## Summary: New Tags & Attributes Learned Today

| Control / Attribute | Type | Purpose | Code Example |
| :--- | :--- | :--- | :--- |
| `type="radio"` | Attribute Value | Single-choice round button | `<input type="radio">` |
| `type="checkbox"` | Attribute Value | Multi-choice square box | `<input type="checkbox">` |
| `name="..."` | Attribute | Groups radio buttons together & labels column | `name="grade"` |
| `value="..."` | Attribute | Sets the specific data text saved when clicked | `value="freshman"` |

---