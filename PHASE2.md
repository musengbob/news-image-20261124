# PHASE 2 — repo + GitHub About (news-image-20261124)

## Repo

- URL: https://github.com/musengbob/news-image-20261124
- Created: 2026-11-24 ~00:28 WIB (after the competition opened 2026-11-24T00:00:00Z)
- Visibility: public, default branch `main`

## Commit

- Full sha: `143aceaaff2f56c42c7e9d29717e0e6cc92a8c5a`
- Pushed: 2026-11-23T17:28Z
- Files in first commit: STORIES.md, compose.py, entry.png, main.ts,
  README.md, PHASE1.md, LICENSE (MIT), .makefun/owner.json
- `.makefun/owner.json` contents: `{"wallet": "GsoqAXMhgx1jfqQPSKevY5EST7uNikMBd5gTWVFUTwYG"}`

## README

- 3 live make.fun badges at the top (bounty, rank, reward) + bounty link
  https://make.fun/bounty/news-image-20261124, same pattern as 20261123.
- Badge liveness verified 2026-11-24 00:29 WIB (all HTTP 200 image/svg+xml):
  - https://make.fun/badge/news-image-20261124.svg
  - https://make.fun/badge/news-image-20261124/musengbob/news-image-20261124/rank.svg
  - https://make.fun/badge/news-image-20261124/musengbob/news-image-20261124/reward.svg
- Bounty page https://make.fun/bounty/news-image-20261124 — HTTP 200.
- README raw on GitHub — HTTP 200.

## GitHub About — verified via `gh repo view ... --json description,homepageUrl,repositoryTopics,url`

- description: "THE WORLD TODAY — sum up 24 November 2026's world news in one image. Built by an AI agent for make.fun's "Sum up 24 November's world news in one image" bounty, $100 in USDC."
- homepage: https://make.fun/bounty/news-image-20261124
- topics: ai-agents, bounties, growth, makefun
- url: https://github.com/musengbob/news-image-20261124

## Clone test (reproduction)

- Cloned https://github.com/musengbob/news-image-20261124.git to a temp dir
  outside the entry dir, ran `mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts`.
- Result: PASS — `out/entry.png` sha256
  `4cfe4315daae4783daa645e6f86f158fe74b5326b862a07edde2d69b10dfe44a`,
  byte-identical to the repo `entry.png` (159,434 bytes) and to the Phase 1 hash.
- Clone HEAD: `143aceaaff2f56c42c7e9d29717e0e6cc92a8c5a` (matches pushed commit).
- Temp clone dir removed after the test.

## Notes

- Phase 1 files untouched: entry.png, compose.py, STORIES.md, main.ts not
  modified after the hero-deck fix. Only README.md (badges + footer link),
  LICENSE, and .makefun/owner.json were added.
- No bundling, no submit, no make.fun API touched in this phase (no API key
  read, no credential file opened).
- No blockers. Ready for the coordinator to bundle + submit before the
  round 1 cutoff 2026-11-24T12:00:00Z (19:00 WIB).
