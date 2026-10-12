# beachpatrol

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/sebastiancarlos/beachpatrol, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/beachpatrol

## Pinned environment

- Project commit: `3b2666962f0507f0484c29e16a78cdc8b95152ac`
- Test commit: `3b2666962f0507f0484c29e16a78cdc8b95152ac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.1 to 6.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.8 | 6.1 | 3 | 3 | [run](https://argusic.com/run/82f9ab6f-ce73-4e5a-b932-c04015685d51) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Node.js v18.19.1 installed but project requires >=22.0.0`
- 1.5 min: `Chromium sandbox crash - container missing unprivileged user namespaces`
- 0.5 min: `playwright install-deps requires root for system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
