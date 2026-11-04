# quartz

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jackyzha0/quartz, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/quartz

## Pinned environment

- Project commit: `97a2d05f80c4c50534959b1d0d41cc4b3895625e`
- Test commit: `97a2d05f80c4c50534959b1d0d41cc4b3895625e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.5 to 4.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.5 | 0 | 0 | [run](https://argusic.com/run/3e0d1890-7f5b-4b9b-b25a-e45ce15c1831) |
| 2 | pass | 100 | 3 | 4.2 | 1 | 1 | [run](https://argusic.com/run/7ed6d3a2-bbc7-4166-a6e4-ff1585085964) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Node.js v18 (needs >=22) and npm 9.2 (needs >=10.9.2) in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
