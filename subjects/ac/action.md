# action

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/test-summary/action, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/action

## Pinned environment

- Project commit: `001f872f7d3bfc266130826cdd8c4b9ca30b15c3`
- Test commit: `001f872f7d3bfc266130826cdd8c4b9ca30b15c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2 to 2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 2 | 2 | 2 | [run](https://argusic.com/run/5e4717b2-00cb-4af4-901c-1e3d5ffd8fb2) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `lint reported 109 errors, and the lint step non-zero exit was masked by shell pipe`
- 1 min: `the built action rejected test/resources/tap/10-results-after-trailer.tap`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
