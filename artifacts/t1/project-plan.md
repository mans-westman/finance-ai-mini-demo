# T1 Project Plan

## Project Goal

Develop a clear and reproducible research workflow for comparing three familiar asset classes: SPY (US equities), TLT (long-term US Treasury bonds), and GLD (gold). The project starts with a written plan here and continues with the same repository in later tutorials to design a bounded analysis task and organize a verifiable agent workflow.

## Available Data

The only input is `data/etf_snapshot.csv`, one row per ETF, described in `data/data_dictionary.md`:

- `ticker` and `asset_class`: identity of each illustrative ETF
- `expected_return_pct`: illustrative annual return assumption (percent per year)
- `volatility_pct`: illustrative annual variability assumption (percent per year)
- `max_drawdown_pct`: illustrative largest peak-to-trough loss (percent; negative values represent losses)
- `expense_ratio_pct`: illustrative annual fund fee (percent per year)

All values are synthetic teaching data, not live or historical market observations, and must not be used as investment advice. The dataset is deliberately small and fixed, so no download or data-cleaning step is required during the tutorials.

## Expected Final Deliverable

The final deliverable of this tutorial series is a written comparison of the three ETFs, produced as a report that combines computed metrics from the data with a personally verified check. Planned outputs include:

- This project plan (`artifacts/t1/project-plan.md`) as the starting point
- Later, an analysis report (for example `artifacts/t2/etf-comparison.md`) with an expense-ratio/drawdown table, calculated dates, one drawdown observation, and one manually verified check

Later analysis steps are planned work and are not yet completed.

## Three Project Milestones

1. **Set up the project (T1, current):** Review the repository and data dictionary, and write an initial project plan.
2. **Run a bounded analysis:** Have an agent inspect the inputs, write and run a small local calculation with an approved Python 3 or Node.js runtime, and produce the comparison report.
3. **Verify and save the result:** Manually check at least one computed value (e.g., a drawdown using `(trough / peak - 1) * 100`), review whether the results support the observation, and save the final report with Git.

## One Data Limitation

The dataset is synthetic teaching data: its values are illustrative assumptions, not current quotations, verified historical estimates, or forecasts. It also omits correlations, taxes, transaction costs, liquidity, currency exposure, and investor-specific constraints, so it cannot support real investment decisions.

## Next Action

Continue with the current task: review this plan and save it with Git. JiuwenSwarm must not commit or push the change during T1; the student performs the save. After that, proceed to the T2 exercise using the instructor-prepared data pack.
