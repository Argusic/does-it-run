# ownmem

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grpcer/ownmem, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ownmem

## Pinned environment

- Project commit: `f75cd4bb183464443b6c517de67ba61a4962501d`
- Test commit: `f75cd4bb183464443b6c517de67ba61a4962501d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 1.5 to 1.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 1.5 | 0 | 0 | [run](https://argusic.com/run/92fb873a-6dd4-4166-b5a0-efd9bfd4fb7b) |
| 2 | pass | 100 | 3 | 1.6 | 1 | 1 | [run](https://argusic.com/run/3f369daf-1ef9-4fac-95b6-38eb47a064a8) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Node.js v18.19.1 is pre-installed but ownmem requires >=20.6.0`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
