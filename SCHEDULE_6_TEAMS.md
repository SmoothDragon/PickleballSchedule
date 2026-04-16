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

## Schedule A: Prioritizes Court Rotation

Constraints satisfied:

- No team plays on the same court in back-to-back rounds
- No team appears on the same court more than 3 times
- Full round robin with no repeated matchups

| Round | Court 1 | Court 2 | Court 3 |
|---|---|---|---|
| 1 | 1 vs 2 | 3 vs 4 | 5 vs 6 |
| 2 | 5 vs 3 | 1 vs 6 | 2 vs 4 |
| 3 | 1 vs 4 | 2 vs 5 | 6 vs 3 |
| 4 | 6 vs 2 | 1 vs 3 | 4 vs 5 |
| 5 | 1 vs 5 | 4 vs 6 | 3 vs 2 |

## Schedule B: Prioritizes Max 2 Per Court

Constraints satisfied:

- No team appears on the same court more than 2 times
- Full round robin with no repeated matchups

| Round | Court 1 | Court 2 | Court 3 |
|---|---|---|---|
| 1 | 1 vs 2 | 3 vs 4 | 5 vs 6 |
| 2 | 1 vs 6 | 5 vs 3 | 2 vs 4 |
| 3 | 6 vs 3 | 1 vs 4 | 2 vs 5 |
| 4 | 4 vs 5 | 6 vs 2 | 1 vs 3 |
| 5 | 3 vs 2 | 1 vs 5 | 4 vs 6 |

## Notes

- No team sits out in either schedule
- Both schedules are complete round robins (15 unique matchups)
- These two strict constraints cannot both be satisfied simultaneously for 6 teams:
  - max 2 appearances per team on any single court
  - no same-court appearances in back-to-back rounds
- An exhaustive search over court assignments (including round reordering) found no schedule that satisfies both at once.

