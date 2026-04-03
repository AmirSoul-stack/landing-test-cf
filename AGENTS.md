# AGENTS.md

## Project
Static landing page test repo for the workflow:
Codex -> GitHub -> Cloudflare Pages.

## Rules
- Use plain HTML, CSS, and JavaScript only
- Do not add frameworks, npm, or build tools unless explicitly requested
- Keep changes simple and deployment-safe
- Do not commit secrets, tokens, or credentials
- Keep the `site/` structure intact unless explicitly instructed otherwise

## Required structure
- README.md
- AGENTS.md
- site/index.html
- site/features.html
- site/about.html
- site/contact.html
- site/thank-you.html
- site/404.html
- site/styles.css
- site/script.js

## Deployment assumptions
- Target: Cloudflare Pages
- No build step required
- Build command: `exit 0`
- Output directory: `site`
- `site/index.html` must remain the main entry point

## Review priorities
- Broken relative paths
- Missing static assets
- Console errors
- Unnecessary dependencies
- Anything that would break static hosting
