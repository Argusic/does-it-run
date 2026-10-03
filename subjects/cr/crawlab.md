# crawlab

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crawlab-team/crawlab, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/crawlab

## Pinned environment

- Project commit: `0485310def8b4f31ea20997846a8d5e7dfc681e5`
- Test commit: `0485310def8b4f31ea20997846a8d5e7dfc681e5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.3 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 17.3 | 4 | 4 | [run](https://argusic.com/run/37b06031-8945-4e93-8122-4746c3660ffa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 1 min: `Vet error: fmt.Sprintf %%s used with int port args in 6 db utility files`
- 2 min: `No MongoDB available for tests requiring DB`
- 1 min: `Persisted config.json had is_master:false blocking master mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
