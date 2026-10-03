# kubeshark

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kubeshark/kubeshark, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kubeshark

## Pinned environment

- Project commit: `35e484c9f1cc4a001bb174c0280a6d97c113d177`
- Test commit: `35e484c9f1cc4a001bb174c0280a6d97c113d177`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.9 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 4.9 | 0 | 0 | [run](https://argusic.com/run/16a08efd-0a01-4ad9-9595-bbe555b13ce5) |
| 2 | pass with mocks | 92 | 3 | 10.2 | 0 | 0 | [run](https://argusic.com/run/ee9acea7-ffe2-4912-b794-eb506586a5d9) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
