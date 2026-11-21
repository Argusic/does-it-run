# isocast

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anomalyco/isocast, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/isocast

## Pinned environment

- Project commit: `dd2d1038f10ae90e07bd08582881ba21aaeaa0cc`
- Test commit: `dd2d1038f10ae90e07bd08582881ba21aaeaa0cc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.1 to 44.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 44.1 | 1 | 1 | [run](https://argusic.com/run/376ca6f5-ad04-4315-9fce-2cca1de5c0a2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `OpenH264 library was a broken 9-byte placeholder instead of the real Cisco binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
