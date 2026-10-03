# trueforge

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/truefoundry/trueforge, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/trueforge

## Pinned environment

- Project commit: `0fe346a7cb09396f71f0a797706209d84b350efb`
- Test commit: `0fe346a7cb09396f71f0a797706209d84b350efb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 71.1 to 71.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 13 | 71.1 | 4 | 0 | [run](https://argusic.com/run/49ff508f-a9e9-4ed0-8969-8b3539a96b30) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Frontend (Vite + Monaco editor) build OOM in ~2GB container`
- `3 trueforge test suites OOM-killed (trueFoundryNaming, perServerMcpHeaders, schedule)`
- `TrueForge UI test suite partially OOM-killed with some pre-existing test failures`
- `Local sandbox unavailable: bubblewrap, socat not installed (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
