# deplao-builder

**Verdict: not yet verified.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/babyvibe/deplao-builder, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/deplao-builder

## Pinned environment

- Project commit: `2bbf8d693b24eaa9922b99ac269ad657fff9290f`
- Test commit: `2bbf8d693b24eaa9922b99ac269ad657fff9290f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 17.3 | 4.1 | 6 | 6 | [run](https://argusic.com/run/4d3af6fd-7bcb-45db-8fc0-0c8125e1976e) |

## What was observed on a clean machine

Attempt 1:

- `Node.js v18.19.1 is below the project's minimum requirement of Node 20+ for several dependencies (sharp, socks-proxy-agent, rcedit, etc.)`
- 2 min: `better-sqlite3 native module compiled for Node.js (NODE_MODULE_VERSION 108) not Electron v41 (NODE_MODULE_VERSION 145) , caused DB init failure on first launch`
- `Go >= 1.24 is not installed , E2EE bridge (fbchat-bridge-e2ee) cannot be built from source; prebuilt binary is Windows-only (.exe)`
- `electron-updater invoked in dev mode , app version '0.0' is not a valid semver, throws ERR_UPDATER_INVALID_VERSION`
- `dbus connection failures , D-Bus system bus socket missing in container`
- `No test files exist in the repository , jest config points to src/__tests__/*.test.ts which does not exist`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
