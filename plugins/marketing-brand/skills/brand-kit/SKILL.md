---
name: brand-kit
description: "Reads a website and builds a brand kit from it (colors, fonts, tone, products, logo), then makes on-brand posts. Use when you start work for a brand or need posts that match a site."
---

# Brand Kit

Give it a website. It reads the site and writes down how the brand looks and
sounds in one file, `BRAND-KIT.md`. Then it uses that file to make a first
batch of social posts that look and sound like the brand, not like generic AI.

Every other skill (captions, carousels, campaigns, page designs) can then read
`BRAND-KIT.md` instead of guessing the brand again.

## When to use

- Starting work for a new brand, client or website.
- Posts or ads keep coming out generic and off-brand.
- Before a campaign, a redesign or a new landing page.
- The brand changed (new colors, new product, new tone) and the kit is old.

If a `BRAND-KIT.md` already exists, read it first and only update what changed.

## Step 1: Read the site

1. Open the home page, one product or service page, the About page and the
   FAQ if there is one. Four or five pages is enough.
2. Many sites (Shopify, Notion, Wix, React sites) build their pages with
   JavaScript, so a plain fetch comes back nearly empty. If that happens, open
   the page in a real browser (Playwright: `require('playwright')`,
   `chromium.launch()`), wait for it to load, then read `document.body.innerText`.
3. In the browser, read the real colors and fonts from the page itself:
   `getComputedStyle` on the body, headings, buttons and links. Don't guess
   them from screenshots.
4. Take one desktop screenshot of the home page for the kit.
5. If the site is password-protected or not live yet, ask for the password or
   use the source files you can reach (the theme code, a repo, a `DESIGN.md`).
   Never guess a password.

If the project has a `DESIGN.md`, `CLAUDE.md` or brand notes, those win over
what you read on the site. Say where they disagree.

## Step 2: Write `BRAND-KIT.md`

Keep it to about one page. Use this shape:

```markdown
# Brand kit: <brand name>
Made from <url> on <date>.

## In one line
<what they sell, to whom, and why it's different>

## Who it's for
<the main customer, in plain words>

## Look
- Colors: <name> #hex (used for…), …   Main accent: #hex
- Fonts: headings <font>, body <font>
- Shapes: <rounded / sharp, buttons, cards, shadows>
- Photos: <style: real / studio / lifestyle, light, mood>
- Logo: <where it is, colors, any rules>

## Sound
- Tone in 3 words: <…>
- Sentences: <short / long, simple / technical>
- Words they use: <…>      Words they never use: <…>
- 3 real lines from the site that sound most like them:
  > …

## What they sell
| Product | Price | The 1 thing to say about it |

## Selling points (in their order)
1. …

## Rules
- <anything to always or never do, e.g. "free shipping is US only">
```

Save it where the user's project files live (the project root, or next to the
site's code). Show the user a short summary, not the whole file.

## Step 3: Make the first posts

Make **5 post ideas** from the kit, each a different job:

1. Show the product solving the main problem.
2. A selling point most people don't know.
3. A tip for the customer, not about the product.
4. A question or a this-or-that to get comments.
5. A soft offer (a deal, free shipping, a gift).

For each one give: the format (reel, carousel, single image, story), the hook
line, the caption, and an image idea written as a prompt that names the
brand's colors, light and photo style from the kit.

Then hand off:
- Captions → `instagram:ig-caption`, swipe posts → `instagram:ig-carousel`,
  reels → `instagram:ig-reel`, then `instagram:ig-human` before anything is posted.
- Real images: use Canva or Higgsfield if they are connected. **Ask before
  making images that cost credits**, and say roughly how many credits.

## Checks before you finish

- Every color in the kit is a real hex from the site or the design notes.
- The 3 example lines are quoted from the site, not written by you.
- No made-up facts: prices, shipping, guarantees and claims all come from the
  site or the user.
- Posts use the kit's words and avoid its "never" words.
