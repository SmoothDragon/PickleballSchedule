# 6-Team Schedule (No One Sits)

This schedule assumes:

- 6 teams (`1` through `6`)
- Head-to-head games
- No byes (all teams play every round)
- Goal: each team plays every other team exactly once

## Minimum Number of Games

For 6 teams, unique matchups are:

- `C(6,2) = 15`

Each round can host 3 games (all 6 teams playing), so:

- `15 / 3 = 5` rounds

So the minimum and exact total is **15 games across 5 rounds**.

## Round-by-Round Pairings

| Round | Court 1 | Court 2 | Court 3 |
|---|---|---|---|
| 1 | 1 vs 6 | 2 vs 5 | 3 vs 4 |
| 2 | 2 vs 3 | 6 vs 4 | 1 vs 5 |
| 3 | 1 vs 4 | 5 vs 3 | 6 vs 2 |
| 4 | 5 vs 6 | 4 vs 2 | 1 vs 3 |
| 5 | 1 vs 2 | 3 vs 6 | 4 vs 5 |

## Check

- No team sits out
- No matchup is repeated
- Every team plays the other 5 teams exactly once
- No team appears on the same court more than 3 times
- No team plays on the same court in back-to-back rounds
