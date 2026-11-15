# CLAUDE.md

Notes for Claude about this project. Read at the start of every session.

## About the business
- **Amvyra** sells heating pads for pets (dogs and cats).
- Key selling points: auto shut-off, 9 heat levels, free shipping, pet-safe gentle heat, soft easy-to-clean covers.
- Tagline used on the site: "Warmth for every paw".

## Brand and tone
- Friendly, warm, cozy tone. Short, simple sentences.
- Colors (defined as CSS variables in `index.html`):
  - Background: `#fdf8f3` (warm cream)
  - Text: `#2b2420`, muted text: `#6b5f57`
  - Accent orange: `#e0703a` (hover: `#c65a27`)
- Fonts: **Fraunces** for headings and the logo, **Inter** for body text (Google Fonts).
- Rounded shapes: pill buttons, cards with rounded corners and a soft orange glow shadow.

## The site
- Single static page: `index.html` with all CSS inline in a `<style>` tag. No build step, no frameworks.
- Current sections, top to bottom: header (logo), hero with "Shop now" button, footer.
- A "3 reasons to choose Amvyra" cards section was tried and removed on purpose. Don't add it back unless asked.
- Known gap: the "Shop now" button links to `#shop`, but no element has that ID yet.

## How to work here
- The owner is learning, so explain changes in plain language and keep the code simple.
- Keep new sections consistent with the existing colors, fonts and card style.
- Make sure pages work on phone screens (no sideways scrolling).
- Commit and push finished changes to the working branch.
