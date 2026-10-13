# axe

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jrswab/axe, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/axe

## Pinned environment

- Project commit: `937b509f1ff28e3610586c8891140ee15d87ad57`
- Test commit: `937b509f1ff28e3610586c8891140ee15d87ad57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 17.4 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 17.4 | 2 | 2 | [run](https://argusic.com/run/ff75c9e2-56fa-45eb-9b5b-9b52c92b9a0f) |

## What was observed on a clean machine

Attempt 1:

- 11 min: `Go toolchain not installed in container (go: not found); cannot build or test`
- 14 min: `After documented 'go build .', 'axe agents list' failed: open <cwd>/axe/agents: not a directory (ENOTDIR not filtered in agent auto-discovery)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
