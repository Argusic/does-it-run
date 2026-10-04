# ios-simulator-mcp

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/joshuayoes/ios-simulator-mcp, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/ios-simulator-mcp

## Pinned environment

- Project commit: `a32f7f836393424d83b9476928da5518e178daa9`
- Test commit: `a32f7f836393424d83b9476928da5518e178daa9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 2.1 to 5.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 0.5 | 2.1 | 2 | 2 | [run](https://argusic.com/run/5f89fe11-8d11-45ba-9db8-da01c2a33fa7) |
| 2 | pass with mocks | 92 | 0.5 | 5.2 | 1 | 1 | [run](https://argusic.com/run/d115f25a-c186-4ca1-a834-c865392b378e) |

## What was observed on a clean machine

Attempt 1:

- `npm install emitted EBADENGINE warnings because node v18.19.1 < required v20, but install and tsc build completed successfully`
- `xcrun not found on Linux (expected , requires macOS/Xcode)`

Attempt 2:

- `Node.js v18.19.1 is below the required >=20 engine. npm install warns but works; tsc compiles fine.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
