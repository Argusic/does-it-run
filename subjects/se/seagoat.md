# SeaGOAT

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kantord/SeaGOAT, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/seagoat

## Pinned environment

- Project commit: `dda7778020f4006b2a91e6f2bb7be922d45eb507`
- Test commit: `dda7778020f4006b2a91e6f2bb7be922d45eb507`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 29.9 to 29.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 29.9 | 1 | 1 | [run](https://argusic.com/run/c04ac6a9-c1db-410d-9716-0d9e566b641d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `12 snapshot tests error: ONNX MiniLM embedding model inference times out (>120s) on CPU during test fixture setup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
