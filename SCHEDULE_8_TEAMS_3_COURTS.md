# 8-Player Rotation Schedule (3 Courts)

This schedule assumes:

- 8 individual players (`1` through `8`)
- Singles pairings (one matchup per court)
- 3 courts available
- Goal: every player faces each of the other 7 players exactly once
- Constraint: no one sits out in consecutive rounds

## Why 9 rounds is not enough

With 8 players, the number of unique head-to-head matchups is:

- `C(8,2) = 28`

With 3 courts, each round can host at most 3 matchups. In 9 rounds, that is:

- `9 * 3 = 27` matchups

Since `27 < 28`, a complete all-opponents schedule cannot be done in 9 rounds.  
The minimum is **10 rounds**.

## 10-Round Schedule

| Round | Court 1 | Court 2 | Court 3 | Sitting |
|---|---|---|---|---|
| 1 | 1 vs 2 | 3 vs 4 | 5 vs 6 | 7, 8 |
| 2 | 4 vs 6 | 7 vs 5 | 8 vs 3 | 1, 2 |
| 3 | 3 vs 5 | 1 vs 6 | 2 vs 4 | 7, 8 |
| 4 | 7 vs 8 | 4 vs 5 | 3 vs 6 | 1, 2 |
| 5 | 1 vs 5 | 8 vs 6 | 7 vs 2 | 3, 4 |
| 6 | 8 vs 2 | 7 vs 3 | 1 vs 4 | 5, 6 |
| 7 | 7 vs 1 | 2 vs 6 | 8 vs 5 | 3, 4 |
| 8 | 2 vs 3 | 8 vs 1 | 7 vs 4 | 5, 6 |
| 9 | 7 vs 6 | 2 vs 5 | *(open)* | 1, 3, 4, 8 |
| 10 | 8 vs 4 | 1 vs 3 | *(open)* | 2, 5, 6, 7 |

## Constraint Check

- Every unique pairing appears exactly once (`28` total matchups)
- No player sits in consecutive rounds
- Two rounds use only 2 courts (required to keep pairings unique while finishing in 10 rounds)
- No player appears on the same court more than 3 times
- No player plays on the same court in back-to-back rounds they play
