# tiny-chess-01

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/sherrypubg128-blip/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/sherrypubg128-blip/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

The strongest chess engine in 4 KB of Python (stdlib only): a 0x88 board
with negamax alpha-beta search on a fixed 50,000-node budget, a
transposition table, quiescence search, MVV-LVA plus killer move ordering,
null-move pruning and late-move reductions, and a tapered piece-square-table
evaluation with bishop pair. It speaks the make.fun env protocol
(`POST /game`, `POST /move`) and is fully deterministic: no wall clock and
no unseeded randomness anywhere, so the same position always yields the
same move.

## Run it

```sh
MAKEFUN_ENV_URL=http://127.0.0.1:PORT python3 main.py
```
