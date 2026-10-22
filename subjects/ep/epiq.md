# epiq

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ljtn/epiq, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/epiq

## Pinned environment

- Project commit: `a293594bb75673c59c31efcb1e3b9810a32ffc80`
- Test commit: `a293594bb75673c59c31efcb1e3b9810a32ffc80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11.2 to 42.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 42.9 | 0 | 0 | [run](https://argusic.com/run/7948b2f0-55ad-4bf2-a841-97e35452be2a) |
| 2 | pass | 100 | 15 | 11.2 | 1 | 1 | [run](https://argusic.com/run/e10d1045-9b83-4713-a80c-e2c087282ab8) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `Node 18 required Node >=20 for vitest dependencies using /v regex flag`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
