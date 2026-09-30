# Week 6 · Data Transformation and Feature Engineering

Three ways to change a table, and the problem each one solves.

## Files

| File | What it is |
|---|---|
| [`week06_reshaping_slides.pdf`](week06_reshaping_slides.pdf) | Lecture slides: reshaping, feature engineering, transformations |
| [`week06_flights_wide_long.ipynb`](week06_flights_wide_long.ipynb) | Long vs. wide with seaborn's `flights` dataset (`pivot_table`) |

## Topics

- **Reshape:** wide vs. long (tidy) data; `pivot`, `pivot_table`, `melt`
- **Engineer features:** ratios, dates, bins, encodings, group summaries; avoiding leakage
- **Transform:** min–max, z-score, robust scaling, log

| Job | The problem it solves |
|---|---|
| Reshape | Your tool cannot work with the layout you were given. |
| Engineer features | The answer is in your data, but not in any column. |
| Transform | The numbers are on a scale that makes your method lie. |
