# 8-Team Schedule (4 Courts, No One Sits)

This schedule assumes:

- 8 teams (`1` through `8`)
- Head-to-head games
- 4 courts
- No byes (all teams play every round)
- Goal: each team plays every other team exactly once

## Minimum Number of Games

For 8 teams, unique matchups are:

- `C(8,2) = 28`

Each round can host 4 games (all 8 teams playing), so:

- `28 / 4 = 7` rounds

So the minimum and exact total is **28 games across 7 rounds**.

## Round-by-Round Pairings

| Round | Court 1 | Court 2 | Court 3 | Court 4 |
|---|---|---|---|---|
| 1 | 1 vs 2 | 3 vs 4 | 5 vs 6 | 7 vs 8 |
| 2 | 5 vs 7 | 6 vs 8 | 1 vs 3 | 2 vs 4 |
| 3 | 1 vs 4 | 2 vs 3 | 5 vs 8 | 6 vs 7 |
| 4 | 2 vs 6 | 4 vs 8 | 3 vs 7 | 1 vs 5 |
| 5 | 3 vs 5 | 1 vs 7 | 4 vs 6 | 2 vs 8 |
| 6 | 4 vs 7 | 2 vs 5 | 1 vs 8 | 3 vs 6 |
| 7 | 3 vs 8 | 1 vs 6 | 2 vs 7 | 4 vs 5 |

## Check

- No team sits out
- No matchup is repeated
- Every team plays the other 7 teams exactly once
- No team appears on the same court more than 2 times
- No team plays on the same court in back-to-back rounds
