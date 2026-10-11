# pisa

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pisa-engine/pisa, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/pisa

## Pinned environment

- Project commit: `d0145556881e23e9b3ac53441c69675209ba0a76`
- Test commit: `d0145556881e23e9b3ac53441c69675209ba0a76`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19 to 19 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 19 | 2 | 2 | [run](https://argusic.com/run/5c4f3b0b-a86a-428d-8ef9-cec2de0494ab) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Submodules not initialized - empty external directories prevented CMake configuration`
- 2 min: `gumbo-parser build failed: requires libtoolize/autotools (not installed, no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
