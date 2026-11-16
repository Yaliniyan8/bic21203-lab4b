# BIC21203 Web Development — Lab #4b: Client-Side Scripting (JSON and jQuery)

- **Name:** YALINIYAN A/L BHUVANESWARAN
- **Student ID:** CI250114

## Overview
This repository contains the client-side scripting solutions for Lab #4b, demonstrating how to structure a valid JSON dataset (`books.json`), retrieve and display JSON data safely using the native JavaScript `fetch()` API (`books.html`), and perform DOM manipulation and event handling using jQuery 4.0.0 (`jquery-dom.html`).

## Setup Instructions
1. Clone or download this repository and open the project folder in **VS Code** (ensure the folder name contains no `#` symbol).
2. Install the **Live Server** extension in VS Code and use a modern desktop browser.
3. Start a local development server by right-clicking the HTML file and selecting **Open with Live Server**.
   > **Important:** Do **not** open `books.html` directly using `file://`, as browsers block `fetch()` requests to local JSON files without a local server.

## How to Run & Expected Results

### Question 1 — Create and Structure JSON Data (`books.json`)
- **Setup:** Open `books.json` in VS Code or run `fetch("books.json").then(r => r.json()).then(console.log)` in the browser console while Live Server is running.
- **Expected Result:** A valid JSON object containing a top-level `"books"` array with two book objects (*The Great Gatsby* and *To Kill a Mockingbird*) parses cleanly with zero syntax errors.

### Question 2 — Retrieve and Display JSON Data (`books.html`)
- **Action:** Open `books.html` through **VS Code Live Server**.
- **Initial Page State & Expected Result:** On page load, the script fetches `books.json` and automatically displays:
  - **First Book Title:** `The Great Gatsby`
  - **Second Book Author:** `Harper Lee`
  - **Genres by Book:**
    - `The Great Gatsby — Fiction, Classics`
    - `To Kill a Mockingbird — Fiction, Coming-of-Age`
  *(If `books.json` is missing or invalid, a user-friendly red error message is displayed instead.)*

### Question 3 — Compare Native JavaScript and jQuery (`jquery-dom.html`)
- **Action:** Open `jquery-dom.html` through **VS Code Live Server** (or a modern browser).
- **Initial Page State:** On page load, jQuery 4.0.0 automatically replaces `#myElement` text with `"Modified Text"` and applies the `.myStyle` class (coral background and `16px` padding) to `#myDIV`.
- **User Interaction:** Press the **Click me** button (`#myButton`).
- **Expected Result:** A browser alert dialog pops up displaying `"Button clicked!"`.

## Output Screenshots
### Question 1 — Validated `books.json`
<img width="975" height="283" alt="image" src="https://github.com/user-attachments/assets/3d9158ad-206a-456f-a27b-6cc2b7d40f34" />


### Question 2 — JSON Data Displayed via `fetch()` (`books.html`)
<img width="436" height="301" alt="image" src="https://github.com/user-attachments/assets/1f85fcfd-50e6-4b29-a622-effab6490145" />


### Question 3 — jQuery DOM & Event Operations (`jquery-dom.html`)
<img width="820" height="435" alt="image" src="https://github.com/user-attachments/assets/f8091e7e-b4e9-4531-830f-<img width="895" height="403" alt="image" src="https://github.com/user-attachments/assets/f94af216-f3f5-47bd-9522-8024a1888523" />

