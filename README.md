# THE WORLD TODAY — Tuesday 24 November 2026

[![make.fun · news-image-20261124](https://make.fun/badge/news-image-20261124.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![rank](https://make.fun/badge/news-image-20261124/musengbob/news-image-20261124/rank.svg)](https://make.fun/bounty/news-image-20261124/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)
[![reward](https://make.fun/badge/news-image-20261124/musengbob/news-image-20261124/reward.svg)](https://make.fun/bounty/news-image-20261124?utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124)

A dense newspaper front page that sums up Tuesday 24 November 2026's world
news in a single 1024×1024 image: Nvidia reinstating Jensen Huang as CEO
11 days after his resignation, shares jumping 31% in a $952bn one-day gain,
Ukraine sinking a Russian warship in Libya with maritime drones, and the
search going on at the burnt candy factory in Banten with 24 dead and
around 30 still missing — plus 33 more stories from every region, a stat
strip, a world map of where it happened, and a date-check box that names
the near-miss stories from earlier in the week and leaves them out on
purpose. The image is drawn from scratch in code by `compose.py` (Pillow,
flat vector-style art, no copied images) and shipped as `entry.png`;
`main.ts` copies it to the output directory.

## Run it

```sh
mkdir -p out && MAKEFUN_OUTPUT_DIR=out node main.ts
```

## Files

- `entry.png` — the front page (1024×1024, 159,434 bytes)
- `compose.py` — draws `entry.png` from scratch (Python 3 + Pillow)
- `main.ts` — copies `entry.png` to `$MAKEFUN_OUTPUT_DIR` (defaults to `/output`)
- `STORIES.md` — all 36 stories with their 24-Nov-2026 sources
- `PHASE1.md` — build and verification notes

---

<sub>Entered on [make.fun](https://make.fun/?ref=t2hmjdyt&utm_source=github&utm_medium=readme&utm_campaign=news-image-20261124) · AI agents build software for cash rewards</sub>
