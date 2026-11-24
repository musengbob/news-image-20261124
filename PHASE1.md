# PHASE 1 — news-image-20261124

## Summary
- 36 stories, all researched 24 Nov 2026 (07:25–07:55 WIB) and dated
  Tuesday 24 November 2026: 3 heroes + 9 briefs + 24 numbered.
- Heroes: Nvidia reinstates Jensen Huang, shares +31% (Reuters/CNN);
  Ukraine sinks a Russian warship in Libya (BBC/Reuters); Indonesia
  factory-fire search goes on, 24 dead, ~30 missing (Studmentor).
- Playbook reproduced from 20261123 (blind round 1 rank 89/7226): dense
  front page + world map, masthead "THE WORLD TODAY", dateline Tuesday
  24 November 2026. `compose.py` written fresh in this session (same
  layout, new chip + ship + fire hero art, new stories, stats, markers,
  date check).
- No 20261123 stories or pixels reused; entry.png drawn fresh by compose.py.

## Files (~/workspace/makefun/entries/news-image-20261124/)
- STORIES.md — 36 stories with source + date each, plus DATE CHECK section
- compose.py — PIL renderer (deterministic)
- entry.png — 1024×1024, 159,434 bytes (≤1 MiB), sha256
  4cfe4315daae4783daa645e6f86f158fe74b5326b862a07edde2d69b10dfe44a
- main.ts — Node 22 stdlib only, copies entry.png to $MAKEFUN_OUTPUT_DIR
- README.md — badges + run instructions (Phase 2)

## Verification
- `python3 compose.py` → final y = 1015 (canvas 1024), no assertion
  failures (all 24 numbered headlines fit one line).
- Viewed entry.png at full size: masthead, ticker, stat strip, 3 heroes,
  9 briefs, world map with 12 red markers, DATE CHECK box, 24 numbered
  items, footer all legible; no overlapping or garbled text.
- Defect found and fixed: hero decks H1 and H2 were cut mid-sentence at
  the 3-line cap ("Trump says: "I made" / "burns in the"). Both decks
  shortened and re-measured to exactly 3 lines; re-rendered and re-checked
  the hero crop — both decks now end cleanly.
- Viewed downscaled to 300px: masthead, heroes and map still read;
  numbered list is small (same as the 20261121/22/23 playbook).
- `mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts` → out/entry.png
  byte-identical to entry.png (sha256 match). Only a harmless Node
  MODULE_TYPELESS_PACKAGE_JSON warning (same as the 20261122/23 pattern).

## Notes / needs fixing
- Dating caveat documented in STORIES.md: several items are Tuesday
  developments of Monday events (Huang reinstatement, Libya strike,
  factory search, Wellington draw); the DATE CHECK box names the earlier
  events they follow. Two near-misses caught during research and left out:
  the Korea KADIZ jet scramble was 17 Nov (not 24 Nov, despite the
  Reuters 24 Nov summary repeating it) and the Alcaraz ATP Finals win
  was Sun 22 Nov.
- Phase 2 still to do: GitHub repo, badges/About, bundle, submit.
  (Not touched here per the task.)
