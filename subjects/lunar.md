# lunar

**Verdict: runs.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lunarphp/lunar, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/lunar

## Pinned environment

- Project commit: `82f6e4a64585ac5f11ca1fce4b6897be870e691a`
- Test commit: `82f6e4a64585ac5f11ca1fce4b6897be870e691a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 21.8 to 36 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 21 | 21.8 | 1 | 0 | [run](https://argusic.com/run/01d35a52-f3cc-4ce7-9540-c1b3b8dc7417) |
| 2 | pass | 100 | 9 | 36 | 3 | 3 | [run](https://argusic.com/run/52b3779f-6d34-4718-9604-7fd50dbbdbb9) |

## What was observed on a clean machine

Attempt 1:

- 21 min: `PHP 8.3+ is required but not installed in the container and cannot be installed`

Attempt 2:

- 2 min: `PHP runtime not installed in container`
- 1 min: `Composer not installed in container`
- 1 min: `PHP memory limit too low (128MB) causing OOM in tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
