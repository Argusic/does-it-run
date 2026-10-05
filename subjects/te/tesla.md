# tesla

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elixir-tesla/tesla, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/tesla

## Pinned environment

- Project commit: `f1d040b237cf6fe07fc57d4915d95dca24546483`
- Test commit: `f1d040b237cf6fe07fc57d4915d95dca24546483`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.6 to 14.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 14.6 | 4 | 4 | [run](https://argusic.com/run/30c35389-b913-4609-bb47-592fb897e161) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Elixir/Erlang not installed in container`
- 3 min: `Erlang build requires ncurses-dev (curses functions not found)`
- 1 min: `unzip command not found for Elixir precompiled zip`
- 1 min: `.tool-versions had imprecise versions (1.19-otp-28, 28.5) vs installed (1.19.6-otp-28, 28.5.0.7)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
