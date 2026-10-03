# xgo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/goplus/xgo, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/xgo

## Pinned environment

- Project commit: `ad73bea11e630f64972b2d822486e66739fc51b4`
- Test commit: `ad73bea11e630f64972b2d822486e66739fc51b4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.5 to 11.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.5 | 2 | 2 | [run](https://argusic.com/run/b846014e-ba83-4619-b5b7-3a5277e2b896) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Go compiler pre-installed in container`
- `xgo test ./... fails on XGo sources (builtin/doc.xgo type errors, cmd/chore/* undefined symbols)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
