# xiadown

**Verdict: not yet verified.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arnoldhao/xiadown, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/xiadown

## Pinned environment

- Project commit: `c8e33101987f123dd8d8504a3ec15bd296d69e13`
- Test commit: `c8e33101987f123dd8d8504a3ec15bd296d69e13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 46.5 to 46.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 22 | 46.5 | 6 | 6 | [run](https://argusic.com/run/38fd2d8c-1ff5-4b14-b7eb-44fb192b9c23) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25.12+ not found`
- 1 min: `Bun not found`
- 5 min: `go-json-experiment/json@v0.0.0-20251027170946 fails to build: references json.SkipFunc and json.DiscardUnknownMembers not in std encoding/json`
- `Missing system dev libraries (glib-2.0, gtk4, webkitgtk-6.0, libsoup-3.0, gio-2.0)`
- `IPv6 loopback [::1] unavailable in container`
- `Missing frontend bindings (bindings/ empty) and Wails CLI`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
