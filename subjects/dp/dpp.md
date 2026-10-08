# DPP

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/brainboxdotcc/DPP, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/dpp

## Pinned environment

- Project commit: `786ceb2e24f286d4e7f4b6b4a5dd934effdee6a4`
- Test commit: `786ceb2e24f286d4e7f4b6b4a5dd934effdee6a4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 7.8 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 7 | 7.8 | 1 | 1 | [run](https://argusic.com/run/c3715ab5-0a8f-4570-99c6-d74088a10434) |
| 2 | pass | 100 | 18 | 19.8 | 1 | 1 | [run](https://argusic.com/run/4a1d31c5-d3b8-448f-adcd-23e56a61906a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Missing zlib development headers and library symlink`

Attempt 2:

- 5 min: `zlib1g-dev package not installed (missing ZLIB headers/libs)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
