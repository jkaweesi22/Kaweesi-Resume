# Jackline Namanda — Resume

A single-page HTML resume for **Jackline Namanda**, focused on QA leadership, release management, technical program management, and AI-related delivery.

## Contents

- **Contact** — Location (Tacoma, WA), email, phone, and GitHub profile link
- **Skills** — Program management, QA & testing, cloud & DevOps, software development, AI, UI/UX, and documentation
- **Employment** — Workerbee Inc, Otic Group, Amazon Prime
- **Featured on GitHub** — Card grid for repository links (edit URLs, titles, and descriptions in `index.html`)

### Adding GitHub repositories

1. Replace `YOUR_USERNAME` in the header GitHub link and in each repo `href`.
2. For each project, update `project-one` / `project-two` (the visible name), the description line, and the link.
3. To add another repo, duplicate an entire `<li class="repo-card">` … `</li>` block inside `.repo-grid`.

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
