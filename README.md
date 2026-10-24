# Everyday Meal Recipes — working GitHub Pages website

**Quickest fix:** Upload only `index.html` into the **root** of the
[`Everyday-Meal-Recipes`](https://github.com/Sakshi-Vatsa/Everyday-Meal-Recipes) repository, replacing the old `index.html`.
Commit to the branch serving GitHub Pages (usually `main`). The page is
self-contained and no longer needs any files in `data/` to display recipes.

Website: https://sakshi-vatsa.github.io/Everyday-Meal-Recipes/

## Contents

- `index.html`: fully standalone mobile-friendly meal planner, with embedded data.
- `data/recipes.json`: editable backup of 9 recipe/drink records, including original quantities and source wording.
- `data/daily-plan.json`: editable backup of 8 daily time slots and the everyday habit.
- `data/weekly-plan.json`: empty weekday assignments; no weekday-specific rotation was provided.
- `QUESTIONS-TO-CONFIRM.md`: outstanding questions about unclear portions and terminology.

## Important for future edits

Updating the JSON backups on GitHub **alone** will not update the live page.
The standalone `index.html` contains the same snapshot so it works without
file-path errors. When you provide additional recommendations, regenerate the
`index.html` snapshot from the updated JSON files, or request a new generated
HTML file. Keep both in sync when changing recipes.

## Privacy

The public site does not include Gmail links or message IDs, email addresses,
health records, or details from any other meal planner. GitHub Pages is public,
so don't commit private conversations or personal medical documents.
