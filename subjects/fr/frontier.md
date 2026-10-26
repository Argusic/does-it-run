# frontier

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/singchia/frontier, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/frontier

## Pinned environment

- Project commit: `dda09a10387750fba85aab0853439081715ffcc6`
- Test commit: `dda09a10387750fba85aab0853439081715ffcc6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 27.8 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 3.5 | 27.8 | 3 | 0 | [run](https://argusic.com/run/1ad156ac-8b93-45a5-891f-d8d1ea0a009d) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `TestListenUDP hangs waiting for UDP packet (listen_test.go:19)`
- `TestEdgeManagerStream crashes with nil pointer dereference (edge_dataplane_test.go:34)`
- `TestServiceManager crashes with nil pointer dereference (service_manager_test.go:37)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
