# STEAR Workshop Website

Landing page for **STEAR — Self-Improving Robot Learning Through Experience and Reflection**, a half-day CoRL 2026 workshop.

Single self-contained `index.html` (all CSS/JS inline) plus one image. No build step.

## Files
- `index.html` — the entire page.
- `static/images/stear_loop.png` — Figure 1 (reflection loop), extracted from the proposal PDF.
- `.nojekyll` — tells GitHub Pages to serve files as-is.

## Preview locally
```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to STEAR-workshop.github.io
This repo name must be `STEAR-workshop.github.io` under the `STEAR-workshop` GitHub org/user.
```bash
git init
git add .
git commit -m "Initial STEAR workshop site"
git branch -M main
git remote add origin git@github.com:STEAR-workshop/STEAR-workshop.github.io.git
git push -u origin main
```
Then in the repo's **Settings → Pages**, set the source to the `main` branch (root). The site goes live at https://STEAR-workshop.github.io.

## Placeholders to fill in before launch (currently marked "TBA")
- Exact date, time slot, and room within CoRL 2026 (hero fact bar + schedule note).
- Submission deadline and notification date (Call for Papers → Key information).
- OpenReview submission URL — replace the disabled `Open submission portal · TBA` button in the CFP section with a real link.
- Optional: speaker headshots (currently shown as initials avatars) and links to speaker homepages.
