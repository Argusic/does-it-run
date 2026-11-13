# pg-aiguide

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/timescale/pg-aiguide, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pg-aiguide

## Pinned environment

- Project commit: `b236d3583fb51f5ef009d2c95d4fc361df748280`
- Test commit: `b236d3583fb51f5ef009d2c95d4fc361df748280`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 2.5 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 3 | 6.3 | 2 | 1 | [run](https://argusic.com/run/9dfa9272-50f8-4fa3-ad32-b61e2029c33a) |
| 2 | pass with mocks | 92 | 1 | 2.5 | 0 | 0 | [run](https://argusic.com/run/613514a3-4021-4797-a8c7-7f215578cea5) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `The ./bun wrapper script tried to download bun via curl|bash but 'unzip' is not available in the container, so the download step failed silently`
- `PostgreSQL is not installed; apt-get requires root which is not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
