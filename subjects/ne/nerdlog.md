# nerdlog

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dimonomid/nerdlog, licensed BSD-2-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/nerdlog

## Pinned environment

- Project commit: `0ff0e8cce10d7745fc6e30d82cc1419d9725b79a`
- Test commit: `0ff0e8cce10d7745fc6e30d82cc1419d9725b79a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.4 to 16.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 7.4 | 3 | 3 | [run](https://argusic.com/run/8f58a565-08a7-4a6f-bebe-a794e5780d90) |
| 2 | pass | 95 | 4 | 16.5 | 4 | 3 | [run](https://argusic.com/run/4d0c696a-474f-43cd-a0ec-e4406a08102c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not found in container`
- 2 min: `gawk (GNU awk) not installed; required by nerdlog_agent.sh`
- 2 min: `tmux not installed; required by end-to-end tests`

Attempt 2:

- 2 min: `Go binary not installed`
- 1 min: `X11 dev headers (libX11-dev) not available without root; clipboard requires CGO`
- 1 min: `gawk (GNU Awk) required by core/nerdlog_agent.sh but not installed; mawk is the default`
- `tmux required by TestE2EScenarios but not installable`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
