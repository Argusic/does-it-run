# TUI-ConsoleLauncher

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fandreuz/TUI-ConsoleLauncher, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/tui-consolelauncher

## Pinned environment

- Project commit: `058f54116c4125ee72732a31d0f83e58c30534ad`
- Test commit: `058f54116c4125ee72732a31d0f83e58c30534ad`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.2 to 10.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 10.7 | 10.9 | 3 | 3 | [run](https://argusic.com/run/019aa47c-cbb7-4c0e-b7b2-04cafbee2d68) |
| 2 | fail | 80 | 8 | 9.2 | 3 | 3 | [run](https://argusic.com/run/0fde8bba-10ef-4547-b1e5-4778a0cd5899) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java runtime found`
- 4.5 min: `Android SDK not found (ANDROID_HOME not set, no sdk.dir)`
- 0.5 min: `Missing signing keystore release.jks`

Attempt 2:

- 2 min: `No Java runtime available`
- 4 min: `Android SDK not found`
- 1 min: `Missing signing keystore for debug builds`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
