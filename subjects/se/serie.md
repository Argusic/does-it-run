# serie

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lusingander/serie, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/serie

## Pinned environment

- Project commit: `4ac4539f802ab1cede9356b02a8e6ca450b604b9`
- Test commit: `4ac4539f802ab1cede9356b02a8e6ca450b604b9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.25 | 5.3 | 0 | 0 | [run](https://argusic.com/run/6579c06f-6d7d-47e9-999e-6b695332d291) |
| 2 | pass | 100 | 1.75 | 3 | 1 | 1 | [run](https://argusic.com/run/83b7df74-ad56-441d-88ff-9ae57c8efe56) |

## What was observed on a clean machine

Attempt 2:

- 0.16 min: `No Rust toolchain installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
