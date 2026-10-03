# Heimdall

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/linuxserver/Heimdall, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/heimdall

## Pinned environment

- Project commit: `808cc90db62b3935f44b91d8feb8af56640f5ce9`
- Test commit: `808cc90db62b3935f44b91d8feb8af56640f5ce9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 8 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 18 | 20.4 | 1 | 1 | [run](https://argusic.com/run/491ff3f0-0f7c-4360-8823-3f9b2e8872ab) |
| 2 | pass | 100 | 10 | 9.5 | 1 | 1 | [run](https://argusic.com/run/5279fe44-ecdf-4d2e-914d-9e0f6e26b43b) |
| 3 | pass | 100 | 6 | 8 | 0 | 0 | [run](https://argusic.com/run/4f3ecd1d-7cd7-42f3-84ec-1249a3167698) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP 8.4+ not installed in container (no root access for apt)`

Attempt 2:

- 3 min: `PHP binary not found in container (php not installed, sudo not available, apt-get locked)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
