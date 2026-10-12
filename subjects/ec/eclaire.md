# eclaire

**Verdict: runs.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eclaire-labs/eclaire, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/eclaire

## Pinned environment

- Project commit: `b6da8f854bf56237df16ab567e2de604e4a9e5e3`
- Test commit: `b6da8f854bf56237df16ab567e2de604e4a9e5e3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 58.3 to 58.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 92 | 46 | 58.3 | 5 | 3 | [run](https://argusic.com/run/af035824-9621-42aa-9e89-ba7d752e59b5) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Container ships Node 18 but project requires Node ^24`
- 5 min: `Interactive setup.js cannot be driven in the harness (PTY input not delivered)`
- 2 min: `Electron aborts in unprivileged container: SUID chrome-sandbox not owned by root`
- 3 min: `pnpm lint exits 1: 542 pre-existing no-unused-vars/no-explicit-any errors in repo source`
- 4 min: `pnpm test:unit intermittently fails in @eclaire/queue due to vitest fork timeout in timing/timing-sensitive files (job-stages, timing-and-lease); all queue tests pass on clean rerun`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
