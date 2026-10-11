# k8spacket

**Verdict: runs.** Argusic Score 75 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k8spacket/k8spacket, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/k8spacket

## Pinned environment

- Project commit: `76c2d1de1ac4fe802a88355bfd638b83be50413c`
- Test commit: `76c2d1de1ac4fe802a88355bfd638b83be50413c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 2 | 11.9 | 2 | 2 | [run](https://argusic.com/run/af3e7265-e03f-47ef-81de-d36f0ab4654d) |
| 2 | pass | 100 | 6 | 5.9 | 1 | 1 | [run](https://argusic.com/run/2e756699-4c0a-4b91-b58d-7f5655ea93a0) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Go toolchain not installed in container`
- `eBPF program loading requires kernel capabilities (unprivileged container)`

Attempt 2:

- 1 min: `Go compiler not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
