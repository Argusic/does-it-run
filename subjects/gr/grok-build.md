# grok-build

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xai-org/grok-build, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/grok-build

## Pinned environment

- Project commit: `37949780c144e37df692e3d669051a21fec24f20`
- Test commit: `37949780c144e37df692e3d669051a21fec24f20`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 70.1 to 81.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 70.1 | 0 | 0 | [run](https://argusic.com/run/117d6152-1a3c-4073-b3f4-e89a66f21324) |
| 2 | fail | 20 | n/a | 81.1 | 0 | 0 | [run](https://argusic.com/run/bc7ca44d-4581-466c-bee3-c2d89bbce495) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
