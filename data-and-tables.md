# Data & Tables

## Clarity & Visual Consistency

- **Minimize Information Fatigue:** Reduce visual noise and maximize information clarity.
- **Avoid Duplicate Metrics Across Views:** Consolidate overlapping visualizations and inspector HUDs into their primary view to reduce cognitive load and maintenance overhead.
- **Single Source of Truth for Summary Badges:** Summary counters (such as rising/falling counts) must derive from the exact same active display mode, dataset, and threshold buckets as the main visualization.

## Numeric & Financial Formatting

- **Tabular Numerals:** Use fixed-width numerals (`tabular-nums` / monospace) for live-updating prices, rates, and vertically aligned numeric columns to prevent layout jitter.
- **Distinguish Missing/Unsupported Data from Zero:** Never coerce `null`, `NaN`, or unsupported metrics into `0`; render them distinctly (e.g., `N/A` or neutral inactive styling) so they are not mistaken for flat or zero-change values.

## Table Layout & Sorting

- **Contain Content Within Boundaries:** Ensure that elements within grids and tables never overflow or extend beyond their container boundaries.
- **Missing/NaN Values at the End on Ascending Sort:** When sorting numerical data in a table in ascending order, intentionally place rows with missing values or `NaN` data at the very end.
