# parse-dmarc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dmarcguardhq/parse-dmarc, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/parse-dmarc

## Pinned environment

- Project commit: `cb4a8b8ca6b5323aa80dd199a9e196de23e9f203`
- Test commit: `cb4a8b8ca6b5323aa80dd199a9e196de23e9f203`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 6 | 3 | 3 | [run](https://argusic.com/run/367e0319-f4cb-45fe-afc3-f38e9c211b36) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not found in container`
- 1 min: `bun not found in container`
- 1 min: `Node.js v18 too old (requires >=22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
