---
title: "Lecture 7 — HTML Tables: Creating Structured Data"
weight: 7
---
# Lecture 7 — HTML Tables: Creating Structured Data
Instructor: **Laksh Budhrani**

---

## Quick Recall: Lectures 1–6 Review

Before we learn how to build structured tables, let's review all the tags and attributes we've mastered so far!

| Tag | Associated Attributes | Type | Purpose | Example |
| :--- | :--- | :--- | :--- | :--- |
| `<h1>` – `<h6>` | *None* | Paired | Headings of different sizes | `<h1>Heading</h1>` |
| `<p>` | *None* | Paired | Text paragraph block | `<p>Paragraph</p>` |
| `<b>`, `<i>`, `<u>` | *None* | Paired | Bold, Italics, Underline | `<b>Bold</b>`, `<i>Italic</i>`, `<u>Underline</u>` |
| `<mark>`, `<s>` | *None* | Paired | Highlight, Strikethrough | `<mark>Highlight</mark>`, `<s>Strike</s>` |
| `<sup>`, `<sub>` | *None* | Paired | Superscript, Subscript | `1<sup>st</sup>`, `H<sub>2</sub>O` |
| `<!-- -->` | *None* | Special | Hidden code notes/comments | `<!-- Note -->` |
| `<hr>`, `<br>` | *None* | Unpaired | Horizontal rule divider, Line break | `<hr>`, `<br>` |
| `<img>` | `src`, `alt`, `width`, `height` | Unpaired | Displays an image | `<img src="pic.jpg" alt="Pic" width="200">` |
| `<a>` | `href`, `target` (`_blank` / `_self`) | Paired | Creates clickable hyperlink | `<a href="https://..." target="_blank">Link</a>` |
| `<ul>` | *None* | Paired | Creates an unordered (bulleted) list | `<ul>...</ul>` |
| `<ol>` | *None* | Paired | Creates an ordered (numbered) list | `<ol>...</ol>` |
| `<li>` | *None* | Paired | Defines an individual item inside a `<ul>` or `<ol>` | `<li>Item</li>` |

> **Class Check-In:** Does anyone have questions about lists or previous project structures before we jump into HTML Tables?

---

## The Story Continues...

<img src="/images/sahil_table_planning.png" alt = "Sahil Planning His Table Image" width = "350">

> **Sahil's Week 7 Update!**
> 
> Sahil is loving his website! Now that his classes at UCI are in full swing, he wants to display his **Weekly Course Schedule** in a clean, organized format.
> 
> Lists work great for vertical stacks of information, but when Sahil wants to align data side-by-side in grid columns (like Course Name, Days, Time, and Location), lists get messy. Sahil needs our help using **HTML Tables** to build a single master class schedule inside a brand-new file: **`sahil_day7.html`**!

---

## Sahil's Request for Today

> *"Hey! I need to build a single structured grid layout so I can view my weekly classes and room numbers clearly!"*
>
> *"Here is what I need you to help me build in `sahil_day7.html`:"*
>
> 1. **Table Structure:** Set up one clean table container to hold my schedule.
> 2. **Header Row:** Create bold, distinct column titles (*Time*, *Course Name*, *Location*).
> 3. **Schedule Rows:** Add 4 rows of data matching my actual university timetable!

---

## Objectives

1. Understand the main table container: **`<table>`**
2. Build horizontal rows using **`<tr>`** (Table Row)
3. Create bold header titles using **`<th>`** (Table Header)
4. Fill in standard data cells using **`<td>`** (Table Data)

---

## How HTML Tables Work (Step-by-Step Theory)

Unlike standard text or lists, HTML tables are built **row by row** from top to bottom. Think of building a table like laying bricks for a house!

### The 4 Core Table Building Blocks

```
┌─────────────────────────────────────────────────────────────┐
│ <table>                          [Step 1: Outer Wall]       │
│   ┌───────────────────────────────────────────────────────┐ │
│   │ <tr>                         [Step 2: Start Row 1]    │ │
│   │ <th>Header 1</th>  <th>Header 2</th>  [Step 3: Titles]│ │
│   └───────────────────────────────────────────────────────┘ │
│   ┌───────────────────────────────────────────────────────┐ │
│   │ <tr>                         [Step 2: Start Row 2]    │ │
│   │ <td>Data 1</td>    <td>Data 2</td>    [Step 4: Values]│ │
│   └───────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────┘
```

---

### Step 1: Create the Main Wrapper (`<table>`)
Every table begins and ends with the `<table>` wrapper. It tells the browser that everything inside should be laid out in a grid.

```html
<table>
    <!-- ALL ROWS GO INSIDE HERE -->
</table>
```

---

### Step 2: Create a Horizontal Row (`<tr>`)
To add a line of information across your page, wrap it in a **`<tr>`** tag (**T**able **R**ow).

```html
<table>
    <tr>
        <!-- CELLS FOR THIS ROW GO HERE -->
    </tr>
</table>
```

---

### Step 3: Define Column Headings (`<th>`)
For the top row of your table, use **`<th>`** (**T**able **H**eader) for column titles.

* **Behavior:** Text inside `<th>` is automatically **BOLD** and **CENTERED**.

```html
<tr>
    <th>Fruit</th>
    <th>Color</th>
</tr>
```

---

### Step 4: Add Regular Data Cells (`<td>`)
For all remaining rows below the header, fill in your data using **`<td>`** (**T**able **D**ata).

* **Behavior:** Text inside `<td>` is regular, left-aligned text.

```html
<tr>
    <td>Apple</td>
    <td>Red</td>
</tr>
```

---

### Complete Basic Example

Here is what a complete 2x2 table looks like when put together:

```html
<table border = "1">
    <!-- Row 1: Headers -->
    <tr>
        <th>Fruit</th>
        <th>Color</th>
    </tr>
    <!-- Row 2: Data -->
    <tr>
        <td>Apple</td>
        <td>Red</td>
    </tr>
    <!-- Row 3: Data -->
    <tr>
        <td>Banana</td>
        <td>Yellow</td>
    </tr>
</table>
```

![Fruit Table Image](/images/fruit_table.png)

---

### Quick Comparison: `<th>` vs `<td>`

| Tag | Full Name | Default Style | Best Used For... |
| :--- | :--- | :--- | :--- |
| **`<th>`** | Table Header | **Bold** & Centered | Top row column names (e.g., *Fruit*, *Color*, *Price*) |
| **`<td>`** | Table Data | Normal & Left-Aligned | Standard data cells below the headers |

> **Golden Rule of Tables:** Never put text directly inside a `<tr>` or `<table>` tag! Text MUST always live inside either a `<th>` or `<td>` cell.

---

## Guided Activity — Building Sahil's Schedule Table

### PART 1 — Project Setup

1. Open **VS Code**.
2. Go to **File → Open Folder** and select your `Sahil_Project` folder.
3. Create a new file named: `sahil_day7.html`.

---

### PART 2 — Expected Browser Output

Here is what Sahil's completed schedule table will look like once we write the HTML together:

![Sahil Day 7 Browser Preview](/images/sahil_day7_preview.png)

---

### PART 3 — Starter Code (We will write the content together live!)

Paste this starter boilerplate into `sahil_day7.html`. We will fill in the `<body>` together in class!

```html
<!DOCTYPE html>
<html>

<head>
    <title>Sahil's Class Schedule</title>
</head>

<body>
    <!-- START WRITING HERE -->



    <!-- STOP WRITING HERE -->
</body>

</html>
```

---

## Independent Activity — My Personal Schedule Tracker!

Now it's your turn! Create a brand-new file for your portfolio to display your school schedule, sports rankings, or weekly routines using a single HTML table.

### Instructions:
1. Open your `Portfolio` folder in **VS Code**.
2. Create a new file named `portfolio_day7.html`.
3. Copy the starter template above into your file and build your page using `<table>`, `<tr>`, `<th>`, and `<td>`.

---

### Your Portfolio Prompt

Your page must include the following **4 requirements**:

1. **Table Setup:** Set up **1 main `<table>` container** with a descriptive `<h1>` title above it.
2. **Header Row (`<th>`):** Create at least **3 column headers** (e.g., *Period*, *Subject*, *Teacher* OR *Day*, *Activity*, *Time*).
3. **Data Rows (`<td>`):** Include at least **3 data rows** (`<tr>`) displaying your schedule or information.

---

### Example Solution
![Laksh's Portfolio Day 7 Image](/images/portfolio_day7.png)

---

## Submission Instructions

Submit your work in Google Classroom under **In‑Class Exercise 7** by:

1. Opening your **Google Doc** from previous lectures.
2. Pasting your HTML code from **both** `sahil_day7.html` and `portfolio_day7.html`.
3. Adding **screenshots** of both rendered pages from your browser.
4. Turning in the document!

---

## Summary: New Tags Learned Today

| Tag | Associated Attributes | Type | Purpose | Example |
| :--- | :--- | :--- | :--- | :--- |
| `<table>` | *None* | Paired | Main container wrapper for table content | `<table>...</table>` |
| `<tr>` | *None* | Paired | Defines a single horizontal row (Table Row) | `<tr>...</tr>` |
| `<th>` | *None* | Paired | Defines a bold, centered header cell (Table Header) | `<th>Header</th>` |
| `<td>` | *None* | Paired | Defines a standard data cell (Table Data) | `<td>Data</td>` |

---