# GoAnime

**Verdict: runs.** Argusic Score 92.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alvarorichard/GoAnime, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/goanime

## Pinned environment

- Project commit: `85258f7b483064e428b0797955e320c152c8a7ea`
- Test commit: `85258f7b483064e428b0797955e320c152c8a7ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 42.6 to 63.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 35 | 63.8 | 2 | 2 | [run](https://argusic.com/run/f3deace4-e6c4-412b-97e8-ef16e5fea995) |
| 2 | pass with mocks | 85.33 | 42 | 42.6 | 3 | 2 | [run](https://argusic.com/run/18a540c2-d715-4137-afb5-269ea1c0e7ce) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go binary not found in container (Go 1.27.1 required but not installed)`
- 10 min: `TestPlaywrightHelpers/hide_then_reveal_moves_the_solver_window failed: CDP minimize requires a window manager; Xvfb alone provides none`

Attempt 2:

- 1 min: `Go 1.27 not found in container`
- 18 min: `Test TestPlaywrightHelpers/hide_then_reveal failed: CDP minimize does not work on Xvfb without a window manager`
- 2 min: `mpv runtime dependency not installed (no root access)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
