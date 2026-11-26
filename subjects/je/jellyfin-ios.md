# jellyfin-ios

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jellyfin/jellyfin-ios, licensed MPL-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/jellyfin-ios

## Pinned environment

- Project commit: `84bf59e1ebac7b851e1745aed49842c85f021824`
- Test commit: `84bf59e1ebac7b851e1745aed49842c85f021824`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.4 to 8.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1 | 7.4 | 0 | 0 | [run](https://argusic.com/run/413707a0-bb65-4573-adae-5a145babed8a) |
| 2 | pass | 100 | 1 | 8.8 | 1 | 1 | [run](https://argusic.com/run/81fcac72-e33d-47fe-8b5d-69358f140416) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Node.js version mismatch: .nvmrc specifies 20 but container has Node 18.19.1; engine-strict=true in .npmrc blocked npm install`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
