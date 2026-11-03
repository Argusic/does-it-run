# katana

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/projectdiscovery/katana, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/katana

## Pinned environment

- Project commit: `09c83e9a8b12b3eda90bd2b5d08b88787cadb62e`
- Test commit: `09c83e9a8b12b3eda90bd2b5d08b88787cadb62e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.5 to 7.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.7 | 0 | 0 | [run](https://argusic.com/run/8130284d-2e9d-44ef-84e0-774d40396613) |
| 2 | pass | 100 | 5 | 7.5 | 1 | 1 | [run](https://argusic.com/run/74877231-0d71-473c-89a1-9c7c656966e0) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go was not installed or available on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
