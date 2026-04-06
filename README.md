# Jackline Namanda — Personal site & portfolio

A small static **personal website** with a **portfolio** page and a printable **résumé**, deployed to GitHub Pages from this repository.

## Pages

| Page | File | What it is |
|------|------|------------|
| Home | [`index.html`](index.html) | Landing: intro, focus areas, contact |
| Portfolio | [`portfolio.html`](portfolio.html) | Project cards (e.g. In Him, GitHub Delivery OS) linking to folders on this site |
| Résumé | [`resume.html`](resume.html) | Full skills and employment history |

Shared layout and styles live in [`css/styles.css`](css/styles.css) (sticky header, typography, cards, print rules).

## Local preview

```bash
python3 -m http.server 8080
```

Open `http://localhost:8080` — start from **Home** (`index.html`).

## GitHub Pages

The workflow in [`.github/workflows/deploy-pages.yml`](.github/workflows/deploy-pages.yml) publishes the **repository root** so subfolders such as `inhim/` and `github-delivery-operating-system/` stay available at the same paths as in development.

## Print / PDF

Open **Résumé** and use **Print → Save as PDF**. Print styles hide the site chrome and keep the résumé content readable.

## Adding portfolio projects

Edit `portfolio.html`: duplicate a `<li class="repo-card">` … `</li>` block and update the `href`, title, and description.
