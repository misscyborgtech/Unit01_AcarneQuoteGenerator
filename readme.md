# Project 1: Random Quote Generator – Arcane Edition

## 🧾 Overview

This project displays randomized quotes from the _Arcane_ universe with additional metadata, styled character images, and background color gradients that match the character’s personality.  
It was created as part of the Treehouse Full Stack JavaScript Techdegree and demonstrates array manipulation, conditional rendering, DOM interaction, and timed updates using vanilla JavaScript.

---

## 📦 Base Project Features (Required)

### ✅ Random Quote Generator

- A random quote displays each time the "Show another quote" button is clicked.
- Each quote object includes a **quote**, **source**, and optionally a **citation** and **year**.
- Quotes are stored in an array of objects and retrieved using `getRandomQuote()`.

### 🔧 Key Functions

#### `getRandomQuote()`

- Returns a random quote object from the `quotes` array.
- Uses `Math.floor()` and `Math.random()` to calculate a valid index.

#### `printQuote()`

- Builds and injects HTML with quote details into the DOM.
- Handles conditional display of optional properties like citation and year.

---

## 🌟 Extra Credit Features

> These enhancements go beyond the core functionality and aim for an "Exceeds Expectations" rating.

### 🎨 Character-Based Backgrounds

- Each character’s quote triggers a **unique background gradient** that matches their aesthetic.
- Implemented using a `colorQuote()` function and a lookup object keyed by `source`.

### 🧠 Additional Properties in Quote Objects

- Quote objects optionally include:
  - `voice`: The actor who voices the character
  - `episodes`: Number of episodes the character appears in
  - `image`: A portrait displayed next to the quote
- These are dynamically injected when present.

### ⏱ Auto-Refreshing Quotes

- Quotes update **automatically every 15 seconds** using `setInterval()`.
- Ensures a fresh experience without user interaction.

---

## 🧠 Lessons Learned

- How to organize and manipulate arrays of objects in JavaScript
- Using DOM methods like `getElementById()` and `.innerHTML` for dynamic content
- Writing conditional logic to selectively add HTML elements
- Leveraging `setInterval()` to automate updates
- How to keep CSS and JavaScript separated while achieving rich UI effects

---

## 📁 Files Structure

- `index.html` – Static page structure
- `css/styles.css` – Styling for layout and characters
- `js/script.js` – Quote logic, DOM manipulation, and interactivity
- `img/` – Character images for enhanced visual context

---

## 🌐 Deployment

https://misscyborgtech.github.io/Unit01_AcarneQuotesGenerator/

## 🚀 Next Steps

- Add validation to avoid generating the same quote twice
- Add an ui element for the setInterval
- Add validation that the setInterval restarts its timer when the user presses the
