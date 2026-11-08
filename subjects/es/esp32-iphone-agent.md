# esp32-iphone-agent

**Verdict: runs.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/onehumanbeing/esp32-iphone-agent, licensed MIT, written in Swift.

Evidence and recordings: https://argusic.com/subject/esp32-iphone-agent

## Pinned environment

- Project commit: `680d22768ef6c67968c1663b99c9870c9c647ab2`
- Test commit: `680d22768ef6c67968c1663b99c9870c9c647ab2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 5.3 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 3.2 | 5.3 | 2 | 0 | [run](https://argusic.com/run/3551d3a7-6671-4ac7-9ada-2d58c2a37645) |
| 2 | pass | 100 | 6 | 6.6 | 1 | 1 | [run](https://argusic.com/run/407bf1d0-fa3b-43d5-9f6a-8ea48fd2c0f5) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Server startup: uxplay binary not found (legacy v0.1.0 dependency, needs system package not installable without root)`
- 0.1 min: `iOS app cannot be built on Linux (requires macOS with xcodebuild)`

Attempt 2:

- `server startup: uxplay binary not found (FileNotFoundError in screen.py _supervise)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
