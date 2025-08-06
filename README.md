# Typing Speed Test – Documentation

## Overview

This HTML file implements a simple yet effective typing speed test web application. Users can select a time duration, start the test, type the provided sample text, and at the end, see their typing speed (WPM), accuracy, and other statistics. The design is visually appealing with a gradient background and responsive layout.

---

## Table of Contents

1. Features
2. Layout & Styling
3. Usage Instructions
4. Code Structure
    - HTML Elements
    - CSS Styling
    - JavaScript Logic
5. Customization
6. Credits

---

## 1. Features

- Selectable test durations (1–5 minutes)
- Random sample text for each duration
- Preloader animation before the test starts
- Real-time countdown timer
- Input area for typing test
- Displays Words Per Minute (WPM), accuracy, and detailed results
- Responsive and modern UI

---

## 2. Layout & Styling

The application uses inline CSS to create:
- A centered container with rounded corners and shadow
- A gradient background for the whole page
- Styled select menus, buttons, and result display
- A preloader overlay with keyboard animation

---

## 3. Usage Instructions

1. Open the page in a web browser.
2. Select your desired test duration from the dropdown.
3. Click the "Start" button.
4. Wait for the preloader animation to finish.
5. When the sample text appears, start typing it exactly as shown.
6. When time runs out, see your results: WPM, accuracy, total words typed, and correct words.

---

## 4. Code Structure

### A. HTML Elements

- `<select id="time-select">`: Dropdown to choose test duration.
- `<button>`: Starts the test.
- `<div id="timer">`: Shows the time left.
- `<div id="text-display">`: Displays the sample text to type.
- `<textarea id="user-input">`: Where the user types.
- `<div id="results">`: Shows test results after completion.
- `<div id="preloader">`: Overlay loader with keyboard animation.

### B. CSS Styling

- Styles for background, container, buttons, select, textarea, and results.
- `.keyboard-animation`: Animates the keyboard emoji in the preloader.
- Responsive and visually appealing design.

### C. JavaScript Logic

#### Sample Texts

- `textSamples`: Object holding sample texts for each time duration.

#### Main Functions

- `showPreloader()`: Shows the loader for 6 seconds, then starts the test.
- `startTest()`: Triggers the preloader.
- `beginTypingTest()`: Initializes test, displays random sample, enables input, starts countdown.
- `finishTest()`: Disables input, calculates:
    - Words per minute (WPM)
    - Accuracy (percentage of correct words)
    - Total words typed
    - Number of correct words
  Displays results in the results div.

- Timer logic uses `setInterval` to decrement `timeLeft` every second.

---

## 5. Customization

- **Change sample texts:** Edit the `textSamples` object in the script section.
- **Adjust preloader time:** Change the timeout duration in `showPreloader()`.
- **Styling:** Modify the `<style>` block for colors, fonts, or layout.
- **Add more durations:** Extend the `textSamples` object and dropdown as needed.

---

## 6. Credits

- Developed by B-kaluwa.
- Source: [GitHub Repository](https://github.com/B-kaluwa/Typing-speed)

---

## File Location

- File: `typing_speed_test.html`
- Repo: `B-kaluwa/Typing-speed`

---

**For more information or to contribute, visit the repository or contact the maintainer.**
