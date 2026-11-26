---
name: pinterest-seo
description: >-
  The Pinterest SEO / search-ranking skill -- the keyword layer that pairs with pinterest-pin-design's visual.
  Use when someone wants pins to rank in Pinterest search, needs keyword research, or wants
  keyword-optimized pin titles/descriptions/boards. Pinterest is a visual search engine where keywords
  and relevance rank you, not followers. Uses the FOUND framework. Reads brand-profile + the pin's
  destination first. The agent researches real queries (autocomplete + Guided Search + Trends; never
  fabricates volume), writes the keyword-led title + a natural description (no stuffing), specs the
  on-pin overlay keyword, and advises boards + link. WoopSocial publishes the pin's title + description
  + board + link; profile/bio, board setup, alt text, Rich Pins, and Trends/Analytics stay native/human.
  No stuffing; Pin->Board->Page must match; fresh pins, not dupes. Distinct from pinterest-pin-design
  (the visual), pinterest-growth (the strategy), and social-seo (cross-cutting search).
version: 1.0.0
---

# pinterest-seo

The **keyword / search-ranking layer** — research the queries and write the keyworded words that make a pin rank. Read **brand-profile** and the pin's **destination** first.

## The POV: a visual search engine — keywords rank you, not followers
Pinterest is a visual search engine: ~97% of top searches are unbranded, follower count barely matters, and pins compound over a ~4-month lifespan — keywords, relevance and engagement rank you. Layer long-tail keywords profile → board → pin, align **Pin → Board → Page**, optimize for saves + long clicks. **Pairs with `pinterest-pin-design`** — the keyword goes in the overlay AND the title.

## The framework: FOUND
- **F — Find the real queries:** autocomplete, Guided Search bubbles + Trends/Predicts; long-tail (3+ words); never fabricate volume.
- **O — Optimize the pin's words:** title = `[Keyword] | [Benefit] | [Context]` (≤100 chars); natural description, no stuffing; spec the overlay keyword.
- **U — Unify Pin → Board → Page:** pin, board and destination reinforce one keyword phrase; claim the site + Rich Pins.
- **N — Nest keywords across every surface:** profile (broad) → boards (topic) → pin title/description/alt/file-name (long-tail).
- **D — Deploy fresh, in clusters, on a seasonal clock:** fresh pins (not dupes), in related clusters, seasonal 45–90 days ahead.

## Honest scope (never violate)
- Research real queries and advise the method — **never fabricate volume or rankings**.
- **No keyword stuffing / over-optimization** (suppressed); **Pin → Board → Page must match**; **fresh pins, not dupes**. Profile, board setup, alt text, Rich Pins and the research tools stay native/human.

## Operating rules (pack amendments — these override any third-party tooling mentioned elsewhere)
- Publish/schedule only with the Pinterest native scheduler, Tailwind, or the official Pinterest API v5. Never use a tool that asks for your Pinterest password.
- Every AI-image pin: turn on "Mark as AI-Modified". Verify the scheduled time after saving — the scheduler uses the timezone displayed on the account.
- Name image files with keywords; alt text on every pin (literal description, no stuffing); link to the page that matches the pin's content, not a generic homepage.

## Full version

This is a free lite preview. The complete skill — with all checklists, templates and references — is in the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
