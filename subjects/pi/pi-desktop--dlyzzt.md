# pi-desktop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DLYZZT/pi-desktop, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/run/2e41f200-0059-49b8-99bf-f0fd995f3cf3

## Pinned environment

- Project commit: `b05fbd40345d2bd74f7da6b66d1cfc64d867fefa`
- Test commit: `b05fbd40345d2bd74f7da6b66d1cfc64d867fefa`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.1 to 11.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 11.1 | 4 | 4 | [run](https://argusic.com/run/2e41f200-0059-49b8-99bf-f0fd995f3cf3) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18 in container, project requires >=22.19`
- 0.5 min: `Electron SUID sandbox helper not configured for unprivileged container`
- 2 min: `Smoke test failed on files.index (search-unavailable)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
