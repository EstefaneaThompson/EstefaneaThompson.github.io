# AGENTS.md

This file provides context and instructions for AI coding agents (Claude, Codex, Copilot, etc.) working on this repository.

---

## Project Overview

This is a personal portfolio website for **Cecilia Thompson** — a Business Intelligence & Analytics professional based in Tulsa, OK.

The site is a **static HTML/CSS/JS portfolio** — no frameworks, no build step, no package manager required. It is designed to be deployable directly via GitHub Pages, Netlify, or Cloudflare Pages.

---

## Stack

| Layer      | Technology                        |
|------------|-----------------------------------|
| Markup     | Semantic HTML5                    |
| Styling    | Vanilla CSS (custom properties)   |
| Behavior   | Vanilla JavaScript (ES6+)         |
| Fonts      | Google Fonts (Inter + Playfair Display) |
| Icons      | None (CSS-only decorative elements) |
| Hosting    | GitHub Pages / Netlify / Cloudflare Pages |

---

## File Structure

```
cecilia-portfolio/
├── index.html          # Home / Hero / All sections (single-page)
├── css/
│   └── style.css       # All styles — variables, layout, components
├── js/
│   └── main.js         # Scroll behavior, nav highlight, animations
├── assets/             # Images, resume PDF, OG image
├── .gitignore
├── AGENTS.md           # You are here
└── README.md
```

---

## Design Tokens

All colors, type sizes, and spacing are defined as CSS custom properties in `css/style.css` under `:root`. **Do not hardcode values** — always reference a CSS variable.

Key variables:
- `--color-bg`: page background
- `--color-surface`: card/section surface
- `--color-text`: primary text
- `--color-text-muted`: secondary/meta text
- `--color-accent`: primary brand accent
- `--color-accent-soft`: light tint of accent for backgrounds
- `--font-display`: display/heading typeface
- `--font-body`: body/UI typeface

---

## Coding Conventions

- **Semantic HTML**: use `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<footer>` correctly.
- **BEM-like class names**: `.section-header`, `.card__title`, `.nav__link--active`.
- **Accessibility**: every interactive element must have visible focus state. Images must have `alt`. Color contrast must meet WCAG AA.
- **No inline styles** unless dynamically applied by JavaScript.
- **Mobile-first**: write base styles for mobile, then `@media (min-width: ...)` for larger breakpoints.
- **No external JS libraries** unless explicitly approved. Keep the bundle zero.

---

## Content Guidance

Cecilia's story is the hero of this site:
- Arrived from Brazil in 2015 with no English and no degree.
- Earned a B.S. in Management Information Systems from Oklahoma State (2024).
- Master's in Business Analytics & Data Science (OSU, expected Dec 2026).
- Now a BI & Reporting professional at Williams Companies (Fortune 500).

**Tone**: Professional, confident, warm. Not corporate-stiff. Her journey is an asset — reference it with pride, not apology.

---

## Agents: What to Do

- Follow the design token system — never break the palette.
- Keep all sections in `index.html` in order: Hero → About → Skills → Experience → Education → Contact.
- Resume link should point to `assets/resume.pdf` (user will drop their actual PDF here).
- Do not add unnecessary dependencies.
- When adding or editing copy, match the existing tone and voice.
- Run an accessibility pass (contrast, focus states, alt text) before considering any task done.
