# tiny-chess-2

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/m1651/makefun-tiny-chess-2/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/m1651/makefun-tiny-chess-2/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A second attempt at the strongest chess engine in 4 KB of Python, rebuilt
from scratch with a different design: 0x88 board, negamax alpha-beta with
iterative deepening to a fixed node budget, quiescence over captures and
check evasions, transposition table, MVV-LVA + killer move ordering,
null-move pruning, and an evaluation with piece-square tables, bishop pair,
king shelter and an endgame king table. No clock, no randomness: the same
position always gets the same move, so replays match.

`engine.py` is the readable source; `main.py` is the same source packed
with the kit's `compress` command.
