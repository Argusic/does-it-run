# platform-ststm32

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/platformio/platform-ststm32, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/platform-ststm32

## Pinned environment

- Project commit: `c7fe5b923c22b9d0bf3304cc1a1fdbe9963f822e`
- Test commit: `c7fe5b923c22b9d0bf3304cc1a1fdbe9963f822e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 2.4 | 1 | 1 | [run](https://argusic.com/run/933936d0-431a-48e9-8b7a-c10c7969cd49) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing git submodules (builder/frameworks/libopencm3, builder/frameworks/arduino/mbed-core) caused 'missing SConscript file libopencm3.py' when building the libopencm3 example`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
