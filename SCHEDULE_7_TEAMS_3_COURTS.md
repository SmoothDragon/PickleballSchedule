# 7-Team Schedule (3 Courts, One Team Sits Each Round)

This schedule assumes:

- 7 teams (`1` through `7`)
- Head-to-head games
- 3 courts
- Exactly one team has a bye each round
- Goal: each team plays every other team exactly once

## Minimum Number of Games

For 7 teams, unique matchups are:

- `C(7,2) = 21`

Each round has 3 games (6 teams playing) and 1 bye, so in 7 rounds:

- `7 * 3 = 21` games

So the minimum and exact total is **21 games across 7 rounds**.

## Round-by-Round Pairings

| Round | Court 1 | Court 2 | Court 3 | Bye |
|---|---|---|---|---|
| 1 | 1 vs 2 | 3 vs 4 | 5 vs 6 | 7 |
| 2 | 5 vs 3 | 7 vs 2 | 1 vs 4 | 6 |
| 3 | 2 vs 4 | 1 vs 5 | 7 vs 6 | 3 |
| 4 | 6 vs 3 | 7 vs 4 | 2 vs 5 | 1 |
| 5 | 4 vs 5 | 6 vs 1 | 7 vs 3 | 2 |
| 6 | 3 vs 1 | 7 vs 5 | 6 vs 2 | 4 |
| 7 | 4 vs 6 | 3 vs 2 | 7 vs 1 | 5 |

## Check

- Every team has exactly one bye
- No matchup is repeated
- Every team plays the other 6 teams exactly once
- No team appears on the same court more than 3 times
- No team plays on the same court in back-to-back rounds they play
