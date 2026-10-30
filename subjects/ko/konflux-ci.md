# konflux-ci

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/konflux-ci/konflux-ci, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/konflux-ci

## Pinned environment

- Project commit: `507449b62240718c3183d8cf1209b166b440b596`
- Test commit: `507449b62240718c3183d8cf1209b166b440b596`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.6 to 17.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 17.6 | 4 | 4 | [run](https://argusic.com/run/0cef2712-5d45-410a-9c9f-a6fb19aa96c3) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `container lacked Go toolchain; operator/go.mod requires go 1.26.0`
- 1 min: `make install failed: kubectl not found on PATH`
- 2 min: `bin/manager startup blocked because cert-manager CRDs absent (informers fail: no matches for kind Certificate)`
- 1 min: `operand pods cannot run: no container runtime/scheduler in this container (cert-manager-webhook unreachable, ApplyFailed on Certificate; Ready=False ComponentsNotReady)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
