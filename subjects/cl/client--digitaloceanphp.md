# Client

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DigitalOceanPHP/Client, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/36a999a5-2502-45a2-9007-95a3a8b1daa9

## Pinned environment

- Project commit: `2ac10c3212fb95fe08b39ebdf31b9471eabf20ac`
- Test commit: `2ac10c3212fb95fe08b39ebdf31b9471eabf20ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 2.7 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.1 | 1 | 1 | [run](https://argusic.com/run/36a999a5-2502-45a2-9007-95a3a8b1daa9) |
| 2 | pass | 100 | 2 | 2.7 | 0 | 0 | [run](https://argusic.com/run/dd2f93ae-ad37-43bc-bcd1-804ec18e5732) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP runtime and Composer not installed in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
