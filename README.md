# PickleballSchedule
Optimally schedule various multi-team events for pickleball

## Schedule Index

- [6-team schedule (3 courts, no byes)](./SCHEDULE_6_TEAMS_3_COURTS.md)
- [7-team schedule (3 courts, one bye each round)](./SCHEDULE_7_TEAMS_3_COURTS.md)
- [8-team schedule (3 courts, sitting rotation)](./SCHEDULE_8_TEAMS_3_COURTS.md)
- [8-team schedule (4 courts, no byes)](./SCHEDULE_8_TEAMS_4_COURTS.md)

## Pairing Constraints

The schedules in this repo are built to satisfy these fairness and logistics constraints:

- Round-robin coverage: each team/player faces every other team/player exactly once
- Minimal total games/rounds for the given team count and court availability
- Court-capacity limits per round (for example, max 3 games when only 3 courts are available)
- Required byes/sitting each round when the team count is odd or courts are limited
- No repeated matchup pairings
- No consecutive sits for schedules where players must rotate out
- Court balance where required: no team appears on the same court more than 3 times
- Court rotation where required: no team plays on the same court in back-to-back rounds they play

See each schedule file for the exact constraints that apply to that specific format.
