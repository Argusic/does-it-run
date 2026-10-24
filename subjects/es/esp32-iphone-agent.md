# esp32-iphone-agent

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/onehumanbeing/esp32-iphone-agent, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/esp32-iphone-agent

## Pinned environment

- Project commit: `680d22768ef6c67968c1663b99c9870c9c647ab2`
- Test commit: `680d22768ef6c67968c1663b99c9870c9c647ab2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 5.3 to 5.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 3.2 | 5.3 | 2 | 0 | [run](https://argusic.com/run/3551d3a7-6671-4ac7-9ada-2d58c2a37645) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Server startup: uxplay binary not found (legacy v0.1.0 dependency, needs system package not installable without root)`
- 0.1 min: `iOS app cannot be built on Linux (requires macOS with xcodebuild)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
