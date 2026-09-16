# timeboard-privacy

The public privacy policy and data-deletion page for **TimeBoard**, the Android countdown-board app published by Overdrive Labs (`com.overdrivelabs.timeboard`). Both pages are single self-contained HTML files with no external assets, covering English, ไทย, 日本語 and 한국어, and they describe the app as it actually ships — currently version 0.3.0.

Published at **https://overdrivelabs998.github.io/timeboard-privacy/** (the data-deletion page is at `/delete-data.html`); those are the URLs used in the Google Play listing.

## For maintainers

Edit `index.html` and `delete-data.html` directly, update the "Last updated" date and the version line in all four languages, then commit and push to `main` — GitHub Pages redeploys the site automatically. Whenever the app gains or loses a permission, a stored field, or a third-party SDK, update the policy **before** that app version is released, so the page linked from Google Play always matches the app on Google Play.
