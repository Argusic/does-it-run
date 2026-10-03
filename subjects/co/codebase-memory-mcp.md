# codebase-memory-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DeusData/codebase-memory-mcp, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/codebase-memory-mcp

## Pinned environment

- Project commit: `c38aa35c277395e71fc8fd2f904231e6d909b5f0`
- Test commit: `c38aa35c277395e71fc8fd2f904231e6d909b5f0`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 3; wall time 14.9 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/ae952dec-94ae-4e5f-951c-dfe191c40e87) |
| 2 | pass | 100 | 11.67 | 14.9 | 2 | 2 | [run](https://argusic.com/run/bc9c3196-fa1b-4735-9dfb-5c26477585ac) |
| 3 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/5de55c6a-4d75-4e5e-8881-3f14e4cf048b) |

## What was observed on a clean machine

Attempt 2:

- 1.5 min: `npm install via npx failed: activation_transaction I/O failed due to group-writable npm cache directory permissions (mode 0775)`
- 2 min: `Full index mode (index_repository without --mode flag) killed by OOM (signal 9, peak 1689 MB RSS against 491 MB budget)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
