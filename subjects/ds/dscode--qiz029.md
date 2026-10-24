# dscode

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/qiz029/dscode, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/run/d2cef4c8-824a-4175-8b0e-7916d01c239a

## Pinned environment

- Project commit: `2a94518ee0a50b6a63d70c4d5987c61efaf63988`
- Test commit: `2a94518ee0a50b6a63d70c4d5987c61efaf63988`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 12.8 to 12.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 12.8 | 4 | 4 | [run](https://argusic.com/run/d2cef4c8-824a-4175-8b0e-7916d01c239a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js v18.19.1 present, project requires ^22.19.0 || >=24.0.0`
- 1 min: `npm ci failed: lockfile out of sync with package.json (dev checkout, not a release tarball)`
- 1 min: `TUI requires real TTY for Ink raw mode , cannot launch in headless container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
