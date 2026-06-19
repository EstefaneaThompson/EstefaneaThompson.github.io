# AGENTS.md

AI coding agent instructions for this repository.

## Project
Personal portfolio website for **Cecilia Thompson** — BI & Analytics professional, Tulsa OK.

## Stack
Pure HTML5 / CSS3 / Vanilla JS. No frameworks, no build step, no npm. Deployable directly via GitHub Pages.

## File structure
```
/
├── index.html       Home
├── about.html       About
├── resume.html      Résumé (live page, not just a PDF link)
├── projects.html    Projects
├── contact.html     Contact
├── style.css        Shared design system — ALL styles live here
├── assets/
│   └── resume.pdf   Drop resume PDF here
└── AGENTS.md        You are here
```

## Design tokens (all in style.css :root)
- `--bg` `--bg2` `--bg3` — dark background layers
- `--border` `--border-soft` — subtle separators
- `--text` `--text-muted` `--text-faint` — text hierarchy
- `--accent` `--accent-dark` `--accent-glow` `--accent-faint` — rose pink (#E8709A)
- `--display` — Playfair Display (headings only)
- `--body` — Inter (all body text)
- `--mono` — monospace (dates, year labels)
- `--content-w: 680px` — max content width
- `--wide-w: 900px` — wide layout (nav, footer, home hero)

## Rules for agents
- NEVER hardcode colors — always use CSS variables
- NEVER add external JS libraries
- NEVER add a build step or package.json
- Keep all styles in style.css — no `<style>` tags in HTML files
- Every page must have: skip link, semantic nav with correct `nav__link--active`, `<main id="main">`, footer
- Accessibility: visible focus states, ARIA labels on nav/buttons, alt text on images
- Mobile first: base styles mobile, `@media (min-width:...)` for larger screens
- Add `.reveal` class to sections for scroll-in animation (already wired in JS)
