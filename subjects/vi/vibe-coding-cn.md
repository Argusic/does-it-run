# vibe-coding-cn

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tradecatlabs/vibe-coding-cn, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vibe-coding-cn

## Pinned environment

- Project commit: `3b8759744e7fd12cb79c4fbe3ac6c6455edfb779`
- Test commit: `3b8759744e7fd12cb79c4fbe3ac6c6455edfb779`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.6 to 5.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 5.6 | 4 | 4 | [run](https://argusic.com/run/4d6854ce-7ee1-43d5-8355-6c3ffa821c7a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 system install is too old for markdownlint-cli@0.48.0 (requires >=20)`
- 1 min: `pip install fails: externally-managed-environment (Debian)`
- `make test failed on check-external-resources: system python3 missing PyYAML`
- `check-research-raw fails: 35 research/ domains missing raw/repository directories`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
