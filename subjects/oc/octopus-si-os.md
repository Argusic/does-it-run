# Octopus-SI-OS

**Verdict: runs with mocks.** Argusic Score 78.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/miuuyy/Octopus-SI-OS, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/octopus-si-os

## Pinned environment

- Project commit: `7e56e315ad2cd5dd554e7797193aa224d81d4fac`
- Test commit: `7e56e315ad2cd5dd554e7797193aa224d81d4fac`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 26.9 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 78.67 | 15 | 26.9 | 3 | 1 | [run](https://argusic.com/run/ec2f5a4f-0aaf-4471-b49e-12d874fe7552) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing ALSA development headers for Rust build`
- `4 octopus-app-server tests fail on Linux (missing tesseract OCR binary and macOS process-authority sandbox backend)`
- `doomsday framework round-trip test fails on Linux (same sandbox gap)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
