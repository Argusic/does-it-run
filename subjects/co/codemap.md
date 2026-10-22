# codemap

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JordanCoin/codemap, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/codemap

## Pinned environment

- Project commit: `df8436b746fc8a532cfff05e573d44381442d1d4`
- Test commit: `df8436b746fc8a532cfff05e573d44381442d1d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 10.7 | 6 | 6 | [run](https://argusic.com/run/e53ffbbf-ff0b-43ba-94fe-e597a7dbec8f) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go: not found on PATH`
- 2 min: `ast-grep not found; --deps and scanner tests degraded to Go-parser-only fallback`
- 2 min: `--diff/blast-radius/repo-handoff fail: no main branch (detached HEAD with no remote refs)`
- 1 min: `collide requires gh CLI + GitHub auth; gh not installed`
- 1 min: `gofmt reported deep non-style issue trigged by -d flag passthrough in e2e test under Go 1.27`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
