# ProductFlow

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yuqie6/ProductFlow, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/productflow

## Pinned environment

- Project commit: `649a8a52f26a39327dac734b5cd0bcb8c9b2f1b0`
- Test commit: `649a8a52f26a39327dac734b5cd0bcb8c9b2f1b0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 7.9 | 4 | 4 | [run](https://argusic.com/run/36e50c3f-aee6-4716-975c-f6707196557c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `hatchling build rejects readme path outside project directory`
- 1 min: `test_image_generation_core.py missing env-vars fixture`
- 4 min: `pnpm install blocked (no root, esbuild build scripts)`
- 5 min: `Vite 7 requires Node 20.19+, container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
