# Ankush Yadav — Portfolio

A single-page portfolio: one `index.html` with no build step or dependencies (fonts load from Google Fonts).

## Before you publish

Everything is filled in: links, email, `resume.pdf`, experience, projects and education. When you update your resume, replace `resume.pdf` and keep the same file name.

If you add something you're not sure about yet, wrap it in `<span class="todo">…</span>`. It will show in a dashed orange box until you remove the wrapper.

## Deploy on GitHub Pages

**Option A: `username.github.io` (recommended, gives the cleanest URL)**

1. Create a new public repo named exactly `ankushyadav1979.github.io`.
2. Upload `index.html` and `resume.pdf` (Add file → Upload files → Commit).
3. The site goes live at `https://ankushyadav1979.github.io` within a minute or two.

**Option B: any repo name**

1. Create a repo (e.g. `portfolio`) and upload the files.
2. Go to **Settings → Pages → Build and deployment**, choose **Deploy from a branch**, then pick `main` and `/ (root)`, and save.
3. The site goes live at `https://ankushyadav1979.github.io/portfolio`.

From the command line:

```bash
git init
git add index.html resume.pdf README.md
git commit -m "Portfolio"
git branch -M main
git remote add origin https://github.com/ankushyadav1979/ankushyadav1979.github.io.git
git push -u origin main
```

## Editing

- **Add a project:** copy one `<article class="project">…</article>` block in the Projects section.
- **Change colours:** edit the tokens at the top of the `<style>` block (`--accent`, `--ink`, etc.). Dark mode uses the second set.
- **Hero chart:** simulated geometric Brownian motion paths are drawn in the `<script>` at the bottom. `MU` and `SIGMA` set drift and volatility, and **Resample** draws a new set.
