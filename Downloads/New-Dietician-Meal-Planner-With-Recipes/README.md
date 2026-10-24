# New Dietician Meal Planner — first recommendations

This is a **separate** GitHub Pages website for the new dietician. It does not include records from Dr. Shikha's existing planner.

## Content added

- **9 distinct recipes / drinks**, matching the user's supplied notes. Pongal is one recipe used at breakfast, lunch or dinner, not three copied recipes. The ginger/coriander/chia/ghee drink is one recipe used both morning and night.
- **8 everyday schedule slots** from approximately 6:30 am through 30 minutes before bed, including an apple within 30 minutes of morning tea.
- **1 everyday leg-raise routine**, recorded exactly as advised without inventing a fixed time.
- A separate **`data/weekly-plan.json`** left unassigned, because no weekday-specific rotation was provided.
- Original wording preserved under each recipe's `source_text`; uncertainties listed in `needs_confirmation`.

## GitHub Pages: create the new repo

1. Create a **new** repository at <https://github.com/new> named `Dietician-Meal-Planner` (or a name of your choice). Your existing `Meal-Planner` repository is unchanged.
2. Extract the ZIP and upload **the actual files and folders**, not the ZIP itself, to the **root** of your new repo. The `data` directory must contain `recipes.json`, `daily-plan.json`, and `weekly-plan.json`.
3. Open the repository **Settings → Pages**, choose **Deploy from a branch**, select branch `main` and folder `/(root)`, then save.
4. For repository name `Dietician-Meal-Planner`, the expected site URL is `https://sakshi-vatsa.github.io/Dietician-Meal-Planner/` once GitHub publishes it. This URL is not live until the repository is created and deployed.

## How to add or adjust recipes

Update `data/recipes.json`. Each record stores an ID, name, allowed slots, portion, ingredients, instructions, alternatives, accompanying foods, source wording, clarification questions and optional video URLs. The website uses `data/daily-plan.json` to list the morning-to-night schedule and the IDs of available options. Keep the IDs stable and reuse them if one recipe belongs to multiple slots.

If the dietician gives a Monday/Tuesday rotation, add those choices to the empty `data/weekly-plan.json` (not shown on the site yet). Avoid assuming the everyday options are all meant to be eaten simultaneously.

## Source ambiguities that must not be guessed

- For **Pongal**, whether 70 g rice and 100 g moong dal are measured dry or after cooking; ghee, raisins and cashew quantities.
- For **rice and masoor dal lunch**, whether the 100 g amounts are raw or cooked.
- For **Rasam**, the source says `corridors` and `one half spoon` — confirm what ingredient and measure were intended. The source also gives a coffee mug but no volume.
- Other unspecified ingredient amounts remain unspecified, including for the drinks, apple toppings and moong dal chilla.
- The leg-raise duration is supplied, but the intended number of legs, exact positioning and daily timing aren't clarified.
- Breakfast allows black coffee; lemon juice is suggested, but no amount is specified.

## Privacy

This repository is for **public GitHub Pages hosting**. Its meal entries contain no name, email addresses, photos, weight, or other personal measurements. Do not add private dietician conversations or health records into a public repository. Follow the dietician's instructions where details are uncertain rather than improvising from the website.

The site runs as static HTML, CSS and JavaScript with local JSON. No analytics, login, external libraries or account access.
