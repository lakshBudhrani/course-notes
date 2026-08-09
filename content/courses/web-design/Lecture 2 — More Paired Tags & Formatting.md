# Lecture 2 — More Paired Tags & Formatting
Instructor: **Laksh Budhrani**

---

## Quick Recall: Lecture 1 Review

Before we jump into today's mission, let's do a quick check-in on what we learned last class:

| Tag             | Name      | What It Does                        | Example                |
| :-------------- | :-------- | :---------------------------------- | :--------------------- |
| `<h1>` – `<h6>` | Heading   | Creates headings of different sizes | `<h1>Heading</h1>`     |
| `<p>`           | Paragraph | Groups text into structured blocks  | `<p>Text here...</p>`  |
| `<b>`           | Bold      | Emphasizes text in **bold**         | `<b>Important</b>`     |
| `<i>`           | Italics   | Slants text in *italics*            | `<i>Stylized note</i>` |

> **Class Check-In:** Does anyone have any questions or doubts about these 4 tags before we add 5 new ones to our toolkit?

---

## The Story Continues...

<img src="/course-notes/images/sahil_studying.png" alt = "Sahil Studying Image" width = "350">

> **Sahil's Week 2 Update!**
> 
> Sahil has survived his first full week of college classes at UC Irvine! Between joining the campus swimming club, finding coffee spots, and studying for midterms, he is trying to keep his college life organized.
> 
> He wants to add a **"Notebook & Goals"** section to his website to track his progress and stats. He needs your help writing this page using 5 new text-formatting tags!

---

## Sahil's Request for Today

> *"Hey again! Thanks for helping me set up my main homepage. Today, I want to build a digital notebook page to track my goals, stats, and checklist."*
>
> *"Here is what I need you to write for me:"*
>
> 1. **Academic Goals Paragraph:** Write a sentence about my goal to focus on classes and become a CS Researcher. I want to underline **UC Irvine** to emphasize my campus pride.
> 2. **Current Status & Stats:** 
>    * Highlight **Surviving Midterms** so anyone visiting sees my current focus instantly.
>    * Write my graduation year as **Class of '29<sup>th</sup>** (with the *th* raised up).
>    * Mention my water intake after swimming practice as **H<sub>2</sub>O** (with the *2* lowered down).
> 3. **College Checklist:** Create a list of 3 dorm tasks, and cross off the ones I've already completed (like moving into my dorm) using a line through the text.

---

## Objectives

1. Learn how to underline key text (`<u>`)
2. Learn how to highlight text (`<mark>`)
3. Learn how to format superscript (`<sup>`) and subscript (`<sub>`)
4. Learn how to cross off text using strikethrough (`<s>`)

---

## Objective 1 — Underline (`<u>`)

#### Simple Definition
The `<u>` tag draws a horizontal line under text to emphasize key terms, titles, or locations.

#### Example
```html
<u>Important Location</u>
```

![Underline Example Screenshot](/images/underline_example.png)

---

## Objective 2 — Highlight (`<mark>`)

#### Simple Definition
The `<mark>` tag adds a bright yellow background behind text, making it stand out like a physical highlighter pen.

#### Example
```html
<mark>High Priority Task</mark>
```

![Highlight Example Screenshot](/images/highlight_example.png)

---

## Objective 3 — Superscript (`<sup>`) & Subscript (`<sub>`)

#### Simple Definition
* `<sup>` (Superscript) raises text slightly **above** the normal line of text.
* `<sub>` (Subscript) lowers text slightly **below** the normal line of text.

#### Example
```html
1<sup>st</sup> Place
Water molecule: H<sub>2</sub>O
```

![Superscript and Subscript Example Screenshot](/images/supsub_example.png)

---

## Objective 4 — Strikethrough (`<s>`)

#### Simple Definition
The `<s>` tag draws a line straight through text. It is commonly used to show things that are no longer accurate or tasks that have been completed.

#### Example
```html
<s>Completed Task</s>
```

![Strikethrough Example Screenshot](/images/strikethrough_example.png)

---

## Guided Activity — Build Sahil’s Notebook Page

### PART 1 — Project Setup

1. Open **VS Code**.
2. Go to **File → Open Folder** and select your `Sahil_Project` folder.
3. Create a new file named: `sahil_day2.html`.

---

### PART 2 — Expected Browser Output

Here is what Sahil's completed notebook page will look like once we write the HTML together:

![Sahil Day 2 Browser Preview](/images/sahil_day2_preview.png)

---

### PART 3 — Starter Code (We will write the content together live!)

Paste this starter boilerplate into `sahil_day2.html`. We will fill in the `<body>` together in class!

```html
<!DOCTYPE html>
<html>

<head>
    <title>Sahil's Notebook & Goals</title>
</head>

<body>
	<!-- START WRITING HERE -->



	<!-- STOP WRITING HERE -->
</body>

</html>
```

---

## Independent Activity — Your Portfolio Goals!

Now it's your turn! Upgrade your own portfolio site by creating a personal stats and goals page.

### Instructions:
1. Open your `Portfolio` folder in **VS Code**.
2. Create a new file named `portfolio_day2.html`.
3. Copy the starter template above into your file and build your page using `<h1>`, `<h2>`, and your **5 new paired tags**.

---

### Your Portfolio Prompt

Your page must include the following **4 sections**:

1. **Main Title (`<h1>`):** `[Your Name]'s Status & Goals`
2. **School Focus (`<h2>` & `<u>`):** A short paragraph mentioning your school name or grade level, underlined with `<u>`.
3. **Current Vibe & Stats (`<h2>`, `<mark>`, `<sup>`, `<sub>`):** 
   * A highlighted current status using `<mark>` (e.g., `<mark>Learning HTML</mark>`).
   * A date or rank using `<sup>` (e.g., `1<sup>st</sup> day of class` or `10<sup>th</sup> Grade`).
   * A small detail using `<sub>` (e.g., `Favorite drink: H<sub>2</sub>O` or `Base<sub>10</sub> math`).
4. **My Checklist (`<h2>` & `<s>`):** A list of 3 personal goals or tasks for this week, with at least 1 task crossed off using `<s>`.

---

### Example Solution
![Laksh's Portfolio Day 2 Image](/images/portfolio_day2.png)

---

## Submission Instructions

Submit your work in Google Classroom under **In‑Class Exercise 2** by:

1. Opening your **Google Doc** from Lecture 1.
2. Pasting your HTML code from **both** `sahil_day2.html` and `portfolio_day2.html`.
3. Adding **screenshots** of both rendered pages from your browser.
4. Turning in the document!

---

## Summary: New Tags Learned Today

| Tag | Name | What It Does | Example |
| :--- | :--- | :--- | :--- |
| `<u>` | Underline | Underlines text | `<u>Underlined</u>` |
| `<mark>` | Highlight | Adds yellow highlight behind text | `<mark>Highlighted</mark>` |
| `<sup>` | Superscript | Raises text above line | `1<sup>st</sup>` |
| `<sub>` | Subscript | Lowers text below line | `H<sub>2</sub>O` |
| `<s>` | Strikethrough | Crosses out text with a line | `<s>Completed</s>` |

---
