# python-calamine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dimastbk/python-calamine, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/python-calamine

## Pinned environment

- Project commit: `b6edec2f844c1b03f363067dc47bd21dd3e1cb2c`
- Test commit: `b6edec2f844c1b03f363067dc47bd21dd3e1cb2c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.1 to 2.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 2.1 | 2 | 2 | [run](https://argusic.com/run/4a7edee4-edd3-49da-81d3-0cc9646b3bb3) |

## What was observed on a clean machine

Attempt 1:

- 0.18 min: `Rust (rustc/cargo) not installed in container`
- 0.03 min: `System pip blocked by externally-managed-environment (PEP 668)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
