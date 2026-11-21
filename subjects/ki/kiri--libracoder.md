# kiri

**Verdict: not yet verified.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/libracoder/kiri, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/run/f5e021de-91ea-4d3a-a4c3-2d0a487fc8f5

## Pinned environment

- Project commit: `260cf66b9b56963a0170857c2b4306c38814e108`
- Test commit: `260cf66b9b56963a0170857c2b4306c38814e108`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 7.1 | 1 | 1 | [run](https://argusic.com/run/f5e021de-91ea-4d3a-a4c3-2d0a487fc8f5) |

## What was observed on a clean machine

Attempt 1:

- `5 kiri-init layer tests fail when run as non-root: tar unpack tries to chown entries to uid 0 (PermissionDenied)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
