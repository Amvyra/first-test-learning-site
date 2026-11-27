---
name: page-builder
description: "Turns a description of a page into 2 quick mockups to choose from, then builds the real page in code and checks it on desktop and phone. Use when you want a new web page or section made from an idea."
---

# Page Builder

You describe a page in plain words ("a landing page for our heating pad, with
reviews and a big Shop button"). This skill shows two quick mockups, lets you
pick, builds the real page, and checks it before calling it done.

## When to use

- A new page, landing page or website section from an idea.
- A new section for a Shopify theme or a static site.
- Rebuilding a page that works but looks wrong.

For small fixes on a page that is already fine, use
`website-design:make-interfaces-feel-better` instead.

## Step 1: Understand the job

Find out, from the request and the project files (ask only what's missing):
- **What the page is for** and **the one action** it wants (buy, sign up, contact).
- **Who visits** and on what (most shop visitors are on phones).
- **What's fixed**: read `BRAND-KIT.md`, `DESIGN.md`, `CLAUDE.md`, a direction
  note from `website-design:moodboard`, and the existing site's code. Use its
  colors, fonts, buttons and card style. If a skill disagrees with
  `DESIGN.md`, `DESIGN.md` wins; say what you overrode.
- **Where it lives**: a plain HTML file, a Shopify theme section, or a
  framework the project already uses. Match the project. No new frameworks.

## Step 2: Plan the sections

Write the page as a short list, top to bottom. For each section: its job in
one line and the real words it needs. Use the brand's real facts (prices,
shipping, guarantees). Never invent reviews, numbers or claims; leave a clear
placeholder like `[real review here]` instead.

## Step 3: Two quick mockups

Build 2 rough versions as simple HTML (one file each, or two boards on one
page). Make them differ in layout or emphasis, not only in color, e.g. "A:
big photo first" vs "B: offer and reviews first".

Take a desktop (1440px) and a phone (390px) screenshot of each and show them.
Ask which one, or what to mix. Keep this fast: one more round at most.

## Step 4: Build the real page

- Clean, simple code that the owner can read. Comment only the tricky parts.
- Use the project's existing colors, fonts and pieces before making new ones.
- Phone first: everything fits on a 390px screen, tap targets are at least
  44px, text is at least 16px.
- Real headings in order (one `h1`), alt text on images, a page title and a
  meta description for Google.
- Every link and button goes somewhere real. No dead `#` links.

## Step 5: Check before saying "done"

If the project has its own check steps (for example in `CLAUDE.md`), follow
those. Otherwise:

1. **Test first, fix nothing yet.** Desktop (1440px) and phone (390px)
   screenshots, click every link and button, open the phone menu, try any
   forms, check text contrast. On the phone, measure that the page isn't wider
   than the screen (`document.documentElement.scrollWidth` should equal the
   window width), because screenshots don't show sideways scrolling.
   Write down every problem.
2. **Fix 3 problems at a time, then test again.** Stop when the list is empty
   or after 3 rounds, and report anything still broken.

Then hand off if useful: `website-checks:seo` for Google,
`website-design:mobile-native` for phone feel,
`website-checks:production-audit` before a launch.

## Tell the user

In plain words: what you built, where the file is, what you checked, and
anything still to fix or fill in (like placeholder reviews).
