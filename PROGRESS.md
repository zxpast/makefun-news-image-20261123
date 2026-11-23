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
  (local 473da16; remote HEAD 55dd5bf0c774bb8609e795af1a470f2a9ffafd4f,
  tree verified equal to local). Note: remote gained an extra commit
  8263a98a "Add .gitignore" first, because the API-created remote tree lacked
  .gitignore and the push helper requires the trees to match.

## EVENING REFRESH — DONE 23 Nov ~21:15 WIB (evening-refresh builder)
- Red-team F1–F5 + hydrogen F6–F11 applied (see BUILD-LOG.md for the
  item-by-item record). Headline fixes: Card #12 "COP31 aftermath: what's
  next?", Card #10 "Amit Shah launches projects" (complete phrase; the
  red-team's longer wordings are 3 lines at capH 12.5 — width-checked).
- F7: Card #9 RIYADH DROPPED — the Rabigh claim was Sunday 22 Nov
  (Reuters 22 Nov; IANS "on Sunday said"; no Monday angle exists).
  Replaced by Card #9 CONGO (cobalt export halt, Reuters Monday).
  DATE CHECK gained "Rabigh claim Sun"; "Houthi strikes Fri" kept
  (different event: Fri intercepts).
- W6 cricket final: Wellington Test DRAWN (NZ 239/5, Mitchell 49*,
  Phillips 26*; India 720/9 dec). Hero 2 + stats + kicker updated;
  scene reads "239/5 FINAL — DRAW" (labelled score).
- Hero 3 body: Zelenskyy's Monday confirmation (Ukraine sea drones hit
  the corvette Merkury); source Arab News → AP.
- Late-day briefs: BERLIN German PMI 55.0, WASHINGTON Dems 12 debates,
  DHAKA first measles-free day in 8 months (toll 1,352). Totals still 33
  stories; regions ASIA 13, AFRICA 2, EUROPE 9, MIDEAST 1, OCEANIA 4,
  AMERICAS 4.
- Card #11 Brentford v Everton kept as fixture (kickoff 20:00 UTC, result
  not in at build time).
- Render: 2 runs byte-identical, no WARN. md5
  cedec2d34e28a39dba280e34c5eb1e04, sha256
  88ff4db37fcdc49d7657d67bcd4ccac8e626851d650607e2f610fbf1ee7c3f2f,
  95,341 bytes (zlib level 9, P9 tie-break). 300px legibility + digit gate
  pass.
- Pushed: (remote HEAD recorded below after push_gitdata.py)
- DO NOT submit. DO NOT bundle. Main agent bundles (with --muse-usage) and
  submits in the 24 Nov 07:00 WIB wave (slot 3). Deadline 25 Nov 07:00 WIB.

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
