# dsh-hub-cli

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/pax-beehive/dsh-hub-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/dsh-hub-cli

## Pinned environment

- Project commit: `1805424c762dec4fb24675f8c1f3202c0eb98091`
- Test commit: `1805424c762dec4fb24675f8c1f3202c0eb98091`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 2.2 | 1 | 1 | [run](https://argusic.com/run/d6a6b417-2c1f-416c-9ab1-6bb27eef64ee) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Container only has Node v18.19.1 and no pnpm/corepack; project requires Node >=22.13 and pnpm 10.33`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
