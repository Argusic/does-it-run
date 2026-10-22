# lazyspotify

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dubeyKartikay/lazyspotify, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/lazyspotify

## Pinned environment

- Project commit: `4fc759a1a7b244ebf7c1f355627de74d97ed6c2f`
- Test commit: `4fc759a1a7b244ebf7c1f355627de74d97ed6c2f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 18.7 to 18.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 18.7 | 3 | 3 | [run](https://argusic.com/run/8ac1ac83-36b1-4e0a-b957-0a351683ff11) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `go toolchain absent (go: not found)`
- 1 min: `TUI would not start: bubbletea could not open /dev/tty`
- 1 min: `OAuth callback with bad code yields 403 + exit (expected auth-failure path, verified against real accounts.spotify.com)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
