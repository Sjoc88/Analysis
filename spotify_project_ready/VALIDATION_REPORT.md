# Spotify validation — first pass (corrected)

## Overall
- JSON files: 11
- Total events: 62,581
- Date range: 2020-12 → 2026-09
- Months represented: 59
- Total listening time: 2,770.8 hours
- Mean monthly listening: 47.0 hours
- Median monthly listening: 41.3 hours
- Peak month: 2021-02 (102.8 hours)
- Lowest month: 2025-08 (0.0 hours)

## Data quality
- Events without track/episode content: 0
- Missing duration: 0
- Negative duration: 0
- Zero-duration events: 721
- Events under 10 seconds: 8,566
- Track events without Spotify URI: 0

## Duplicates
- Exact duplicate observations: 134
- Core-event duplicate observations: 152
- Duplicates are preserved for now.

## Important note
The first monthly diagnostic had a SQL grouping bug: `GROUP BY month` resolved to the stored numeric `month` column instead of the calculated year-month label. The database itself was unaffected. This report and chart use the corrected grouping expression.
