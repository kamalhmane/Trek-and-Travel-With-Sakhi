---
name: ig-human
description: "Rewrite Instagram text so it sounds like a real person wrote it, not an AI or a brochure. Use when the user asks to humanize text, make a caption or script sound natural, or fix Marathi that sounds translated or robotic."
---

# Make it sound human

Read `.claude/ig-brands.md` first for the brands, voice, language and rules. If it is missing, ask the user for the account, niche, audience and language.

## Steps

1. Take the text and where it will be used (caption, voiceover, DM,
   comment).
2. Rewrite it the way the owner would say it aloud to a friend:
   - everyday spoken words, not formal or translated ones
   - short sentences of mixed length
   - one concrete detail in place of each general claim
   - natural spoken Marathi endings ("जाताय", "येतंय")
3. Remove: stock openers ("Are you ready to..."), rows of emoji, three
   adjectives in a row, hashtags inside sentences, and exclamation marks
   after every line.
4. Keep every fact, name, date and price exactly as given.

## Output

The rewritten text, then one line on what changed. For voiceover text,
also read it for rhythm: mark where to pause with a line break.
