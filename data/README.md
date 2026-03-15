# Dataset Information

The datasets used in this project were derived from publicly available cricket match data sources.

Primary sources include:

- Cricsheet ball-by-ball datasets
- ESPN Cricinfo scorecards

Due to repository size limits and licensing considerations, the full datasets are not included in this repository.

## Data Structure

Typical dataset fields include:

- match_id
- over
- ball
- striker
- bowler
- runs_off_bat
- extras
- wicket_type
- fielders_involved

These fields are used to compute context-aware performance metrics such as:

- Phase Weighted Runs
- Boundary Impact Score
- Dot Ball Cost
- Wicket Impact Score
