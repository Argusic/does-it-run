# abogen

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/denizsafak/abogen, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/abogen

## Pinned environment

- Project commit: `08e2ee8b85bbb7a6bdbe4d21adbed3150a0f80c5`
- Test commit: `08e2ee8b85bbb7a6bdbe4d21adbed3150a0f80c5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.4 to 22.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11.2 | 22.4 | 3 | 3 | [run](https://argusic.com/run/3b4118e7-21ae-4ff5-8f6a-62b1d9747a56) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Debian's externally-managed Python blocked direct pip install`
- 0.5 min: `sh shell lacks source; . venv/bin/activate used instead`
- 1.5 min: `PyQt test crashed with Aborted (no display)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
