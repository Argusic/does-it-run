# tcping

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pouriyajamshidi/tcping, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/tcping

## Pinned environment

- Project commit: `7de8f932f49b50ad9f3af93edc5e038d7d2b6c19`
- Test commit: `7de8f932f49b50ad9f3af93edc5e038d7d2b6c19`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 3.7 | 1 | 1 | [run](https://argusic.com/run/51b79239-4050-45c7-8061-9252b77d2864) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go toolchain not found in PATH (no Go binary in container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
