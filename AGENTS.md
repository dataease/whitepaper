# Repository Guidelines

## Project Structure & Module Organization
- Root contains `DataEase-whitepaper.html` and its asset folder `DataEase-whitepaper.fld/` (images, header, theme files). 
- Keep relative paths intact: the HTML references assets by filename inside `.fld`.
- If adding assets, place them in `DataEase-whitepaper.fld/` and reference with relative paths.

## Build, Test, and Development Commands
- View locally: `open DataEase-whitepaper.html` (macOS) or double‑click in a file browser.
- Optional local server (helps with some browser policies): `python3 -m http.server` then open `http://localhost:8000/DataEase-whitepaper.html`.
- No build step; this is a static export.

## Coding Style & Naming Conventions
- HTML: keep semantic tags where possible; avoid inline styles unless necessary for fidelity.
- Assets: follow existing pattern `imageNNN.(jpg|png)` to keep ordering clear (e.g., `image063.jpg`).
- Indentation: 2 spaces for HTML; wrap lines at ~120 chars.
- Do not rename or move `DataEase-whitepaper.html` or the `.fld` directory.

## Testing Guidelines
- Visual check: open the HTML and verify all images render and links work.
- Links: ensure internal anchors resolve; use relative paths only.
- Accessibility spot check: provide alt text for new images where feasible.
- If large edits: test in at least two browsers (e.g., Safari/Chrome).

## Commit & Pull Request Guidelines
- Commit messages: use concise prefixes like `docs:`, `assets:`, `fix:` (e.g., `docs: update section 3 wording`).
- One logical change per commit; keep diffs focused on content you touched.
- PRs should include: short description, before/after screenshots for visual changes, and any manual test notes.

## Security & Maintenance Notes
- Do not embed secrets or tracking scripts.
- Keep external dependencies out of the repo; prefer self‑contained assets inside `.fld`.
- Large images: compress before adding to keep repo small.

## Agent-Specific Instructions
- When editing files, preserve file names and relative links in `DataEase-whitepaper.fld/`.
- Avoid restructuring; prioritize minimal diffs to maintain link integrity.
