---
name: moodboard
description: "Makes 2 or 3 mood boards (colors, fonts, photos, sample buttons and cards) on one page so you can pick a look before anything is built. Use before designing a site, a page or a campaign."
---

# Moodboard

Before building a website, a new page or a campaign, show the user a few
clear "looks" side by side and let them pick one. It is much cheaper to change
a mood board than a finished site.

Each board is one look. All boards go on **one page** (an Artifact if you can
publish one, otherwise a single HTML file) so they are easy to compare.

## When to use

- Starting a new website, landing page or redesign.
- Planning a campaign, a launch or a seasonal look (Black Friday, winter…).
- The user says "I don't know what I want" or "make it look better".

Skip it for small fixes. Use `make-interfaces-feel-better` for polish instead.

## Step 1: Gather what's fixed

Read what already exists before inventing anything:
- `BRAND-KIT.md` (from `marketing-brand:brand-kit`), `DESIGN.md`, `CLAUDE.md`
  or brand notes. Their colors, fonts and rules stay unless the user wants a
  new brand.
- What the page or campaign is for, who sees it, and the one action it wants.

Ask at most 2 short questions if something big is missing. Otherwise decide.

## Step 2: Pick 2 or 3 directions

Make the directions **really different**, not three shades of the same idea.
Give each a short name and one line, e.g. "Cozy cabin: warm wood, soft light,
handwritten touches."

If the brand is fixed, keep its colors and fonts in every board and change the
other things: layout, photo style, mood, spacing, how loud the accent is.

## Step 3: Build each board

Each board shows, in this order:

1. **Name and one line** about the feeling.
2. **Colors**: 5 to 6 swatches with hex codes and what each is for
   (background, text, accent, button…). Check the text color on the
   background passes contrast (4.5:1 for normal text).
3. **Fonts**: a heading and a paragraph set in the real fonts (Google Fonts).
4. **Real pieces**: a sample button, a product card and a small hero strip
   built in HTML and CSS with the board's colors and fonts. This shows how
   the look works, not just how it feels.
5. **Photos**: 3 to 4 image tiles. Use one of these, in order:
   - the brand's own photos, if you have them;
   - images made with Higgsfield or Canva, if connected. **Ask before making
     images that cost credits**, and say roughly how many;
   - otherwise, simple CSS or SVG tiles with a written photo direction
     ("close-up, cat curled on a grey pad, warm window light").
6. **3 words** for the mood, and **1 thing to avoid**.

Keep the page phone-friendly: boards stack on a phone, no sideways scrolling.

## Step 4: Let them pick

Show the page, then ask which board they like, or what to mix ("colors from A,
photos from B"). Make at most one more round.

When they pick, write a short **direction note** (5 to 8 lines: colors, fonts,
photo style, mood words, the thing to avoid) and save it next to the project's
design notes. Then hand off:
- building a page → `website-design:page-builder`;
- design rules for a whole site → `website-design:frontend-design-direction`
  and `website-design:design-system`;
- a campaign → `marketing-brand:marketing-campaign`.
