---
name: ig-plan
description: "Build an Instagram content calendar for a week or a month, with the format, topic, hook and goal for each day. Use when the user asks for a content plan, posting schedule, content calendar, or what to post this week or month."
---

# Instagram content plan

Read `.claude/ig-brands.md` first for the brands, voice, language and rules. If it is missing, ask the user for the account, niche, audience and language.

## Steps

1. Take the period (default: 7 days), how many posts per week the user
   can manage (default: 4 feed posts plus daily stories), and any trips
   to promote with their dates.
2. Balance the content: roughly half to reach new people (Reels), a
   quarter to build trust (reviews, behind the scenes, history stories),
   and a quarter to sell (trip announcements, last seats).
3. Build up to each trip date: announce, explain, show proof, last call.
4. Fit the season and any festival or long weekend in the period. Check
   dates rather than guessing them.

## Output

A table with one row per day: date and day, format (Reel, carousel,
photo, story), topic, hook line, goal, and call to action.

Below it: what to shoot in one batch for the week, and which skill to run
next for each item (`ig-reel`, `ig-carousel`, `ig-story`, `ig-caption`).
