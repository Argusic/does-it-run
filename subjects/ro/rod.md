# rod

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/go-rod/rod, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/rod

## Pinned environment

- Project commit: `d38c75327872c72a1cf2010dad7527f9e52eebf3`
- Test commit: `d38c75327872c72a1cf2010dad7527f9e52eebf3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 59 to 59 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 0.15 | 59 | 5 | 4 | [run](https://argusic.com/run/ce5f45b2-d92e-4908-ae04-fc205ef83eb0) |

## What was observed on a clean machine

Attempt 1:

- 0.15 min: `Go compiler not found in environment`
- 0.1 min: `gotrace requires GODEBUG=tracebackancestors=1000`
- 0.1 min: `TestShapeInIframe: X coordinate delta 2.89 > tolerance 1`
- 0.2 min: `TestLaunchUserMode: container has no sandbox, chromium crashes without --no-sandbox`
- `TestManaged: pre-existing flaky race condition with context timeout causing net.OpError type assertion panic`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
