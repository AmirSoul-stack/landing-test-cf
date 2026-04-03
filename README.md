# landing-test-cf

Test repository for a static landing page using this workflow:

**Codex -> GitHub -> Cloudflare Pages**

## Purpose

This repository is only for testing the deployment flow before building the real landing page.

The goal is to verify that:

- Codex can create and update files in the repo
- GitHub stores the landing page files correctly
- Cloudflare Pages can deploy the site successfully

## Stack

This project uses:

- HTML
- CSS
- JavaScript

No frameworks, package managers, or build tools are required unless explicitly added later.

## Project structure

```text
.
├── AGENTS.md
├── README.md
└── site/
    ├── index.html
    ├── styles.css
    └── script.js
