---
name: ig-profile
description: "Write or improve an Instagram profile: name field, bio, call to action, link and Highlights. Use when the user asks for a bio, wants their profile improved, or is setting up a new Instagram account."
---

# Instagram profile

Read `.claude/ig-brands.md` first for the brands, voice, language and rules. If it is missing, ask the user for the account, niche, audience and language.

## Steps

1. Ask for or read the current profile text if the user has one. Claude
   cannot open the profile, so work from what the user pastes or uploads.
2. Name field (30 characters at most): the brand plus searchable words
   such as "Treks" or "Pune", because this field is searched.
3. Bio (150 characters at most), in 3–4 short lines:
   who it is for, what they get, a proof point if the user supplied one,
   and one call to action.
4. Link: say what it should point to (WhatsApp, booking form, website).
5. Highlights: 4–6 names of up to 10 characters each, with what goes in
   each, for example Treks, Reviews, FAQ, Book.

## Output

Give 3 bio options with a character count for each, one recommended name
field, the link advice and the Highlights list. Count characters properly;
do not estimate.
