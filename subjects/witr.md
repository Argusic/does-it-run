# witr

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pranshuparmar/witr, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/witr

## Pinned environment

- Project commit: `dc4fa1da82d3e266fcbd928641b4f30b3077c64f`
- Test commit: `dc4fa1da82d3e266fcbd928641b4f30b3077c64f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 3.8 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.2 | 0 | 0 | [run](https://argusic.com/run/a5d119bb-e666-4f29-b48a-2faf68f1c944) |
| 2 | pass | 100 | 3.1 | 4.2 | 1 | 1 | [run](https://argusic.com/run/fc6281fd-fba1-45b6-a029-bf7e65fd92b5) |
| 3 | pass | 100 | 8 | 3.8 | 0 | 0 | [run](https://argusic.com/run/0c0e17ad-559f-47d4-94eb-4e3f02cb98a5) |

## What was observed on a clean machine

Attempt 2:

- 1.5 min: `Go compiler not found on system PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
