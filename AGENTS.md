# Repository Guidelines

## Project Structure & Module Organization
- `index.html` is the home page: markup, Tailwind configuration, and custom CSS live here.
- `our-story.html` is the About / Our Story page. It follows the brand standards (gold `#D09F4F`, navy `#162C45`, cream `#F6F1E7`; Cormorant Garamond Italic SemiBold wordmarks; Montserrat Bold labels at 0.19em tracking). Photo slots are left as commented `PHOTO NEEDED` blocks until brand photography exists.
- `_redirects` maps `/our-story` and `/about` to `our-story.html` on Netlify.
- `docs/shopify-brand-copy.md` holds the paste-ready Shopify brand blurb and Juliette story line (Shopify is a separate property, not edited from this repo).
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
