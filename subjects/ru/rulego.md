# rulego

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rulego/rulego, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/rulego

## Pinned environment

- Project commit: `9ccf5f5416bb3821e29bf9116f059e9aa02b0df4`
- Test commit: `9ccf5f5416bb3821e29bf9116f059e9aa02b0df4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.1 to 8.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 8.1 | 1 | 1 | [run](https://argusic.com/run/bf0b2d52-28b9-4265-b16e-f63d746e079e) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go compiler (golang) not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
