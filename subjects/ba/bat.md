# bat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sharkdp/bat, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/bat

## Pinned environment

- Project commit: `7323a7514f7601737640e7172be115127d6db08c`
- Test commit: `7323a7514f7601737640e7172be115127d6db08c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 4.7 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 9.5 | 0 | 0 | [run](https://argusic.com/run/bfe0e2de-d9ff-4ec6-9fc1-ac36de5567b9) |
| 2 | pass | 100 | 1.2 | 4.7 | 0 | 0 | [run](https://argusic.com/run/4baea2fe-346b-4637-8337-b999d114fa06) |
| 3 | pass | 100 | 3.5 | 5.4 | 0 | 0 | [run](https://argusic.com/run/ab6ed57f-955c-4e43-a2f7-de3c783fc456) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
