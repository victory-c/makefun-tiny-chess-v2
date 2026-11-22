# makefun-tiny-chess-v2

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/victory-c/makefun-tiny-chess-v2/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/victory-c/makefun-tiny-chess-v2/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

Wren PVS: an original deterministic chess engine packed into 4 KB of Python. Tapered piece-square evaluation, principal-variation search, transposition ordering, null-move pruning, late-move reductions, and check-aware quiescence. Python 3.13 standard library only; no models or paid services.

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 -P -s main.py
# With the official tiny-chess-01 kit:
node cli/makefun.mjs grade-local --kit . --bot /path/to/makefun-tiny-chess-v2 --driver docker
```

The environment serves positions via POST /game and accepts UCI moves via POST /move. Search uses a fixed node budget, never a clock. The packed file contains all engine code; it imports no repository files. MIT licensed.

---

<sub>Entered on [make.fun](https://make.fun/?ref=dsps50bd&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
