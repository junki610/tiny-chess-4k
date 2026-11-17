# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/junki610/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/junki610/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine squeezed into 4,077 bytes of Python (lzma + base85 packed): negamax alpha-beta with a transposition table, PVS, LMR, null-move pruning, check extensions and quiescence search; piece-square-table evaluation with bishop pair, endgame king table and passed-pawn bonuses. Fixed 50,000-node search, fully deterministic.

## Run it

```sh
MAKEFUN_ENV_URL=<make.fun game server URL> python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=mctnptqw&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
