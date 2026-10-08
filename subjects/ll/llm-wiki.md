# llm-wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nvk/llm-wiki, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/llm-wiki

## Pinned environment

- Project commit: `1224fbcdf3827f4ba56d225a9e359f5e8a5594e5`
- Test commit: `1224fbcdf3827f4ba56d225a9e359f5e8a5594e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.2 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.01 | 4.2 | 2 | 2 | [run](https://argusic.com/run/0371ee34-629c-4e0b-9db9-2b72d819edcc) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test-local-cli-retract.sh failed due to missing xxd binary (not installed in container)`
- 3 min: `test-token-benchmarks.sh failed because benchmark script tried to create temp dirs in root-owned /work/ (root.parent)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
