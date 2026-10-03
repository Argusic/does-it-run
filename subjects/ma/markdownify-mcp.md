# markdownify-mcp

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zcaceres/markdownify-mcp, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/markdownify-mcp

## Pinned environment

- Project commit: `024f97cea9a94cd842c445eea4503c442c79bd71`
- Test commit: `024f97cea9a94cd842c445eea4503c442c79bd71`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.7 | 1 | 1 | [run](https://argusic.com/run/6cc36db5-1f35-47f6-a05b-7124909665ff) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `repmomix shebang uses 'node' but Node 18 can't run repomix (needs Node 20+); all 11 fromRepo tests failed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
