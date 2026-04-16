# Scrum Workflow

This repo contains the working version of the team's scrum ticket status workflow.

## Web View

The browser-rendered version lives in `index.html`. It now loads diagram content from Markdown files listed in `diagrams/manifest.json`, so the webpage and the Markdown source stay in sync.

## Diagrams

- `diagrams/story-status-workflow.md`: current workflow diagram source
- `diagrams/manifest.json`: list of diagrams shown in the browser switcher

## Notes

When the page is served over GitHub Pages or any local web server, `index.html` fetches the Markdown files directly and renders the first Mermaid code block it finds. Browsers usually block that fetch behavior on raw `file://` URLs, so local preview should use a small HTTP server if needed.
