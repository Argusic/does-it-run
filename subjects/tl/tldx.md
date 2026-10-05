# tldx

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brandonyoungdev/tldx, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/tldx

## Pinned environment

- Project commit: `eb7468bae310428234fcb8b5d162a84ccf7de1d5`
- Test commit: `eb7468bae310428234fcb8b5d162a84ccf7de1d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 32.3 to 32.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 32.3 | 2 | 2 | [run](https://argusic.com/run/8e0bb2bb-1c20-491c-8f20-5996fed2ed2d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go toolchain not installed in container (no root to apt-install)`
- 1 min: `First attempt to download Go used wrong archive name .linux-x64 (404)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
