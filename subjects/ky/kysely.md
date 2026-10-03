# kysely

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kysely-org/kysely, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/kysely

## Pinned environment

- Project commit: `cd479e295aaf13eb9e2140efdae7e57d6b2e412e`
- Test commit: `cd479e295aaf13eb9e2140efdae7e57d6b2e412e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.9 to 6.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 6.9 | 2 | 2 | [run](https://argusic.com/run/fabf55f1-58fb-4232-a7ae-94a9339f3aba) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18 was installed but project requires >=22`
- 1 min: `pnpm not found in PATH before nvm switch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
