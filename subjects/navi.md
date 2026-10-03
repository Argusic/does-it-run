# navi

**Verdict: runs.** Argusic Score 92.2 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/denisidoro/navi, licensed Apache-2.0, written in Rust.

Evidence and recordings: https://argusic.com/subject/navi

## Pinned environment

- Project commit: `f7330b9ad5bd95b7d1a3c96d00e0a77deb589147`
- Test commit: `f7330b9ad5bd95b7d1a3c96d00e0a77deb589147`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 21.6 to 27.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 88 | 1.3 | 27.2 | 5 | 4 | [run](https://argusic.com/run/14fd7692-5c38-47b1-83f2-21149cc6f52e) |
| 2 | pass | 100 | 60 | 25.7 | 6 | 6 | [run](https://argusic.com/run/782cea0e-cf06-458e-a2ab-fee1757ce715) |
| 3 | pass with mocks | 88.67 | 21 | 21.6 | 6 | 5 | [run](https://argusic.com/run/a4337071-4863-45e7-85af-fd7468184bf0) |

## What was observed on a clean machine

Attempt 1:

- 0.6 min: `No Rust toolchain installed`
- 0.2 min: `fzf binary not found`
- 0.3 min: `fzf requires a TTY for interactive selection, but no PTY was available`
- 0.1 min: `Shell helper function not found because BASH_ENV had unexpanded NAVI_HOME`
- `3rd party tests (tldr, cheatsh) and integration test (tmux) require external binaries not available`

Attempt 2:

- 10 min: `No Rust toolchain available`
- 3 min: `fzf missing , navi requires it for interactive selection`
- 5 min: `tmux missing , required by integration test`
- 2 min: `tealdeer missing , required for tldr integration`
- 2 min: `wget missing , required for cheat.sh integration`
- 5 min: `Interactive 3rd-party tests fail without a PTY (failed to open /dev/tty)`

Attempt 3:

- 10 min: `Rust toolchain not installed`
- 1 min: `fzf not installed`
- 1 min: `Bash tests need PTY (failed on /dev/tty)`
- 5 min: `tldr not installed (required for 3rd party test)`
- 1 min: `wget not installed (required for cheatsh integration)`
- `tmux not installed (required for integration test)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
