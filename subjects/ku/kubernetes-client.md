# kubernetes-client

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/maclof/kubernetes-client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/kubernetes-client

## Pinned environment

- Project commit: `1b0bdbd2e69f9a6567b1a10fe6db85762d9df3ad`
- Test commit: `1b0bdbd2e69f9a6567b1a10fe6db85762d9df3ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 7.2 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11.4 | 0 | 0 | [run](https://argusic.com/run/7ecabc50-9a78-4fc9-9f17-a5ae5a4df12a) |
| 2 | pass with mocks | 92 | 6 | 7.2 | 2 | 2 | [run](https://argusic.com/run/efcdba2d-c8e4-4d8b-8b88-f2c38bf4a4ad) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `PHP runtime not installed in container`
- 1 min: `Composer not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
