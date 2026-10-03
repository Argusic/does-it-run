# rtk

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rtk-ai/rtk, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/rtk

## Pinned environment

- Project commit: `475f9ddfc20dbce4dab206329a36d8303cd9aa09`
- Test commit: `475f9ddfc20dbce4dab206329a36d8303cd9aa09`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 4; wall time 4.6 to 9.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 7.1 | 0 | 0 | [run](https://argusic.com/run/e0f82675-9a59-4579-85a4-05d1c59e1421) |
| 1 | pass | 100 | 5.5 | 9.3 | 0 | 0 | [run](https://argusic.com/run/bd74dbb5-e9b1-4051-8bba-260c5a89bb52) |
| 2 | pass | 100 | 2.5 | 4.6 | 0 | 0 | [run](https://argusic.com/run/c831c07c-1cc4-4fb0-9cce-7834e6a153ad) |
| 3 | pass | 100 | 6 | 7.6 | 0 | 0 | [run](https://argusic.com/run/bdbbd1db-d6f0-40a4-89a9-0b14f92dbca3) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
