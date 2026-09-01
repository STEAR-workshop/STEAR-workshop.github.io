# STEAR Workshop Website

Landing page for **STEAR — Self-Improving Robot Learning Through Experience and Reflection**, an ICRA 2027 workshop in Seoul, Republic of Korea.

Static HTML and CSS with local image assets. No build step.

## Files
- `index.html` — the entire page.
- `data/banner-icra2027.png` — ICRA 2027 Seoul/robotics hero image.
- `data/` — speaker, organizer, sponsor, and site style assets.
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

## Placeholders to fill in before launch
- Exact ICRA 2027 workshop date (May 24 or 28), time slot, and room.
- Submission deadline and notification date (Call for Papers → Key information).
- OpenReview submission URL and final participant paper template.
- Confirmed invited speakers, organizer affiliations, sponsor, and award details.
