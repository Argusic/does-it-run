# SoduWork

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mdiri-ai/SoduWork, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/soduwork

## Pinned environment

- Project commit: `5dd7fd91caea608d248d3fb6c8c78cf27a1b190e`
- Test commit: `5dd7fd91caea608d248d3fb6c8c78cf27a1b190e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 13.8 to 19.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 13.8 | 2 | 2 | [run](https://argusic.com/run/4891bb1a-cc15-4175-94b7-0241599f2989) |
| 2 | pass | 100 | 2 | 19.8 | 3 | 3 | [run](https://argusic.com/run/44dc0c0e-74ab-4b69-a33a-0028bc23cf0a) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 provided by Ubuntu 24.04 but the project requires v22.19+`
- 3 min: `Electron sandbox fails in container (need SUID chrome-sandbox owned by root with mode 4755)`

Attempt 2:

- 2 min: `Node.js 18.19.1 is installed but project requires 22.19+`
- `Desktop Electron client cannot start due to SUID sandbox helper not owned by root`
- `119 client tests fail from source checkout due to missing Pi SDK packages (@earendil-works/pi-coding-agent, @earendil-works/pi-ai)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
