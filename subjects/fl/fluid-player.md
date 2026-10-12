# fluid-player

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fluid-player/fluid-player, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fluid-player

## Pinned environment

- Project commit: `026a61c8be3a58a5a0d38af5ca2fd4ff65ac1811`
- Test commit: `026a61c8be3a58a5a0d38af5ca2fd4ff65ac1811`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 32.3 to 41.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 41.5 | 0 | 0 | [run](https://argusic.com/run/d80afd0c-46f9-4352-abd0-a8aeba4e9ee3) |
| 2 | pass | 100 | 15 | 32.3 | 4 | 4 | [run](https://argusic.com/run/50de5ce3-3132-4b01-849c-ae276e66c35f) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `External video URLs (commondatastorage.googleapis.com) returned HTTP 403, blocking video playback in tests`
- 3 min: `webpack-dev-server crashed with EMFILE (too many open watched files)`
- 2 min: `Playwright Firefox could not connect to dev server (NS_ERROR_CONNECTION_REFUSED) due to IPv6/IPv4 mismatch`
- 5 min: `Firefox autoplay policy blocked video playback after ad transitions during midRoll test`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
