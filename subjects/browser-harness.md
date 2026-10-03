# browser-harness

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/browser-harness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/browser-harness

## Pinned environment

- Project commit: `afbcc381b963040c19627d788e40c7e7663171ee`
- Test commit: `afbcc381b963040c19627d788e40c7e7663171ee`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.8 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 4.8 | 2 | 2 | [run](https://argusic.com/run/a26c8481-60d9-4618-a699-86448782281b) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `No Chrome browser installed in container , daemon refused to start`
- 2 min: `Chrome needs --no-sandbox in unprivileged container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
