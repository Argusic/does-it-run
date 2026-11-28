# fora

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/imfeh2/fora, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/run/74f6e7f8-2479-47b9-acbe-6b90132980d9

## Pinned environment

- Project commit: `65cff719123a6d551461e2ff454a52ac90acb8ae`
- Test commit: `65cff719123a6d551461e2ff454a52ac90acb8ae`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.1 to 25.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 16 | 25.1 | 1 | 0 | [run](https://argusic.com/run/74f6e7f8-2479-47b9-acbe-6b90132980d9) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `bubblewrap (bwrap) not available for sandboxed execution - user namespaces disabled in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
