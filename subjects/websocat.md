# websocat

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vi/websocat, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/websocat

## Pinned environment

- Project commit: `3a3574cd2f5d17857d87f3982e72c3ede159dde0`
- Test commit: `3a3574cd2f5d17857d87f3982e72c3ede159dde0`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 2.5 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 25.1 | 0 | 0 | [run](https://argusic.com/run/ef44f2b6-02fd-4df8-b347-eafbe4440eb2) |
| 2 | pass | 100 | 0.5 | 2.7 | 0 | 0 | [run](https://argusic.com/run/55a56de4-7da6-42ae-b82e-aa2842add2f0) |
| 3 | pass | 100 | 8 | 2.5 | 0 | 0 | [run](https://argusic.com/run/8a2a9663-d116-40e7-adf3-ddb3d6eb4dc1) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
