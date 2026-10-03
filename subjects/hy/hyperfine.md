# hyperfine

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sharkdp/hyperfine, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/hyperfine

## Pinned environment

- Project commit: `f12f3d9f86f3643b3b7deace5e160b1f0f44d2b7`
- Test commit: `f12f3d9f86f3643b3b7deace5e160b1f0f44d2b7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 1.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0 | 2.9 | 0 | 0 | [run](https://argusic.com/run/8dabdb2c-7b00-4870-998a-75bb0b83fed4) |
| 2 | pass | 100 | 10 | 7.9 | 0 | 0 | [run](https://argusic.com/run/f310e0bb-74e7-4fbf-a341-331e9a255ca5) |
| 3 | pass | 100 | 0.5 | 1.9 | 0 | 0 | [run](https://argusic.com/run/91d45aa8-a020-4a0d-b55c-d895f6837a4c) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
