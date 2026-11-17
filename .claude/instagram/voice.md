# voice.md

Every ig-* skill reads this file first. It covers two Instagram accounts, the
Marathi rules, and which bundled tools work on Marathi text. Keep it up to
date; the skills use it instead of asking the same questions again.

The skills come from https://github.com/Jakeschincariol/instagram-agent-skill
(MIT, see `.claude/skills/LICENSE-instagram-agent-skill`). The only local
changes: paths point at `.claude/instagram/` in this repository instead of
`~/.claude/instagram/`, and each SKILL.md points here first.

---

## Which account

If the user does not say, use the account the conversation is already about.
If that is unclear, ask once. Never mix the two in one post.

## Account 1: TouriKo

- **Handle:** @touri.ko
- **What it does, in one sentence:** Holidays and adventure trips, mainly treks
  to Sahyadri forts and nearby places in Maharashtra.
- **Tagline:** "Every Trip, A Story". Under the logo: "Holidays · Adventure".
- **Brand colours (from the logo):** yellow #fbdd21, blue #004aad, orange
  #f28d28. Blue backgrounds with yellow accents tested best with the owner.
- **Logo:** round yellow badge with blue mountains and an orange sun. Ask the
  user for the file if a design needs it.
- **What it sells:** treks and trips. Bookings by Instagram DM, unless the
  user gives a phone or WhatsApp number.

## Account 2: Trek & Travel with Sakhi

- **Handle:** @_with_sakhi (about 14k followers, as of November 2026)
- **What it does, in one sentence:** Guided treks and study tours
  ("अभ्यासपूर्ण भटकंती") to Sahyadri forts such as Raigad, leaving from Pune and
  Mumbai.
- **What it sells:** treks; bookings over WhatsApp. `index.html` in this
  repository holds the current trip, date and price. Read it before writing
  about a trip, and check that the date has not passed.
- **Also open to:** paid brand collaborations (trek gear, homestays, snacks,
  travel services). Paid or gifted posts must carry Instagram's "Paid
  partnership" label or #ad.

## Who both accounts talk to

Marathi-speaking trekkers and families, mainly in Pune and Mumbai, from
first-timers to regular weekend trekkers.

## What we sound like

- **On camera:** warm, practical, proud of Maratha history and the forts.
  Like a friend who has done this trek fifty times.
- **Language:** Marathi first for anything the audience reads or hears.
  Everyday spoken Marathi ("निघालाय", "येतंय", "नक्की"), not formal or
  translated-sounding words. Common English words people actually say are
  fine (ट्रेक, सेव्ह, फॉलो, जॅकेट). Reply to the user in the language they write in.
- **Words we use:** गड, किल्ला, सह्याद्री, भटकंती, पहाट, सूर्योदय, ट्रेकर्स.
- **Words we avoid:** stiff Sanskritised words where an everyday one exists
  ("पादत्राणे" → "बूट"), and English jargon such as "grip" or "sole" in
  voiceovers ("पकड", "तळवा").
- **Swearing:** no.
- **Emoji in captions:** a few, never one per line.
- **Voiceover or to-camera:** both. Marathi speech runs about 2–3 words a
  second; time scripts on that, not English words per minute.

## Season

Monsoon greenery (June–September), clear views and sunrise treks
(November–February), heat and night treks in summer (March–May).

## Off limits

- Never invent trip dates, prices, seat counts, phone numbers, reviews,
  follower numbers or results. Leave `{{blank}}` and ask.
- No false urgency ("last 2 seats") unless the user says it is true.
- Do not copy another creator's video or script; borrow the structure only.
- Claude cannot open Instagram. Work from what the user pastes, uploads or
  describes, and say what could not be checked.

## Proof we can use

Nothing confirmed yet. Ask the user for real numbers (treks run, trekkers
taken, reviews with permission) and add them here.

-
-

## The ask

- **Keyword CTA:** `TREK` (comment it to get trip details by DM). Confirm
  with the user before using it on TouriKo.
- **Where the link goes:** ask the user; not recorded yet.

---

## Bundled tools and Marathi text

The pack's Python tools were written for English. From reading their code:

- `ig-caption/caption.py`: **use it.** The 125-character feed window,
  hashtag count, link and line checks work on Marathi. Ignore its
  "concrete names" check, which only spots capitalised English words.
- `ig-human/humanize.py`: **use it for typography only** (em dashes,
  invisible characters, curly quotes). Its slop word list is English.
- `ig-human/detect.py`: **do not trust its score on Marathi.** It only counts
  English letters, so a Marathi draft scores as nearly empty. For Marathi,
  apply its five checks by judgement and say so.
- `ig-reel/hookscore.py`: **do not trust its score on Marathi** (English word
  lists). Score Marathi hooks by its five criteria by hand: says in under 3
  seconds, a concrete detail, something at stake, payload first, a clear
  viewer.
- `ig-reel/beats.py`: timing assumes English words per minute; check Marathi
  timing at 2–3 words a second instead.
- Run every tool on English text normally.
