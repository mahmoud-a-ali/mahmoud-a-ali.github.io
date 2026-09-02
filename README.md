# mahmoud-a-ali.github.io

Personal academic website for **Mahmoud Ali** — Robotics Ph.D. candidate at Indiana University (VAIL).

Live site (after deploy): <https://mahmoud-a-ali.github.io>

Plain HTML/CSS — **no build step, no Jekyll**. GitHub Pages serves the files as-is
(`.nojekyll` is included so nothing is processed).

## Structure

```
index.html            About + News + selected publications
publications.html     Full publication list
cv.html               CV (experience, education, teaching, skills)
assets/
  css/main.css        Theme (edit colors via the :root variables at the top)
  img/profile.jpg     Profile photo  ← replace with a higher-res headshot anytime
  img/favicon.svg     Monogram favicon
  pdf/Mahmoud_Ali_CV.pdf   Downloadable CV  ← replace with your latest CV
.nojekyll             Tells GitHub Pages to skip Jekyll processing
```

## Edit the content

- **Bio / research:** `index.html` → `#about` section.
- **News:** `index.html` → `#news` list (newest first).
- **Publications:** add a `.pub` block in `publications.html` (and, if notable, in the
  "Selected publications" section of `index.html`).
- **Colors / fonts:** the `:root` block at the top of `assets/css/main.css`
  (`--accent` is the crimson used throughout).

## Preview locally

```bash
cd mahmoud-a-ali.github.io
python3 -m http.server 8000
# open http://localhost:8000
```

## Deploy to GitHub Pages

1. Create a **public** repo on GitHub named exactly `mahmoud-a-ali.github.io`.
2. Push this folder:
   ```bash
   git remote add origin https://github.com/mahmoud-a-ali/mahmoud-a-ali.github.io.git
   git push -u origin main
   ```
3. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch `main` / `/ (root)`. Save.
4. The site goes live at <https://mahmoud-a-ali.github.io> within a minute or two.
