# homeassistant-solax-modbus

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wills106/homeassistant-solax-modbus, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-solax-modbus

## Pinned environment

- Project commit: `05a4a716140ea7a6583cf4439bbfaa95ee32dfb9`
- Test commit: `05a4a716140ea7a6583cf4439bbfaa95ee32dfb9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.1 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 5.1 | 1 | 1 | [run](https://argusic.com/run/960c1e3a-f2bb-4e4f-b252-207ce180a95f) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `TypeError: %x format: an integer is required, not str in logging for block.start`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
