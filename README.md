# Jackline Namanda — Resume

A single-page HTML resume for **Jackline Namanda**, focused on QA leadership, release management, technical program management, and AI-related delivery.

## Contents

- **Contact** — Location (Tacoma, WA), email, phone, and GitHub profile link
- **Skills** — Program management, QA & testing, cloud & DevOps, software development, AI, UI/UX, and documentation
- **Employment** — Workerbee Inc, Otic Group, Amazon Prime
- **Featured on GitHub Pages** — Cards link to the **project pages** on this site (`inhim/`, `github-delivery-operating-system/`). A line under the heading links to the **source repositories** on GitHub.
- **In Him — Daily Scripture (project page)** — `inhim/index.html` — GitHub links use **`jkaweesi22`** (matches this repo’s `origin`). Forks should search-replace if your handle differs.
- **GitHub Delivery Operating System** — `github-delivery-operating-system/index.html` — landing page for the Delivery OS framework (npm install, workflows table, docs links). Points at the public [Phaneroo](https://github.com/Phaneroo/github-delivery-operating-system) repo and npm package.

### GitHub Pages (GitHub Actions — recommended)

This repo includes [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml). It uploads the repository root as a static site on every push to **`main`** or **`master`** (and can be run manually under **Actions → Deploy GitHub Pages → Run workflow**).

1. Push this repository to GitHub (e.g. `Kaweesi-Resume`).
2. **Settings → Pages → Build and deployment:** set **Source** to **GitHub Actions** (not “Deploy from a branch”).
3. Merge or push the workflow to **`main`** / **`master`**. The first run may ask you to approve workflow permissions once.
4. After a successful run, the site base is `https://<username>.github.io/Kaweesi-Resume/`.
   - **Resume:** `https://<username>.github.io/Kaweesi-Resume/` (root `index.html`).
   - **In Him:** `https://<username>.github.io/Kaweesi-Resume/inhim/`.
   - **Delivery OS:** `https://<username>.github.io/Kaweesi-Resume/github-delivery-operating-system/`.

**Alternative:** you can still use **Deploy from a branch** (root `/`) instead of Actions; do not enable both at once for the same site.

Open `inhim/index.html` locally with the same static server as the resume to preview.

### Editing Featured on GitHub Pages

1. Card `href`s should point at **project folders** on this site (e.g. `inhim/`), not `github.com` URLs.
2. Keep **source repo** links in the intro paragraph (`repo-note`) so visitors can still open code on GitHub.
3. To add another project, add a subfolder with `index.html`, duplicate a `<li class="repo-card">` block, and link both the card and a source line.

## View locally

Open `index.html` in a browser, or serve the folder with any static file server.

```bash
# Example with Python 3
python3 -m http.server 8080
```

Then visit `http://localhost:8080`.

## Print / PDF

Use the browser print dialog (File → Print or **Cmd+P** / **Ctrl+P**) and choose “Save as PDF” for a clean export. Styles include basic print-friendly margins.

## Files

| File        | Description                    |
| ----------- | ------------------------------ |
| `index.html` | Resume markup and embedded CSS |
| `inhim/index.html` | In Him — Daily Scripture project landing page (GitHub Pages) |
| `github-delivery-operating-system/index.html` | GitHub Delivery OS — npm, workflows, documentation links |
| `.github/workflows/deploy-pages.yml` | Workflow that deploys the static site to GitHub Pages |
