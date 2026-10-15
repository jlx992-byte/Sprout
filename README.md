# Sprout — Emory meal planner
A browser-local meal planner for Emory students living independently. No accounts, backend, build tools, external APIs, or dependencies.

## Run
Open `dist/index.html` in a modern browser, or serve the `dist` directory with any static web server.

## GitHub Pages
Create a GitHub repository and upload the three files **inside dist** (`index.html`, `style.css`, `app.js`) to its root. In Settings → Pages, choose Deploy from a branch, then main and / (root). Save. GitHub provides the published URL. Alternatively retain this repository structure and deploy `dist` using a Pages workflow.

## Features
- Daily clipboard, date picker, past and future meals
- Meal names, descriptions, breakfast/lunch/dinner/snack categories
- Ingredient quantities and manually entered calories, protein, carbs, fat
- Planned daily totals and eaten calorie total
- Pantry quantities, units, optional date reminders
- Mark eaten to deduct linked inventory; undo to restore
- Quantity checks, matching-unit checks and grouped deductions
- Weekly waste logging with quantities grouped by unit; undo restores stock
- Responsive layout, native accessible dialogs, browser storage

Nutrition applies to the entered ingredient quantity, not per 100g. Pantry links require matching units; no implicit conversions. Unlinked ingredients are tracked nutritionally but do not affect inventory. Dates are user reminders, not food-safety judgments. No environmental impact or health outcome claims are calculated.

Data stays in localStorage for this browser and site origin. Clearing browser data removes it; switching devices, browsers or hosting addresses does not transfer it. Storage failures show a visible warning.

Independent student project, not affiliated with Emory University.
