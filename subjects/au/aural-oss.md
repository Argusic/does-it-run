# aural-oss

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1146345502/aural-oss, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/aural-oss

## Pinned environment

- Project commit: `ff366fbf52f2adb15d288bd2ce659e925cbbaafc`
- Test commit: `ff366fbf52f2adb15d288bd2ce659e925cbbaafc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 11.3 to 11.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.5 | 11.3 | 2 | 2 | [run](https://argusic.com/run/41a432c0-0693-473f-a749-2b1bc981e027) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Node.js 18.x installed but project requires >=20.9`
- 0.5 min: `Playwright Chromium browser not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
