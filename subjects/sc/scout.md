# scout

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/outcrawlai/scout, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/scout

## Pinned environment

- Project commit: `3de831bba2f0bd57f8879a9e76eff3ead4a9042b`
- Test commit: `3de831bba2f0bd57f8879a9e76eff3ead4a9042b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.3 to 10.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 10.3 | 3 | 3 | [run](https://argusic.com/run/39cf50b5-9cbc-4914-a4aa-cc753b538680) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `bun is not installed in the container (only Node 18, but the project requires Bun and Node 22+)`
- 2 min: `playwright install under Node 18 was refused: 'Playwright requires Node.js 20 or higher'`
- 1 min: `my first draft standalone smoke script constructed Scout without models and aborted with ScoutConfigError: models is required`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
