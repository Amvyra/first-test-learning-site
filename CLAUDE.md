# CLAUDE.md

Notes for Claude about this project. Read at the start of every session.

## About the business
- **Amvyra** sells heating pads for pets (dogs and cats).
- Key selling points: auto shut-off, 9 heat levels, free shipping, pet-safe gentle heat, soft easy-to-clean covers.
- Tagline used on the site: "Warmth for every paw".

## The real store (Shopify)
- The real store is **amvyra.com**, built on **Shopify** (Basic plan, prices in USD).
- This GitHub repo is only a **practice/test site** for learning Claude Code and GitHub. It is not the real store.
- Status (Nov 2026): not launched yet. Visitors see a password-protected "Opening soon" page.
- Live theme: "Amvyra main 2.0" (published Nov 22; a copy of "Amvyra main" with a reworked heating pad product page). "Amvyra main backup" is kept unpublished as the backup. Older drafts were deleted.
- Redesign draft: "Amvyra redesign (Nov 22)", unpublished, a copy of "Amvyra main backup" (the backup was renamed by the owner). Concept "Frost outside, ember inside": midnight/paper surfaces, logo red-to-orange gradient, Fraunces + Figtree, new sections `amv-hero`, `amv-split`, `amv-spotlight`, `amv-heat-dial` (with tip box), plus product-page tools `amv-fit` (size check) and `amv-run-cost` (running cost), styles in `assets/amvyra-redesign.css`, rules in the theme's `DESIGN.md`. Created by Claude, so Claude can publish it if the owner says yes.
- Theme design polish lives in `assets/amvyra-polish.css` (loaded after `base.css` in `layout/theme.liquid`).
- Shipping: free on every order in the US ("Free shipping on every pad" across the site and the Shipping Policy page). Optional "Package protection" ($4.99) is offered at checkout on purpose; leave it.
- Delivery: 10 to 16 days from order (ships in 1–3 days), U.S. only. Email replies: within 24–48 hours. Main menu: Home page, Shop the pad, Contact, Track Your Order, FAQ. FAQ and Shipping Policy pages match this (updated Nov 22).
- Reviews: Judge.me. Offers/bundles: Pumper Bundles (colors set in the app; the redesign overrides the selected-offer outline and the review button in theme CSS).
- Shopify blocks deleting themes, and publishing themes Claude didn't create, through the connection; the owner does those in admin.
- Changes to the real store go through the Shopify connection, not this repo. Always ask before changing anything in the store.

### Products
- **Main product:** Amvyra Auto Shut-Off Pet Heating Pad (Grey), **$64.99**. For cats and small dogs: 9 heat levels, timer that switches it off on its own, wipe-clean surface, chew-resistant cord.
- **Free gifts with purchase** (active, product type "Free Gift Items"):
  - Faux Fur Pad Cover (Grey or Brown), listed at $25.00. Zips onto the heating pad.
  - Pet Grooming and Massage Glove, listed at $12.99.
  - Obstacle-Dodging Pet Ball, listed at $12.99.
- **Drafts (not visible yet):** USB Heated Pet Bed ($69.99), Cat Teaser Wand, Cat Nail Clipper, Paw & Nose Balm.
- **Archived:** older non-pet products from before the store focused on pets, and an older 3-setting heating pad. Ignore these unless asked.

### Collections and pages
- Collections in use: Home page, Winter Pet Essentials, Free Gifts.
- Published pages: Contact, FAQ, Shipping Policy, Your Privacy Choices.
- "cozyden" (probably an earlier store name) remains only in the archived Dog Chew Toy Carrot Rope's handle. The USB Heated Pet Bed's handle was changed to `amvyra-usb-heated-pet-bed`.

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
