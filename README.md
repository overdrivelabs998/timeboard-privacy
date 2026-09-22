# timeboard-privacy

The public privacy policy, data-deletion page and feedback form for **TimeBoard**, the Android countdown-board app published by Overdrive Labs (`com.overdrivelabs.timeboard`). Each page is a single self-contained HTML file with no external assets, available in English, ไทย, 日本語 and 한국어, and describes the app as it actually ships — currently version 0.6.1.

Published at **https://overdrivelabs998.github.io/timeboard-privacy/**:

| Page | Path |
|---|---|
| Privacy policy (linked from Google Play) | `/` |
| Delete your data (linked from Google Play) | `/delete-data.html` |
| Feedback form (opened from the app's Help & Feedback) | `/feedback.html` |

## Languages

Every page shows **one language at a time**. It is chosen in this order: a `?lang=en|th|ja|ko` link, the visitor's saved choice, an old `#th`-style anchor, then the browser/device language list, falling back to English. The language button at the top left switches language, remembers the choice, and the page links carry `?lang=` so the choice follows the visitor. Without JavaScript all languages are shown one after another.

The language bar, its CSS and the two small scripts are copied identically into all three pages; change them in all three together.

## For maintainers

- **Privacy and delete pages:** each language is a `<section class="lang" lang="xx">` with its own title and "Last updated" line. Edit the text in all four sections, update the date and version line in each, then commit and push to `main`. GitHub Pages redeploys automatically.
- **Feedback page:** the form text lives in the `T` dictionary in its script, one entry per language. It sends nothing itself; it composes an email to overdrivelabs998@gmail.com.
- Whenever the app gains or loses a permission, a stored field, or a third-party SDK, update the policy **before** that app version is released, so the page linked from Google Play always matches the app on Google Play.
