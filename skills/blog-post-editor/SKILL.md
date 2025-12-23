---
name: blog-post-editor
description: Create or edit blog-style posts on the 23 Tree Studio static landing page by directly editing index.html. Use when adding, updating, reordering, or removing post cards that include an image and excerpt, or when adding a blog/journal section if one does not exist.
---

# Blog Post Editor

## Overview
Add or update blog-style post cards in the static `index.html` for 23 Tree Studio. Posts are simple cards with an image, title, short excerpt, and optional date or category.

## Quick Start
1. Open `index.html`.
2. Find an existing blog/journal section (ids like `#blog` or `#journal`). If missing, insert a new section after `#gallery` and before `#visit`.
3. Duplicate a post card and update the image URL, alt text, title, date/category line, excerpt, and link.
4. Keep Tailwind classes and typography consistent with the rest of the page.
5. Verify responsive layout by keeping the grid classes intact.

## Use the Templates
- Use `assets/blog-card.html` for a single post card.
- Use `assets/blog-section.html` to scaffold a full blog section.

## Editing Guidelines
- Keep excerpts to 1-2 sentences (about 120-200 characters).
- Use descriptive alt text and https image URLs.
- Prefer simple HTML: `h3` for titles, `p` for excerpts.
- Keep anchors and navigation in sync if you add a new section link.

## Examples
- Add a new post for a workshop announcement with a new image and excerpt.
- Update the excerpt text for an existing post card.
- Reorder posts by moving card blocks within the grid.

## Files
- Primary file: `index.html`

## Assets
- `assets/blog-card.html`
- `assets/blog-section.html`
