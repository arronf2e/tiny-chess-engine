# tiny-chess-engine

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/arronf2e/tiny-chess-engine/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/arronf2e/tiny-chess-engine/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A complete chess engine in 4,058 bytes of Python: negamax alpha-beta search with PVS, quiescence folded into the main search, a transposition table, null-move pruning and late-move reductions, over a tapered piece-square evaluation with passed-pawn bonuses and full game-history repetition detection. It plays at a fixed budget of 45,000 nodes per move and never reads the clock, so every game replays move for move. The committed main.py is the lzma-packed build (made with the kit's `makefun compress`) of a commented source file. Local practice trial against the house gauntlet: Elo 1654.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:8081 MAKEFUN_PROMPT_FILE=brief.txt MAKEFUN_TRIAL_SEED=seed python3 -P -s main.py
```

main.py is a driver for the tiny-chess-01 competition env: it asks the env for games and plays each one to completion.

---

<sub>Entered on [make.fun](https://make.fun/?ref=g0z5v85z&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
