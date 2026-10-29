# loomix

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/haaarshsingh/loomix, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/loomix

## Pinned environment

- Project commit: `8ec600923b149e8861a7796cd6d4012ce1289c9c`
- Test commit: `8ec600923b149e8861a7796cd6d4012ce1289c9c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.9 to 3.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 3.9 | 2 | 2 | [run](https://argusic.com/run/829f604e-6177-466d-84b4-6c0e35e3ce22) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Node.js is v18.19.1 but next build requires >=20.9.0`
- 1 min: `bun not installed and unzip system package missing, so bun.sh installer failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
