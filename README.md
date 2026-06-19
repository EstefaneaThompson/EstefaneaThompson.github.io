# Cecilia Thompson — Personal Portfolio

> Business Intelligence & Analytics · Power BI · SQL · Databricks · OSU '24 · MS incoming Dec 2026

Live site: _add your URL here after deploying_

---

## About

Personal portfolio for Cecilia Thompson — BI & Analytics professional at Williams Companies (Fortune 500), OSU alumna (B.S. MIS, 2024), and Master's candidate in Business Analytics & Data Science (expected December 2026).

Arrived in the United States from Brazil in 2015 with no English and no degree. Built everything from scratch.

---

## Tech Stack

- **HTML5** — semantic, accessible markup
- **CSS3** — custom properties, flexbox, grid, no frameworks
- **Vanilla JavaScript** — scroll behavior, nav highlighting, animations
- **Google Fonts** — Inter (body) + Playfair Display (display)
- Zero dependencies. No build step required.

---

## Project Structure

```
cecilia-portfolio/
├── index.html          # Main single-page site
├── css/
│   └── style.css       # All styles and design tokens
├── js/
│   └── main.js         # Interactivity and scroll behavior
├── assets/
│   ├── resume.pdf      # → Drop your resume PDF here
│   └── og-image.png    # → Drop an OG/social image here
├── .gitignore
├── AGENTS.md           # Instructions for AI coding agents
└── README.md
```

---

## Getting Started

No build step needed. Open `index.html` directly in a browser, or serve locally:

```bash
# Option 1 — Python (built into macOS/Linux)
python3 -m http.server 3000

# Option 2 — Node
npx serve .
```

Then open `http://localhost:3000`.

---

## Deploying

### GitHub Pages
1. Push this repo to GitHub.
2. Go to **Settings → Pages → Source → main / root**.
3. Your site will be live at `https://<username>.github.io/<repo-name>`.

### Netlify (recommended — free, custom domain, HTTPS)
1. Drag and drop the project folder at [netlify.com/drop](https://netlify.com/drop), or connect your GitHub repo.
2. No build command needed. Publish directory: `.` (root).

### Cloudflare Pages
1. Connect your GitHub repo in the Cloudflare dashboard.
2. Build command: _(none)_. Output directory: `.`.

---

## Customizing Content

All content is in `index.html`. Search for `<!-- EDIT:` comments to find the easiest places to update:

- **Hero tagline** — `<!-- EDIT: hero -->`
- **About paragraph** — `<!-- EDIT: about -->`
- **Projects** — `<!-- EDIT: projects -->`
- **Contact links** — `<!-- EDIT: contact -->`

All design tokens (colors, fonts, spacing) are CSS custom properties in `css/style.css` under `:root`.

---

## Adding Your Resume

Drop your resume PDF into `assets/resume.pdf`. The "Download Résumé" button in the nav and hero will automatically link to it.

---

## License

Code: MIT. Content (copy, bio, work history): © Cecilia Thompson, all rights reserved.
