# tiny-chess-4k

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/junki610/tiny-chess-4k/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/junki610/tiny-chess-4k/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A chess engine squeezed into 3,317 bytes of Python (packed with makefun compress): negamax alpha-beta with a transposition table, PVS, LMR, null-move pruning, check extensions and quiescence search; piece-square-table evaluation with bishop pair, endgame king table and passed-pawn bonuses. Fixed 50,000-node search, fully deterministic.

## Design notes

- 0x88-style 128-square board with pseudo-legal move generation and in-loop king-safety filtering.
- Evaluation is precomputed into per-piece 128-entry tables; the endgame switches the king to a centralisation table and adds passed-pawn bonuses.
- The search never reads a clock: it stops on a fixed node budget, so every game replays move-for-move.

## Run it

```sh
MAKEFUN_ENV_URL=<make.fun game server URL> python3 main.py
```

---

<sub>Entered on [make.fun](https://make.fun/?ref=mctnptqw&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
