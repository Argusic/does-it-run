# agent-workspace-linux

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/agent-sh/agent-workspace-linux, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/agent-workspace-linux

## Pinned environment

- Project commit: `0bc4c041d06a3d093f179e1a3bd8ba0f2d0be547`
- Test commit: `0bc4c041d06a3d093f179e1a3bd8ba0f2d0be547`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.3 to 14.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 14.3 | 3 | 3 | [run](https://argusic.com/run/7d5cf000-8368-4ce0-b964-8bb3f66db304) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `npm prebuilt binary requires GLIBC 2.43 but system has GLIBC 2.39`
- 3 min: `Missing openbox window manager and xdotool for workspace start`
- 1 min: `Test binary linking failed: rust-lld could not find -lxcb -lfreetype -lxkbcommon -lxkbcommon-x11`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
