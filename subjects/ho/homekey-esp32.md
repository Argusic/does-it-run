# HomeKey-ESP32

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rednblkx/HomeKey-ESP32, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/homekey-esp32

## Pinned environment

- Project commit: `2514b364406820bbe07b619bb5a84a1d1663850f`
- Test commit: `2514b364406820bbe07b619bb5a84a1d1663850f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 19.9 to 19.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 19.9 | 4 | 4 | [run](https://argusic.com/run/e726e4d7-5f28-42aa-85c9-a6327dc1bc0c) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `ESP-IDF toolchain not installed`
- 2 min: `bun not found on PATH (needed for web UI build)`
- 2 min: `Node.js v18 too old for Vite 8 (requires 20.19+)`
- 1 min: `Dependency cache error for lan86xx_common component`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
