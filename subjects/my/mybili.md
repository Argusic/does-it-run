# mybili

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ellermister/mybili, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/mybili

## Pinned environment

- Project commit: `6f79230017d10eb4869bd03c4fc7975b86420c43`
- Test commit: `6f79230017d10eb4869bd03c4fc7975b86420c43`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.5 to 4.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 4.5 | 5 | 5 | [run](https://argusic.com/run/faaaa290-b4a7-444a-8329-7600fa353314) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PHP 8.3 not installed in container`
- 1 min: `Composer not installed in container`
- 1 min: `Redis-server not installed in container`
- 1 min: `pnpm not installed (node v18 incompatible with pnpm 11)`
- 1 min: `Vite manifest not found - frontend assets not built`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
