# ksnugroho.github.io

Personal academic website for **Kuncahyo Setyo Nugroho**, styled after an academic
faculty homepage, with the **IBM Plex Sans** typeface. Single static page, no build step.

## Files

| File | Purpose |
|------|---------|
| `index.html` | The whole site (HTML + CSS + JS inline) |
| `profile.jpg` | Profile photo, cropped 1:1 (640×640) |
| `cv.pdf` | Full CV — linked from the "Download CV" button |

## Publish to GitHub Pages

1. Create a repository named exactly **`ksnugroho.github.io`** under your account `ksnugroho`.
2. Put these three files in the repository root.
3. Push:

```bash
git init
git add index.html profile.jpg cv.pdf README.md
git commit -m "Add personal academic website"
git branch -M main
git remote add origin https://github.com/ksnugroho/ksnugroho.github.io.git
git push -u origin main
```

4. In the repo: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   branch **`main`**, folder **`/ (root)`**, then Save.
5. After a minute the site is live at **https://ksnugroho.github.io/**.

## Customizing

- **Content** lives directly in `index.html` as plain HTML — edit the text between the
  `<!-- ===== SECTION ===== -->` comments.
- **Colors / fonts** are CSS variables at the top of the `<style>` block (`:root`).
  The accent is IBM Blue `#0f62fe`; dark mode variables follow.
- **Theme toggle** (◐ in the nav) lets visitors switch light/dark; it also follows the
  OS preference by default.
- **Add social links** (Google Scholar, LinkedIn, ORCID): there is a commented-out
  template inside the `.social` block in the hero — uncomment and fill in your URLs.

## Notes

- The photo was cropped to a centered head-and-shoulders square from your original.
  Replace `profile.jpg` with any 1:1 image to change it.
- `cv.pdf` is your uploaded CV. Re-upload to update the download.
