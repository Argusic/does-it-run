# numa

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/razvandimescu/numa, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/numa

## Pinned environment

- Project commit: `df7bd995d1108c8f9d92afeffa5efc21c8ac8ba3`
- Test commit: `df7bd995d1108c8f9d92afeffa5efc21c8ac8ba3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.8 to 5.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 5.8 | 1 | 1 | [run](https://argusic.com/run/dc6cf2b2-a301-4363-bcae-a2a10d1f032f) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Rust toolchain not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
