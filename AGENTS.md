# AGENTS.md

## Project summary
This repository is a test landing-page project used to validate the workflow:
Codex -> GitHub -> Cloudflare Pages.

The site is a static website.
Default stack:
- HTML
- CSS
- JavaScript

Unless explicitly requested, do not introduce frameworks, package managers, or build tools.

## Primary goals
- Keep the project simple and easy to deploy
- Preserve a clean static-site structure
- Avoid unnecessary dependencies
- Make changes that are safe for GitHub + Cloudflare Pages deployment

## Repository structure
Expected structure:

- README.md
- AGENTS.md
- site/
  - index.html
  - styles.css
  - script.js

If new files are added, keep the structure organized and easy to understand.

## Working rules
- Prefer small, focused changes
- Do not rename core files or folders unless explicitly asked
- Do not delete existing content unless it is clearly obsolete or requested
- Do not add secrets, tokens, environment values, or private credentials
- Do not add backend services, databases, or server-side logic unless explicitly requested
- Do not add frameworks or libraries unless the task specifically requires them

## HTML standards
- Use semantic HTML where practical
- Keep structure clean and readable
- Use accessible markup when possible
- Ensure the page works as a static entry point from `site/index.html`

## CSS standards
- Keep CSS organized and readable
- Prefer simple, maintainable styling
- Avoid unnecessary complexity
- Preserve responsive behavior
- Do not use external CSS frameworks unless explicitly requested

## JavaScript standards
- Use plain JavaScript unless explicitly asked otherwise
- Keep scripts lightweight
- Avoid unnecessary abstractions
- Do not add dependencies for simple interactions
- Prevent console errors

## Deployment assumptions
Target deployment is Cloudflare Pages.

Default assumptions:
- No build step is required for this project
- Static output directory is `site`
- `site/index.html` must exist
- Asset paths must work correctly in static hosting

## Testing and verification
Before considering work complete, verify:
- `site/index.html` exists
- CSS and JS are linked correctly
- The page can load as a static site
- There are no obvious broken paths
- There are no obvious console errors from the implemented code
- The result remains suitable for Cloudflare Pages static deployment

## Review guidelines
When reviewing or generating changes, prioritize:
- deployment safety
- simple file structure
- readability
- minimalism
- accessibility
- responsive layout
- absence of secrets
- no unnecessary dependencies

Flag as important:
- missing `index.html`
- broken relative paths
- code that requires a build step without request
- framework installation without request
- credentials or secrets committed to the repo
- changes that break Cloudflare Pages assumptions

## Change policy
Unless the user explicitly asks for a branch + PR workflow:
- small test changes may be committed directly to the working branch
- larger or riskier changes should be isolated clearly
- keep commits scoped to the task

If the user requests a pull request:
- create a focused branch
- keep the PR scoped to one objective
- summarize changed files clearly

## Preferred output style
When implementing tasks:
- state what was changed
- list created or modified files
- keep explanations concise
- note any assumptions
- note any manual follow-up needed in GitHub or Cloudflare

## When unclear
If requirements are ambiguous and the ambiguity affects structure, deployment, or tooling choices, ask for clarification before making major changes.
If the ambiguity is minor, choose the simplest static-site option and state the assumption.
