# BUILD-LOG — news-image-20261123 EVENING REFRESH

Evening-refresh builder, 23 Nov 2026, ~20:45–21:15 WIB. Base: pre-work
W1–W5 render md5 `ebdfc3b7ff5c43dfc7ed158e3b7303b8` (verified by re-render
BEFORE any edit — byte-identical, 96,268 bytes). Remote HEAD verified
first-hand via gh_api.py before edits: `9f5e7cbc3e589df2e9c768187e998ec121ee96a3`
(unchanged since the main agent's check; local tree == remote tree).
Local HEAD at start: 74d8b2d (main.ts modified in place, uncommitted).

## F1–F5 (REDTEAM-LOG.md, 3.5-flash) — all applied
- F1 Brief #28 NEW DELHI: "Shah's visit is his first bilateral trip abroad
  as PM. (IANS)" → "Balen Shah's visit is his first trip abroad as PM.
  (IANS)" — names Balen Shah explicitly; "bilateral" dropped, still 2 lines.
- F2 Brief #20 GENEVA: "Gukesh and Sindarov hold media day; Game 1 Tuesday.
  (Chess.com)" → "Gukesh and Sindarov hold media day in Geneva. (Chess.com)"
  — "Game 1 Tuesday" (24 Nov) removed; media day was Monday.
- F3 Card #9 RIYADH headline "Houthis claim refinery strike": MOOT — the
  whole card was dropped per F7 (below) and replaced by the Congo card.
  No "Houthis" headline remains on the page.
- F4 Card #12 ANTALYA headline: "COP31 talks left adrift" → "COP31
  aftermath: what's next?" — the red-team's full wording ("COP31 aftermath:
  diplomats ask what's next") is 3 lines at capH 12.5 (width-checked), so
  the shorter form is used; it matches the body ("Diplomats ask what's
  next. (Korea Times)") and makes the Monday-aftermath framing explicit.
- F5 DATE CHECK item 3: "India 720 Sun" → "India 720/9 Sun" — the "/9"
  marks it as the declared Sunday innings total, distinct from hero 2's
  Monday "239/5". Still 3 lines (width-checked + render: no WARN).

## F6–F11 (REDTEAM-HYDROGEN-LOG.md, gemini-4-hydrogen) — applied / decided
- F6 Card #10 ITANAGAR headline: "Amit Shah launches Rs 4,000-crore" →
  "Amit Shah launches projects" — the red-team's wording ("...Rs 4,000-crore
  projects") is 3 lines at capH 12.5 (width-checked), so the complete phrase
  "Amit Shah launches projects" is used; the Rs 4,000-crore figure stays in
  the body ("Projects worth Rs 4,000 crore. (IANS)"). 2 lines, no truncation.
- F7 Card #9 RIYADH date — MOST IMPORTANT: DROPPED the card. Re-verified
  first-hand: Reuters 22 Nov ("Yemen's Houthis said on Sunday they had
  carried out an operation targeting Saudi Arabia's Rabigh oil refinery",
  https://www.reuters.com/world/middle-east/yemens-houthis-say-they-attacked-saudi-rabigh-oil-refinery-2026-11-22/);
  IANS Nov 23 dateline ("on Sunday said the first operation targeted the
  Rabigh oil refinery"); China Daily Asia ("said Sunday"); AnewZ ("said on
  Sunday (22 November)"). The Indian Express live blog (the builder's
  source) is a Monday re-report of a Sunday claim — no Monday angle exists
  (no new Saudi response or new claim Monday), so the card was dropped,
  not reworded. Replaced by a verified Monday story: Card #9 CONGO
  (headline "Congo halts cobalt exports again", body "Exports halted from
  Nov 30. (Reuters)", Reuters 23 Nov, opened first-hand; regulator ARECOMS
  said Monday; second halt since April 2025). Map pin 9 moved Riyadh →
  Kinshasa (15.3, -4.3); place "CONGO" (not "KINSHASA") so the kicker keeps
  its number ("9. CONGO · CONFIRMED" fits; "9. KINSHASA · CONFIRMED" does
  not). Regions: AFRICA 1→2, MIDEAST 2→1. DATE CHECK: "Rabigh claim Sun"
  ADDED (the near-miss is now listed as excluded); "India–Bulgaria Sat"
  dropped to keep the box at 3 lines. "Houthi strikes Fri" KEPT — different
  event (Fri 20 Nov intercepts), as instructed.
- F8 Brief #17 MANCHESTER: "Pochettino questions Yoro red after 4-0 loss.
  (India Today)" → "Pochettino questions Yoro red card. (India Today)" —
  the "4-0 loss" (Sunday's scoreline) is dropped, removing the second 4-0
  on the page (DATE CHECK keeps "Liverpool 4-0 Sun"). "On Monday" was NOT
  added: Pochettino's quotes were Sunday post-match (Reuters 22 Nov); the
  brief is a Monday India Today report, same aftermath pattern as cards
  5/13 — claiming Monday for the quote itself would be shaky.
- F9 Card #13 SEATTLE: NOT changed — the Monday-ness (The Hindu's Monday
  report of the lawyer's Sunday statement) cannot be made explicit without
  a false day claim; accepted documented confusion risk (same as hydrogen's
  downgrade). Body unchanged.
- F10 DATE CHECK "Dems 258 Sun" → "Dems win House Sun" — the bare seat
  figure is gone. Still 3 lines.
- F11 headline/body disconnects (cards 6/7/8/13): fixed 6, 7, 8.
  - Card #6: "Private sector shrinks fastest" → "Private sector hits
    5-year low" (matches body "PMI 46.1, lowest since Aug 2021").
  - Card #7: "Gold climbs, oil slips in thin trade" → "Asian markets slide
    in thin trade" (matches body "Japan shut; Kospi -2.8%").
  - Card #8 body: "Destroyed by 2019 fire. (Nikkei)" → "Reopens with fire
    safeguards. (Nikkei)" (the reopening itself is now in the body).
  - Card #13 body: NOT changed — adding "Detained at Sea-Tac on Saturday"
    would put a Saturday fact in a Monday card next to DATE CHECK's
    "Sea-Tac Sat" (confusion); headline already says "Detained".

## Other red-team nits applied
- N4 Card #5 DYMER body: "Toll up to 7 after Sunday. (Reuters)" → "Toll
  up to 7 on Monday. (Reuters)".
- N6 Brief #18 MUMBAI: "this week" dropped ("Tata Sons gears up for a
  go-public decision. (TOI)").
- N7 Brief #14 source: "(Stats NZ)" → "(StatsNZ)" (reads as "State NZ"
  at judge resolution).
- N8 Hero #1 headline: "Modi, Shah hold talks in New Delhi" → "Modi,
  Nepal PM hold talks in New Delhi" (2 lines, width-checked); scene
  caption "MODI · SHAH" → "MODI · BALEN SHAH" (hydrogen's extra ambiguity
  source). Kicker already said "Nepal's Shah".
- N9 Hero #3 headline: "UN urges probe into Benghazi attacks" → "UN urges
  probe into Benghazi attack" (singular — one corvette + one merchant ship;
  body names the single corvette).
- N3 Card #10 kicker still numberless ("ITANAGAR · CONFIRMED") — documented
  pre-work deviation, unchanged (does not fit 188px with the number).
- E1–E3 / E-H1 NOT "fixed" (correct as-is): Balen Shah IS PM of Nepal
  (sworn in 27 Mar 2026); NZ–India Test and UN drone-boat report verified
  in RESEARCH.md.

## W6 — cricket final + score labelling (evening refresh)
- HERO 2 (final result, verified first-hand ×3: ICC article published
  2026-11-23T08:39:17Z, ESPNcricinfo match report, AAP): the Wellington
  Test was DRAWN. NZ 239/5 (120 overs), Mitchell 49*, Phillips 26*;
  India 720/9 dec, NZ 368. Headline "India six wickets from a win in
  Wellington" → "New Zealand hold India to a draw". Body "New Zealand 157
  for 4 at lunch on the final day, still 195 behind." → "New Zealand 239
  for 5 at the close. Mitchell 49 not out. Draw." Scene score "157/4" →
  "239/5", subline "SIX WICKETS TO GET" → "FINAL — DRAW" (labelled, never
  a bare score). STATS #1 "157-4 / New Zealand at lunch, day 5" → "239-5 /
  New Zealand, drawn Test". Kicker "India six wickets from victory" →
  "Wellington Test drawn". All other stats already carry labels (PMI, Q3,
  toll, gold, futures).
- HERO 3 body updated to the day's development (verified first-hand: AP
  summary 23 Nov 05:18 EST; UN News 23 Nov; Xinhua 23 Nov): "UN mission
  calls for an independent inquiry after drone boats hit a ship off
  Benghazi." → "Zelenskyy says Ukraine's sea drones hit a Russian corvette.
  (AP)" — Zelenskyy said Monday Ukrainian forces used seven sea drones to
  strike the corvette Merkury (sank, per his claim; body says "hit", the
  conservative wording). Hero source changed Arab News → AP so the kicker
  matches the body's source (headline's UN-probe fact was reported Monday
  by UN News / Arab News / Xinhua). Scene caption "DRONE BOATS OFF
  BENGHAZI" unchanged.

## Evening refresh — late-day stories (all verified 23 Nov, first-hand)
- Card #9 RIYADH → CONGO (see F7 above). Reuters, opened first-hand.
- Brief #15 TOKYO Sanrio → BERLIN "German growth fastest since Mar 2022.
  (Reuters)" (Reuters 23 Nov: flash composite PMI 55.0, highest since
  March 2022). EUROPE 8→9, ASIA 14→13.
- Brief #29 SYDNEY ASX → WASHINGTON "Democrats plan 12 debates for 2028
  primary. (AP)" (AP 23 Nov: DNC announcement Monday, first debate June).
  AMERICAS 3→4, OCEANIA 5→4.
- Brief #30 NEW DELHI MoUs (duplicates hero 1) → DHAKA "First measles-free
  day in eight months; toll 1,352. (TBS News)" (TBS News 23 Nov 15:45+06,
  opened first-hand: no measles deaths in the 24h to 8am Mon 23 Nov, first
  such day in 8+ months; cumulative toll 1,352). ASIA unchanged.
- Card #11 Brentford v Everton: UNCHANGED (fixture wording kept) — kickoff
  20:00 UTC (03:00 WIB 24 Nov), result not in at build time (~21:00 WIB).
- Totals: still 33 stories (3 heroes + 10 cards + 20 briefs). Regions:
  ASIA 13, AFRICA 2, EUROPE 9, MIDEAST 1, OCEANIA 4, AMERICAS 4 (= 33).
- No other story replaced: all other morning items re-checked against the
  day's wires and still stand as Monday 23 Nov.

## Renderer change (cycle 39 C2c)
- main() now empties the output dir's CONTENTS via readdirSync + rmSync
  before writing (canonical pattern; never removes the dir itself — it is
  a grader mount point). No output change: renders are byte-identical
  apart from the content edits. Node 22 stdlib-only, deterministic, no
  network at grading — unchanged.

## P9 (tie-break: smaller file wins on an exact judge tie)
- encodePNG already uses deflateSync level 9 (maximum zlib compression).
  No pixel or legibility change. Final file 95,341 bytes (down from
  96,268 pre-work; the drop is from shorter text, not from a compression
  change — level 9 was already in use). 300px legibility re-checked
  (see below).

## Render + checks
- Re-render: 2 runs, byte-identical, NO WARN (no TRUNCATED lines).
  - md5: `cedec2d34e28a39dba280e34c5eb1e04` (both out1 + out2)
  - sha256: `88ff4db37fcdc49d7657d67bcd4ccac8e626851d650607e2f610fbf1ee7c3f2f`
  - 95,341 bytes, 1024x1024.
- Pre-edit verification render (for the record): md5
  `ebdfc3b7ff5c43dfc7ed158e3b7303b8`, 96,268 bytes — superseded.
- Visual check (full 768px judge view + 2x crops of heroes, cards, DATE
  CHECK): masthead date, kicker, stat numbers, hero headlines, region
  strip all legible; all card headlines/bodies 2 lines, no truncation;
  DATE CHECK 3 lines, all 15 items present; card 9 kicker keeps its
  number ("9. CONGO · CONFIRMED"); hero 2 scene reads "239/5 FINAL —
  DRAW". Known font defect unchanged: lowercase 's' still renders close
  to 'c' at small sizes (wording mitigations only — F3/F6/N7 applied).
- 300px legibility: date, kicker, hero headlines, stat numbers
  (239-5, 46.1, +2.2%, 7, $3,577, +2.8%) all read correctly; digit gate
  passes (preview300.png in out1/, gitignored).
- `makefun check`: (result recorded below after commit — see "Checks").
- cycle39-pre-submit-check.sh C1–C9: (result recorded below after commit).

## Checks
- `makefun check` (kit CLI, --repo . --commit 5995ed6, no transcripts):
  4 passed, 1 failed, 14 skipped, 5 at-submission. The 1 failure is
  transcripts_present — EXPECTED (no bundle supplied; the main agent
  bundles at submit in the 24 Nov 07:00 wave). Same result as the morning
  draft's check. Note in the output: this kit copy is level 36, the site
  is at level 38 (informational; no action taken — downloading a newer kit
  was not part of this task).
- cycle39-pre-submit-check.sh C1–C9: ALL MECHANICAL CHECKS PASS (C1, C1b,
  C2, C2b, C2c, C3, C5, C6, C9; C4/C7 skipped — not meme-x / no bundle).
  C8: PNG age ~0.1h (fresh). C6 manual digit check done on the 300px
  preview (all stat numbers read correctly).

## Push
- Base remote HEAD (verified first-hand): 9f5e7cbc3e589df2e9c768187e998ec121ee96a3
- New remote HEAD: d3040980bd9b27dc0dbaf14697a340899632cbba (local 5995ed6;
  tree verified equal by push_gitdata.py; re-verified first-hand via
  gh_api.py). Record commit (this file + PROGRESS.md with the push hash)
  pushed after as: (see PROGRESS.md)
- DO NOT SUBMIT — main agent bundles + submits in the 24 Nov 07:00 WIB wave.
