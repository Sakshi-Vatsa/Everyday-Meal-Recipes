# Everyday Meal Recipes — refreshed website and app icon

This version removes all “Things to confirm” warnings from the website; retains the original leg-raise instruction without editorial commentary; corrects the Rasam ingredient to **1 teaspoon coriander**; and removes the incorrectly transcribed **2 teaspoons moong dal** from Rasam. The moong dal used in Pongal and chilla is unchanged.

The site contains 9 distinct recipes and drinks in 8 daily time slots. The data is bundled directly into `index.html`, so the page loads even when separate `data/` files are absent from your hosting setup. No personal records or Gmail links are included.

## Publish on GitHub Pages

Upload these **six** files to the root of https://github.com/Sakshi-Vatsa/Everyday-Meal-Recipes and commit:

- `index.html` (replaces previous file)
- `apple-touch-icon.png`
- `icon-192.png`
- `icon-512.png`
- `favicon-32.png`
- `manifest.webmanifest`

You may optionally upload the `data/` folder as a separately editable backup and `icon-options/` for future icon changes. They are **not required** for the website to work.

## Icon choice

The current default is **Option 8 — Terracotta steaming bowl** (warm rust-orange). It is deliberately different from Dr. Shikha's green plate-and-leaf icon. A sheet of 10 options is supplied as `icon-options.png`, and individual images in `icon-options/`. To switch, replace the four root PNG icon files with sizes exported from a different icon option. The manifest need not change as long as filenames stay the same.

On iPhone, remove the previous home-screen shortcut, visit the refreshed GitHub Pages URL in Safari and add it to Home Screen again to update the icon. On Android, remove and reinstall the shortcut or PWA after the deployment.

If you edit the JSON files, remember the page uses its *embedded* copy of the data. Editing `data/*.json` alone will not alter the live website.
