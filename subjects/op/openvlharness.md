# OpenVLHarness

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/uclanlp/OpenVLHarness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openvlharness

## Pinned environment

- Project commit: `c080224d31774fcf1b3c0f55abb71d143f7f3501`
- Test commit: `c080224d31774fcf1b3c0f55abb71d143f7f3501`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 2.5 to 5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 5 | 0 | 0 | [run](https://argusic.com/run/24a5aa74-bc12-4198-b8cc-5e68dd737de3) |
| 2 | fail | 80 | 0.5 | 2.5 | 0 | 0 | [run](https://argusic.com/run/1329d9e7-5ae3-4eb6-a602-16a9d625a558) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
