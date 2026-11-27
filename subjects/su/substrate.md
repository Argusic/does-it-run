# substrate

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agent-substrate/substrate, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/substrate

## Pinned environment

- Project commit: `715f2daa63371a19f54a0e37997569e3c2cb3cb9`
- Test commit: `715f2daa63371a19f54a0e37997569e3c2cb3cb9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.5 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 12 | 16.5 | 2 | 0 | [run](https://argusic.com/run/aeda57bb-da1c-4e9b-bda4-f3e56e453c28) |

## What was observed on a clean machine

Attempt 1:

- `Test TestSetSysctlReportsAnUnrelatedError in internal/ateomnet/netns fails because /proc/sys is mounted read-only in the container (needs CAP_SYS_ADMIN/root)`
- `Docker, kubectl, and kind are not installed , full cluster-based install (kind/GKE) and E2E tests cannot run in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
