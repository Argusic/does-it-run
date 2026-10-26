# vizra-adk

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vizra-ai/vizra-adk, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/vizra-adk

## Pinned environment

- Project commit: `dc5f302ac0d523febc731d80615aefb72feb2c30`
- Test commit: `dc5f302ac0d523febc731d80615aefb72feb2c30`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.6 to 8.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.6 | 2 | 2 | [run](https://argusic.com/run/d60f7a32-b003-4a61-b75e-92aad140a176) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.2+ not installed , missing entirely from container`
- 1 min: `Composer not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
