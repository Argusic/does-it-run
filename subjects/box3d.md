# box3d

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/erincatto/box3d, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/box3d

## Pinned environment

- Project commit: `9f998c862d54c03a633ecea3831937385c78b532`
- Test commit: `9f998c862d54c03a633ecea3831937385c78b532`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.2 | 1 | 1 | [run](https://argusic.com/run/64501cc9-e3fe-4740-817c-b5b5a05c717d) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Samples build failed: gtk+-3.0 dev headers not found for nfd dependency (requires libgtk-3-dev, libxi-dev, libxcursor-dev)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
