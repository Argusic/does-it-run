# zensical

**Verdict: runs.** Argusic Score 98.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zensical/zensical, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/zensical

## Pinned environment

- Project commit: `27fa3105d2f27ad7f6b98fc87944450316f58078`
- Test commit: `27fa3105d2f27ad7f6b98fc87944450316f58078`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.7 to 22.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 22.4 | 6 | 6 | [run](https://argusic.com/run/132a555d-7766-43e0-882b-b51041b39d78) |
| 2 | pass | 96.67 | 38 | 15.7 | 6 | 5 | [run](https://argusic.com/run/1d8955a0-fa31-40ba-9f56-83d133715762) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Rust toolchain not installed`
- 1 min: `Externally-managed Python environment prevents system pip installs`
- 1 min: `UI templates missing (zensical/templates/ was gitignored, empty)`
- 0.1 min: `Initial build failed because Cargo not on PATH for maturin`
- 2 min: `Unit tests failed with 'zensical.zensical' import error (repo shadowing installed module) and missing bs4/pandas`
- `31 pandas table-reader tests fail on pandas 3.x API changes`

Attempt 2:

- 18 min: `No Rust toolchain installed`
- 3 min: `System pip blocked by PEP 668 external environment policy`
- 1 min: `maturin not found on PATH during pip build subprocess`
- 3 min: `Missing dev dependencies (bs4, lxml, etc.)`
- 13 min: `Missing templates/ directory for builtin theme`
- `Pre-existing integration test fixture failure (test_preserves_entity_spellings_in_titles)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
