# google-images-download

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hardikvasa/google-images-download, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/google-images-download

## Pinned environment

- Project commit: `9057dad76ce4bcdd20e9c332f4172ecb7c6c0559`
- Test commit: `9057dad76ce4bcdd20e9c332f4172ecb7c6c0559`
- Worker image digest: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 13.1 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 27 | 26.6 | 6 | 6 | [run](https://argusic.com/run/3e8c719e-f2ab-40bb-b17e-dfb3afc9cd32) |
| 2 | fail | 80 | 9 | 13.1 | 1 | 1 | [run](https://argusic.com/run/fe2ac484-cef2-400e-bbde-7f15e7c513e0) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No pip available in base container - installed via get-pip.py with --break-system-packages`
- 5 min: `No Chrome/Chromium browser installed in container`
- 8 min: `Missing system shared libraries for Chrome (libglib2.0, libnss3, libxcb, etc.)`
- 3 min: `Missing fontconfig and fonts causing Chrome crash on HTTPS pages`
- 3 min: `Chrome binary path not configurable in source code - added --chrome_bin argument and CHROME_BIN env var support`
- 4 min: `Google returns CAPTCHA to headless Chrome from container IP - cannot download actual images`

Attempt 2:

- 5 min: `No Chromium/Chrome browser available in container (no root access to apt, snap not available). Selenium-based download tests cannot execute.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
