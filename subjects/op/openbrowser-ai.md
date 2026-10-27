# openbrowser-ai

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/billy-enrizky/openbrowser-ai, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/openbrowser-ai

## Pinned environment

- Project commit: `447d886a733f0e4db1340b98585b0d3248c69d30`
- Test commit: `447d886a733f0e4db1340b98585b0d3248c69d30`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.7 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 26.7 | 2 | 2 | [run](https://argusic.com/run/7795b527-2a6f-4858-918b-b3480e02ebdf) |

## What was observed on a clean machine

Attempt 1:

- `openbrowser-ai install uses 'uvx' which is not in container`
- `'openbrowser-ai --template' fails because InquirerPy not listed in dev deps`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
