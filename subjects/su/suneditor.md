# suneditor

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JiHong88/suneditor, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/suneditor

## Pinned environment

- Project commit: `4f3d788f8ab394c578cd509bcbda13c43aa68f6e`
- Test commit: `4f3d788f8ab394c578cd509bcbda13c43aa68f6e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 39.1 to 87 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87 | 0 | 0 | [run](https://argusic.com/run/f7b5f21a-f9ce-41a0-98fe-e984cc5e24f8) |
| 2 | pass | 100 | 2 | 39.1 | 2 | 2 | [run](https://argusic.com/run/09578a1b-c346-477e-97a2-f7ec9d27672f) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `jest OOM crash (1-2 suites killed) under default 128-worker parallelism in 512MB container , all OOM'd suites pass when run individually`
- 2 min: `npm run build:dev CSS minimizer: serialize-javascript uses crypto.getRandomValues without import, fails on Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
