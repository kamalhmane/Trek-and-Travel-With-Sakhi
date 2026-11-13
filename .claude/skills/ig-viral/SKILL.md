---
name: ig-viral
description: "Generate Instagram Reel/video ideas built to maximise reach, with hooks, shot lists, captions and a posting plan. Use when the user asks for Instagram video ideas, Reel ideas, viral content ideas, hooks, or a weekly Instagram content plan (e.g. \"/ig-viral give me 3 video ideas for this week\")."
---

# Instagram viral video ideas

Produce ready-to-shoot Instagram Reel ideas for the user's account.

## 1. The account

Read `.claude/ig-brands.md` first for the brands, voice, language and rules. If it is missing, ask the user for the account, niche, audience and language.

For Trek & Travel with Sakhi, read `index.html` for the current trip, date
and price, and tie at least one idea to the next trip when one is listed.

## 2. Parse the request

- Count: the number the user gave; default 3.
- Period: default "this week".
- Language: match the user's language (Hindi, Marathi, Hinglish, English).
- If web search is available, check current trending audio and formats in
  the niche; never invent a trending sound name.

## 3. Write each idea

Mix formats across the set so no two ideas use the same one: mistake/myth
bust, behind-the-scenes process, numbered list, before/after, POV, story
with a twist, reply-to-comment.

For each idea give:

- **Title and length** (most Reels: 15–40 seconds).
- **Hook**: the exact on-screen text and spoken line for the first 2
  seconds. Specific to the niche, no generic "Did you know".
- **Shot list**: 3–7 numbered shots, each one line, filmable on a phone.
- **On-screen text** for each shot where it helps.
- **Audio**: voiceover, original audio, or "trending audio in your niche".
- **Caption**: at most 3 lines, with the first line restating the hook.
- **CTA**: one action that suits the format (share for relatable, save for
  lists, follow for a series, comment a keyword for leads).
- **Hashtags**: 3–5 niche tags, not generic ones like #viral.
- **Why it should work**: one line naming the signal it drives (watch
  time, shares, saves, comments).

## 4. Close with a posting plan

Give the days and times to post across the period, spaced out, in the
audience's time zone, and one tip on what to check in Insights afterwards
(3-second hold rate, average watch time, shares).

## Rules

- Ideas must be shootable by one person with a phone unless the user says
  otherwise.
- Do not promise virality or quote follower or view numbers as guarantees.
- No fake claims, fake reviews, or copying another creator's video
  shot for shot.
- Keep the whole answer scannable: one block per idea, no long intros.
