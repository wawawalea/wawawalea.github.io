# Lea Li 李冰睿 — Personal Website

A clean, single-page academic + project portfolio. Plain HTML, CSS & JS — no build step, no dependencies.

## Local preview

```bash
cd ~/lea-website
python3 -m http.server 8000
# open http://localhost:8000
```

## Files

| File | What it is |
|------|------------|
| `index.html` | All page content (Hero, About, Research, Projects, Contact) |
| `styles.css` | Theme — edit the `:root` variables at the top to recolor |
| `script.js` | Nav, mobile menu, scroll reveal |
| `.nojekyll` | Tells GitHub Pages to skip Jekyll processing |

## Editing content

- **Name / tagline / bio** — top of `index.html`, in the `.hero` section.
- **Projects** — the `.cards` block. Each `<a class="card" href="...">` points to a repo; swap the `href` for direct project links.
- **Links** — GitHub, email, and Scholar appear in the hero, contact section, and footer. The Scholar link is a placeholder (`scholar.google.com`) — replace with your profile URL once you have one.
- **Colors** — change `--indigo` (and friends) in `styles.css`.

## Deploy to GitHub Pages

Push the contents of this folder to a `username.github.io` repo (or any repo with Pages enabled on the `main` branch, root folder). The site is fully static.

```bash
git init
git add .
git commit -m "Personal website"
git branch -M main
git remote add origin https://github.com/wawawalea/wawawalea.github.io.git
git push -u origin main
```

Then: repo **Settings → Pages → Deploy from a branch → main / (root)**.
