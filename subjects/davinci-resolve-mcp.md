# davinci-resolve-mcp

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/samuelgursky/davinci-resolve-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/davinci-resolve-mcp

## Pinned environment

- Project commit: `6337d8cf706852854b601e3ce05d643a9366b905`
- Test commit: `6337d8cf706852854b601e3ce05d643a9366b905`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.6 to 21.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 35 | 21.6 | 2 | 0 | [run](https://argusic.com/run/a5601ea3-9531-4afb-af11-8ef1d91c72d9) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `DaVinci Resolve not installed - scripting API paths not found; install.py warns but proceeds`
- 5 min: `Node.js v18.19.1 < 20.9 required by resolve-advanced; 17/961 tests fail`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
