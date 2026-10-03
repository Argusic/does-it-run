# App-Store-Connect-CLI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rorkai/App-Store-Connect-CLI, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/app-store-connect-cli

## Pinned environment

- Project commit: `6d4943bd8830bdf1c8888859ee166989d2b9f24c`
- Test commit: `6d4943bd8830bdf1c8888859ee166989d2b9f24c`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 3; wall time 11.1 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 14 | 1 | 1 | [run](https://argusic.com/run/e491db65-1c8f-4fbb-a71e-a7351a1025e6) |
| 2 | pass with mocks | 92 | 15 | 11.8 | 0 | 0 | [run](https://argusic.com/run/c278ffcf-ace4-4a06-af8d-5550f5498446) |
| 3 | pass with mocks | 92 | 8 | 11.1 | 0 | 0 | [run](https://argusic.com/run/ee7e7508-7000-4199-b4b1-f9759fb1bc9b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `make not installed: 6 TestMake* tests skipped because 'make' binary is not on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
