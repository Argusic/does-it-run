# toast

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/stepchowfun/toast, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/toast

## Pinned environment

- Project commit: `a6d5791eb652230533515d39bb4ac9da8677f3d7`
- Test commit: `a6d5791eb652230533515d39bb4ac9da8677f3d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 3.2 | 2 | 2 | [run](https://argusic.com/run/82032f48-5d46-47ad-b3cb-3710155a9cad) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Install.sh script fails without /dev/tty and sudo in non-interactive container`
- `Docker not available (no binary, no socket) - core Toast functionality requires Docker`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
