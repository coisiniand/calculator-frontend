# Frontend Code Style Guide

This document defines the style standards for the front-end code of the calculator project. The goal is to keep the code clear, maintainable, and easy to read.

## 1. General Principles

- Keep the code simple and readable.
- Prefer clear naming over short abbreviations.
- Maintain consistent code formatting across the project.
- Keep functions and files focused on a single responsibility.
- Avoid unnecessary complexity.

## 2. HTML Standards

- Use semantic HTML elements where possible.
- Keep structure clean and easy to understand.
- Use meaningful class names and IDs.
- Avoid inline styles when styles can be placed in a CSS block.
- Maintain consistent indentation and spacing.

Examples:

```html
<div class="calculator-panel">
  <button class="operator" type="button">+</button>
</div>
```

## 3. CSS Standards

- Use lowercase class names.
- Use kebab-case for CSS class names.
- Group related styles together.
- Keep selectors simple and specific.
- Prefer CSS variables for repeated values such as colors and spacing.
- Avoid too many nested selectors.

Example:

```css
:root {
  --primary-color: #8b5cf6;
  --panel-bg: rgba(15, 23, 42, 0.8);
}

.calculator-panel {
  background: var(--panel-bg);
  border-radius: 18px;
}
```

## 4. JavaScript Standards

- Use `const` for constants and `let` for variables that may change.
- Use descriptive function names.
- Keep functions short and focused.
- Separate DOM logic from business logic when possible.
- Use clear event handling and avoid repeated code.
- Add comments only where they improve understanding.

Example:

```javascript
const display = document.getElementById('display');

function updateDisplay(value) {
  display.textContent = value;
}
```

## 5. Naming Conventions

- HTML/CSS: use `kebab-case` naming, e.g. `history-panel`, `clear-btn`
- JavaScript: use `camelCase`, e.g. `updateDisplay`, `fetchCalculation`
- Constants: use uppercase names when appropriate, e.g. `API_URL`

## 6. Frontend Interaction Rules

- Keep API requests simple and predictable.
- Handle loading and error states clearly.
- Avoid direct hard-coded logic when a reusable function is better.
- Keep user feedback obvious and accessible.

## 7. Example Structure

```html
<div class="calculator-app">
  <section class="calculator-panel">
    <div id="display">0</div>
  </section>
</div>
```

```javascript
function handleButtonClick() {
  const value = '1 + 2';
  updateDisplay(value);
}
```

## 8. Summary

The front-end code should be easy to understand, easy to maintain, and consistent in style. Clear structure, clear naming, and simple logic are the main goals of this project.
