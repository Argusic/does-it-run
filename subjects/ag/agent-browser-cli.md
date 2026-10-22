# agent-browser-cli

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sleepinginsummer/agent-browser-cli, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/agent-browser-cli

## Pinned environment

- Project commit: `ce9a70c79ba064dd5c83d76205c849f11318c683`
- Test commit: `ce9a70c79ba064dd5c83d76205c849f11318c683`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.6 to 34.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 34 | 34.6 | 6 | 6 | [run](https://argusic.com/run/7afa98a3-8241-4f21-8f69-ff5adcf2854f) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npm global install failed with EACCES on /usr/local`
- 8 min: `hand-rolled WebSocket mock closed right after handshake`
- 9 min: `standalone mock exited after ~40s due to its own read timeout`
- 4 min: `scan --text-only returned empty content`
- 9 min: `click/fill/send-keys on @e refs: Runtime.callFunctionOn response missing value`
- 2 min: `mouse-click could not verify: element has no layout box`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
