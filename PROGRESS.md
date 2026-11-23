# PROGRESS — news-image-20261123 (continuation build, 23 Nov 2026)

## DONE (as of ~10:00 WIB, 23 Nov)
- Morning draft's story set was almost entirely wrong-day; rebuilt from verified
  Monday-23-Nov items only (see RESEARCH.md "REBUILD PASS" for every verdict).
- 33 stories: 3 heroes (Modi–Shah talks; NZ–India Test Day 5; UN Benghazi probe),
  10 cards, 20 briefs. Regions: ASIA 14, EUROPE 8, OCEANIA 5, AMERICAS 3,
  MIDEAST 2, AFRICA 1. DATE CHECK box lists 17 wrong-day exclusions.
- main.ts: Node 22 stdlib-only, no network, deterministic. New 'port' scene
  (Benghazi) + 'chart' icon; region strip two-pass draw; DATE CHECK 3 lines.
- Verification: 2 runs byte-identical,
  sha256 a1d56dc2b0df786d5130e94e1baf43db72ea20d42ddb79251751d3d5b73921f4,
  entry.png 90,150 bytes, 1024x1024, no WARN. Viewed at 2x/8x zoom: heroes,
  cards, briefs, map pins, region strip, DATE CHECK all legible.
- Committed + pushed to https://github.com/zxpast/makefun-news-image-20261123
  (commit hash in git log).

## REMAINS — evening refresh ~21:00 WIB (14:00 UTC)
1. Cricket final result (NZ–India, Wellington Day 5) — update HERO 2 headline,
   body, scene score (currently 157/4 at lunch, six wickets to get), and STATS.
2. Brentford v Everton result (~22:00 UTC) — update card 11 if result is in;
   if not, keep the fixture wording.
3. US daytime news + Monday bulletins (e.g. Bangladesh measles Monday bulletin;
   WHO Ebola team Monday evacuation, if any; Sparta II Monday update, if any).
4. Re-render twice, confirm byte-identical + no WARN, view the PNG, re-push.
5. DO NOT submit. DO NOT bundle. Main agent bundles (with --muse-usage) and
   submits in the 24 Nov 07:00 WIB wave (slot 3). Deadline 25 Nov 07:00 WIB.

## KNOWN WEAK SPOTS (acceptable, do not block)
- Briefs are 2-line fine print (capH 8) — dense at 300px, heroes/cards carry it.
- 'duet' scene figures are small (pre-existing).
- NZ retail sales released 21:45 UTC Sun = Monday 10:45 NZDT (footer covers
  "in some time zone").
