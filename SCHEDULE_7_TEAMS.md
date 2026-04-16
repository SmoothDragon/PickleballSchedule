# 7-Team Schedule (One Team Sits Each Round)

This schedule assumes:

- 7 teams (`1` through `7`)
- Head-to-head games
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
| 1 | 1 vs 6 | 2 vs 5 | 3 vs 4 | 7 |
| 2 | 2 vs 3 | 1 vs 4 | 7 vs 6 | 5 |
| 3 | 6 vs 4 | 7 vs 5 | 1 vs 2 | 3 |
| 4 | 5 vs 3 | 6 vs 2 | 7 vs 4 | 1 |
| 5 | 4 vs 2 | 7 vs 3 | 5 vs 1 | 6 |
| 6 | 3 vs 1 | 5 vs 6 | 7 vs 2 | 4 |
| 7 | 4 vs 5 | 7 vs 1 | 3 vs 6 | 2 |

## Check

- Every team has exactly one bye
- No matchup is repeated
- Every team plays the other 6 teams exactly once
- No team appears on the same court more than 3 times
- No team plays on the same court in back-to-back rounds they play
