# landing-test-cf

Test repository for a static landing page using this workflow:

**Codex -> GitHub -> Cloudflare Pages**

## Purpose

This repository is for testing the deployment flow before building the real landing page.

The goals are:

- verify that Codex can create and update repo files
- verify that GitHub stores the files correctly
- verify that Cloudflare Pages can deploy the site successfully

## Stack

- HTML
- CSS
- JavaScript

No frameworks, package managers, or build tools are required.

## Project structure

```text
.
├── AGENTS.md
├── README.md
└── site/
    ├── index.html
    ├── features.html
    ├── about.html
    ├── contact.html
    ├── thank-you.html
    ├── 404.html
    ├── styles.css
    └── script.js
```

## Cloudflare Pages settings

Use these settings in Cloudflare Pages:

- **Production branch:** `main`
- **Build command:** `exit 0`
- **Build output directory:** `site`

## Local preview

Open `site/index.html` in a browser.

## Notes

This is a test deployment project. The production landing page should be created in a separate repository or a separate Cloudflare project once this process is working.
