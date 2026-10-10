# opencode-telegram-bot

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/grinev/opencode-telegram-bot, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/opencode-telegram-bot

## Pinned environment

- Project commit: `fac8c99ed8213d8a669a4cb2c864e97e6a5c613b`
- Test commit: `fac8c99ed8213d8a669a4cb2c864e97e6a5c613b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 16.3 | 3 | 3 | [run](https://argusic.com/run/5256c496-b260-4802-b9c1-31898c09c1e8) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 is below the required ^22.14.0; npm install succeeded with EBADENGINE warnings but vitest failed at startup ('node:util' does not export 'styleText')`
- 5 min: `Container has /.dockerenv, making isContainerRuntime() return true in production code. Five test files (open, worktree, opencode-start, opencode-stop, auto-restart) did not mock isContainerRuntime, so commands returned 'not available in Doc`
- `4 e2e forward-proxy tests fail (socks, socks5, socks5h, http) trying to connect to IPv6 loopback ::1 , IPv6 loopback is not reachable in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
