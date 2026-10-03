# gentle-ai

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gentleman-Programming/gentle-ai, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gentle-ai

## Pinned environment

- Project commit: `2c25e878eea407876abf96f3448ab56b8f79e344`
- Test commit: `2c25e878eea407876abf96f3448ab56b8f79e344`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 16.9 to 79.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 80 | 3 | 79.4 | 5 | 2 | [run](https://argusic.com/run/90f3e3d7-9f09-4ea4-9616-e678301ee9a4) |
| 2 | pass | 100 | 3 | 23.5 | 1 | 1 | [run](https://argusic.com/run/d3328763-067e-4b67-a0f9-04d3dc1980ad) |
| 3 | pass | 100 | 3 | 16.9 | 2 | 2 | [run](https://argusic.com/run/aa54658f-b755-4f04-ad76-4a6cc0dca323) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Go 1.25.10 not installed on system`
- 15 min: `Node.js v18.19.1 cannot execute .mts TypeScript files directly`
- `internal/cli tests hang waiting on /dev/tty for git clone`
- `internal/components/sdd tests have concurrency deadlock when run as a suite (all individual tests pass)`
- `internal/reviewtransaction tests have slow git-file-backed tests that time out under load (some pass individually)`

Attempt 2:

- 3 min: `Go 1.25.10+ not installed`

Attempt 3:

- 2.5 min: `Go 1.25.10+ not found in container (Ubuntu 24.04 ships Go 1.22)`
- 2.5 min: `Node.js 18 does not natively support .mts TypeScript files; tests failed with SyntaxError: Cannot use import statement outside a module`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
