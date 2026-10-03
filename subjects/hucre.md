# hucre

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/productdevbook/hucre, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hucre

## Pinned environment

- Project commit: `de00ffce5dec928a314808aae58aaa7b5553bc9d`
- Test commit: `de00ffce5dec928a314808aae58aaa7b5553bc9d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.5 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 3.5 | 0 | 0 | [run](https://argusic.com/run/b4346a50-9937-4f54-ab48-ad87b960c37d) |
| 2 | pass | 100 | 2 | 4.4 | 2 | 2 | [run](https://argusic.com/run/12dc7092-71da-4050-99cb-190caa885557) |

## What was observed on a clean machine

Attempt 2:

- 0.5 min: `Node v18.19.1 installed, project requires >=24`
- 0.1 min: `pnpm not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
