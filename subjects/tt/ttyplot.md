# ttyplot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tenox7/ttyplot, licensed Apache-2.0, written in C.

Evidence and recordings: https://argusic.com/subject/ttyplot

## Pinned environment

- Project commit: `533a25e5194897befb8085bc11981f73f05b7368`
- Test commit: `533a25e5194897befb8085bc11981f73f05b7368`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.2 to 17.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 17.2 | 4 | 4 | [run](https://argusic.com/run/5f231590-85cd-424f-b138-eb8abcf7a9d2) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pkg-config: Package ncursesw not found (missing libncurses-dev headers)`
- 0.5 min: `make: ncurses.h not found (header needed for compilation)`
- 0.5 min: `make: VERSION_STR undeclared (not passed when bypassing pkg-config)`
- 8 min: `Runtime crash: "corrupted size vs. prev_size" heap corruption when piping stdin`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
