# homeassistant-solax-modbus

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/wills106/homeassistant-solax-modbus, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-solax-modbus

## Pinned environment

- Project commit: `05a4a716140ea7a6583cf4439bbfaa95ee32dfb9`
- Test commit: `05a4a716140ea7a6583cf4439bbfaa95ee32dfb9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 3 to 5.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.5 | 5.1 | 1 | 1 | [run](https://argusic.com/run/960c1e3a-f2bb-4e4f-b252-207ce180a95f) |
| 2 | pass with mocks | 92 | 5 | 3 | 1 | 1 | [run](https://argusic.com/run/c2a6d0ad-4c3b-48b5-bc17-f81e375a0d60) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `TypeError: %x format: an integer is required, not str in logging for block.start`

Attempt 2:

- 5 min: `%x format specifier in logging and _block_key() in __init__.py failed when block.start/block.end were non-integer strings (e.g. 'inverter', 'pm') from test mocks, causing TypeError: %x format: an integer is required, not str`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
