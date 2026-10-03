# yaak

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mountain-loop/yaak, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/yaak

## Pinned environment

- Project commit: `7f302536168585be4603aea09491a78b75c57070`
- Test commit: `7f302536168585be4603aea09491a78b75c57070`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 24 to 24 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 24 | 5 | 5 | [run](https://argusic.com/run/c225def5-2ebf-4789-8984-f2513730560c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Missing Rust toolchain`
- 1 min: `Node.js v18 too old (needs v24+)`
- 2 min: `libdbus-1-dev headers missing (libdbus-sys build failure)`
- 4 min: `Missing vendored plugin runtime and plugins for CLI build (include_str! failure)`
- 1 min: `Tauri desktop app requires WebKit2GTK dev libraries`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
