# iwf

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/indeedeng/iwf, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/iwf

## Pinned environment

- Project commit: `ad3d109fd9d8093da94d5c77aaba888d6490cbdc`
- Test commit: `ad3d109fd9d8093da94d5c77aaba888d6490cbdc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.3 to 16.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 16 | 16.3 | 6 | 6 | [run](https://argusic.com/run/dabd25a2-8506-4f33-b06f-9fee6cea7b28) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.24 not installed in container`
- 4 min: `S3/MinIO endpoint refused on port 9000`
- 2 min: `Temporal dev server kept dying after backgrounding`
- 1 min: `iWF could not reach Temporal after session exit`
- 1 min: `iWF could not connect to Temporal due to IPv6 resolution of localhost`
- 1 min: `Workflow start returned 500 due to missing search attributes`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
