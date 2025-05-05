# 🌀 Arcane Quotes Generator

This project is a random quote generator inspired by the **Arcane** series. It dynamically selects and displays a quote in the browser, with a custom visual style tailored to each character.

## 🚀 Features

- Randomly displays quotes from the **Arcane** universe
- Uses an array of objects containing metadata like source, year, voice actor, and number of episodes
- Automatically refreshes with a new quote every 15 seconds
- Background changes based on the quoted character
- Button available to manually generate a new quote

## 🧠 Project Structure

### 1. `quotes[]`

An array of quote objects, each including:

- `quote`: the quote text
- `source`: the character who said it
- `citation`: the season or work it comes from (optional)
- `year`: the year it originated (optional)
- `voice`: the voice actor (optional)
- `episodes`: total number of episodes the character appears in (optional)

### 2. `getRandomQuote()`

Returns a random quote object from the `quotes` array.

### 3. `printQuote()`

- Calls `getRandomQuote()`
- Dynamically builds an HTML string with the quote's details
- Injects the content into the `<div id="quote-box">`
- Also calls `colorQuote()` to change the background based on the character

### 4. `colorQuote()`

Instead of generating a random color, I took the liberty of assigning a **custom gradient to each character**. This visually reinforces the unique personality of each Arcane figure.

### 5. Auto-refresh

A `setInterval()` function calls `printQuote()` every **15 seconds** to keep the interface dynamic and fresh.

---

## 🌐 Deployment

https://misscyborgtech.github.io/Unit01_AcarneQuotesGenerator/

## 🚀 Next Steps

- Add validation to avoid generating the same quote twice
- Add an ui element for the setInterval
- Add validation that the setInterval restarts its timer when the user presses the

---

💬 **Feedback or suggestions?** Feel free to reach out via GitHub!  
Thanks for stopping by 🖖
