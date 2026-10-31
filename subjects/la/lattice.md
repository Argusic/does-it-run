# lattice

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/techygarg/lattice, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/lattice

## Pinned environment

- Project commit: `4b0bc6e625b99a98044ebe97e2440b3bbda937c9`
- Test commit: `4b0bc6e625b99a98044ebe97e2440b3bbda937c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15 to 15 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 45 | 15 | 1 | 0 | [run](https://argusic.com/run/0a85a31b-7856-4d94-b13d-217c849d05e8) |

## What was observed on a clean machine

Attempt 1:

- 30 min: `npm run build fails: Minimum Node.js version not met (Node v18.19.1 vs engines.node >=20.0 pinned by repo and CI)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
