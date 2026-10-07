# yt-x

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Benexl/yt-x, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/subject/yt-x

## Pinned environment

- Project commit: `d7e30982ae13682fdf060055d9ba7dda598f4228`
- Test commit: `d7e30982ae13682fdf060055d9ba7dda598f4228`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 7.4 | 5 | 5 | [run](https://argusic.com/run/e0840e56-6687-472d-bb58-4bce36108d1c) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install yt-dlp failed: externally-managed-environment`
- 2 min: `fzf binary not found on system`
- 1 min: `mpv not installed; app refused playback`
- 2 min: `auto-update check blocks non-interactive use without TTY`
- 1 min: `youtube download requires sign-in (bot detection)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
