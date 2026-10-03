# playwright-go

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mxschmitt/playwright-go, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/playwright-go

## Pinned environment

- Project commit: `775648cd1805851a893029e5eed1c8a0962b4e30`
- Test commit: `775648cd1805851a893029e5eed1c8a0962b4e30`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.7 to 41.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 41.7 | 3 | 3 | [run](https://argusic.com/run/5cd14fae-4b77-4780-ad9e-f86b81832404) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- `Playwright system dependency warning - host missing libgstreamer, libxslt, libsecret, etc.`
- `TestPageAddLocatorHandlerShouldThrowWhenHandlerTimesOut hangs when running full suite`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
