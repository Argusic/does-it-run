# tinydb

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/msiemens/tinydb, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tinydb

## Pinned environment

- Project commit: `4aa53111d72c9cbaafcdc039211caf49f4face6f`
- Test commit: `4aa53111d72c9cbaafcdc039211caf49f4face6f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 1.8 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.3 | 1.8 | 0 | 0 | [run](https://argusic.com/run/c8642b71-3b5d-40ba-9c84-26438199b1e6) |
| 2 | pass | 100 | 0.3 | 2 | 0 | 0 | [run](https://argusic.com/run/fbf4df59-5760-4581-8518-f6f107d11111) |
| 3 | pass | 100 | 15 | 3.1 | 3 | 3 | [run](https://argusic.com/run/04d63596-12ef-444a-8bc6-2c2fe98959cd) |

## What was observed on a clean machine

Attempt 3:

- 6 min: `smoke script expected ~(name=='John') to contain only Bob, forgot int/char rows`
- 2 min: `smoke script assumed update({age:23}) matched one John row; it matches both`
- 2 min: `smoke script asserted new-table insert returns 1, but prior failed runs left a doc in the extra table`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
