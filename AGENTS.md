# Repository Guidelines

## Project Structure & Module Organization
- `index.html` is the entire site: markup, Tailwind configuration, and custom CSS live here.
- `README.md` contains hosting notes (Squarespace domain, Netlify hosting).
- There are no separate source, build, or asset directories; images and fonts are pulled from CDNs.

## Build, Test, and Development Commands
- No build step is required. Open the file directly for quick checks:
  - `open index.html`
- For a local server (useful for form behavior or absolute paths):
  - `python3 -m http.server` then visit `http://localhost:8000`
- Tailwind is loaded via CDN; changes are immediate on refresh.

## Coding Style & Naming Conventions
- HTML uses 4‑space indentation; keep blocks aligned and readable.
- Tailwind classes are the primary styling method; custom CSS belongs in the `<style>` block near the top.
- If you add new design tokens, extend `tailwind.config` in the embedded script.
- Keep IDs and anchor links in sync with navigation (e.g., `#about`, `#gallery`).

## Testing Guidelines
- There is no automated test suite.
- Manually verify:
  - Navigation anchors jump to the right sections.
  - Layout responsiveness at common breakpoints (mobile, tablet, desktop).
  - External assets load (fonts, icons, images).

## Commit & Pull Request Guidelines
- Git history is minimal and does not enforce a convention; use short, imperative messages (e.g., “Update hero copy”).
- PRs should include:
  - A concise summary of changes.
  - Screenshots or a quick screen recording for UI updates.
  - Notes on any external dependencies added or removed (CDNs, fonts, images).

## Hosting & Configuration Notes
- Site is hosted on Netlify with a Squarespace-managed domain (per `README.md`).
- The contact form uses Netlify’s form handling (`data-netlify="true"`); keep the hidden `form-name` input intact.
