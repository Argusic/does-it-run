# tableau

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elixir-tools/tableau, licensed MIT, written in Elixir.

Evidence and recordings: https://argusic.com/subject/tableau

## Pinned environment

- Project commit: `6a6c89430113eee6b5fc5aa3140b7c9d034661d7`
- Test commit: `6a6c89430113eee6b5fc5aa3140b7c9d034661d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.9 to 7.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 7.9 | 4 | 4 | [run](https://argusic.com/run/98c8a8ba-949a-463e-81c7-d294c3044bf1) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `No Elixir/Erlang runtime in container`
- 0.3 min: `ncurses-dev headers/libs missing from system`
- 0.2 min: `Erlang configure: CFLAGS missing -O flag after adding include path`
- 0.1 min: `libtinfo.so symlink broken in extracted .deb`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
