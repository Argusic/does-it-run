# html2image

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vgalin/html2image, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/html2image

## Pinned environment

- Project commit: `81c0609f57c1b604485a39d23fb4e0b211015745`
- Test commit: `81c0609f57c1b604485a39d23fb4e0b211015745`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.6 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 30 | 4.6 | 5 | 5 | [run](https://argusic.com/run/c1c32d98-a3f5-4da9-a14a-1b2e8bdaec07) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `No Chrome/Chromium browser found on the system`
- 3 min: `Chrome crashes with 'No usable sandbox' error (requires --no-sandbox)`
- 1 min: `pip 26.x internal error: cannot import name 'importlib' from pip._internal.metadata`
- 2 min: `Edge browser tests fail because msedge is not installed`
- 1 min: `System pip blocked by PEP 668 externally-managed-environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
