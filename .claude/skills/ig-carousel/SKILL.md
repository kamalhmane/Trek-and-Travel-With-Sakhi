---
name: ig-carousel
description: "Plan an Instagram carousel slide by slide, with the text for every slide, a design note and a caption. Use when the user asks for a carousel, a swipe post, or a multi-slide guide, checklist or itinerary post."
---

# Instagram carousel

Read `.claude/ig-brands.md` first for the brands, voice, language and rules. If it is missing, ask the user for the account, niche, audience and language.

## Steps

1. Take the topic and goal. Default: 7 slides, goal saves.
2. Slide 1 is the hook: a promise or question in 8 words or fewer.
3. Slides 2 to the second-last carry one point each: a heading of up to
   6 words and a body of up to 20 words.
4. The last slide is the call to action: save, share, follow, or DM.
5. Order the slides so each one gives a reason to swipe to the next.

## Output

For each slide: number, heading, body text, and a one-line visual note
(photo to use, icon, or layout). Then:

- Design note: size 1080×1350, brand colours and logo placement from the
  brands file, the same layout on every slide.
- Caption and 3–5 hashtags.

If the user wants the slides made as images, build them as HTML, render
them to PNG at 1080×1350, and check each one before sending.
