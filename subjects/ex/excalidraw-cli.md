# excalidraw-cli

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/swiftlysingh/excalidraw-cli, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/excalidraw-cli

## Pinned environment

- Project commit: `838ff3caefc0511055db0780210a27ca704a1f0d`
- Test commit: `838ff3caefc0511055db0780210a27ca704a1f0d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.6 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 7.6 | 7.6 | 2 | 1 | [run](https://argusic.com/run/e18d78d2-9ffe-4072-a8c4-7000823643a7) |

## What was observed on a clean machine

Attempt 1:

- 2.5 min: `Node.js v18.19.1 is installed but project requires >=20.19.0`
- `Test 'is not behind any stable git tag' fails because the checkout has zero git tags`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
