# HomeSpan

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HomeSpan/HomeSpan, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/homespan

## Pinned environment

- Project commit: `107ffc07f4455754ea89068d8cf2e992de3583e6`
- Test commit: `107ffc07f4455754ea89068d8cf2e992de3583e6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 37.2 to 63.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 62 | 63.1 | 3 | 3 | [run](https://argusic.com/run/061bbd02-cec1-46ac-928f-d25ceb8f28a9) |
| 2 | pass with mocks | 92 | 18 | 37.2 | 4 | 4 | [run](https://argusic.com/run/980109bd-eb54-4975-a9f4-ffb42c71ee63) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Out of disk space (7.4GB/7.8GB used) during ESP32 core toolchain install`
- 1 min: `Default ESP32 partition scheme provides only 1.3MB APP space; HomeSpan sketches exceed it (107% full)`
- 1 min: `arduino-cli not available in environment`

Attempt 2:

- 3 min: `No Arduino tooling installed in container`
- 2 min: `PlatformIO project not initialized`
- 10 min: `Arduino-ESP32 core 2.0.17 too old for HomeSpan 2.1.8 (needs >=3.3.0)`
- 2 min: `Firmware (1.6MB) exceeds default 1.3MB partition`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
