# Northbound Signal Site - Codex Rules

This is a static GitHub Pages marketing site for Northbound Signal.

## Project Shape

- Plain HTML/CSS with no build step.
- Main files: `index.html`, `styles.css`, `404.html`, `assets/`, `CNAME`, `robots.txt`, `sitemap.xml`, favicon assets.
- Deployed from the `main` branch through GitHub Pages.

## Editing Rules

- Keep changes simple and static-site friendly.
- Preserve the custom domain in `CNAME`.
- Do not introduce a build framework unless Gustavo explicitly asks.
- Image prompts/checklists live in the private agents repo; do not duplicate private Agents context here.

## Bitwarden Secrets Manager

- Secrets are retrieved through Bitwarden Secrets Manager CLI (`bws`) using OS-provided auth environment variables, including `BWS_ACCESS_TOKEN` and `BWS_ORG_ID`. Do not print or log those values.
- If `bws` is not on PATH in the current shell, fix PATH/installation or ask Gustavo; do not copy secrets into files, chat, session logs, or persistent environment variables.
- Secret names are identifiers, not values. Fireflies uses the Bitwarden Secrets Manager secret named `FIREFLIES_API`; load it only into the process/session that needs Fireflies MCP access.
- Never write retrieved secret values to repository files, Obsidian notes, AGENTS/CLAUDE files, or session logs.

## Local Preview

Use a simple static server when needed:

```bash
python3 -m http.server 8080
```

## Session Logging

Log page/content changes and preview checks. Do not copy unrelated private Agents details into this folder.
