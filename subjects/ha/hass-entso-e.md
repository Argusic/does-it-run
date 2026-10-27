# hass-entso-e

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JaccoR/hass-entso-e, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hass-entso-e

## Pinned environment

- Project commit: `cbdf67ac0e73fd685a02e27ad7b6bef2c5af7ca6`
- Test commit: `cbdf67ac0e73fd685a02e27ad7b6bef2c5af7ca6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 40.4 to 40.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 45 | 40.4 | 4 | 4 | [run](https://argusic.com/run/74b0af70-5fb6-4d1c-a542-17f267467994) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `test_api_client.py used Windows-only backslash paths (..\, .\datasets\) and top-level relative import, so tests could not run on Linux`
- 6 min: `HA crash: aiodns 3.2.0 + pycares 5.2.1 TypeError Channel.getaddrinfo() on DNS resolution`
- 10 min: `HA default_config can not build/install C-extension deps (pyspeex-noise, netifaces, mutagen, libturbojpeg) because Python.h and system libs are missing without root`
- 8 min: `test_be_15M_avg failed: parser did not fill sparse 15-min period hours into hourly buckets (expected 36.30 at 00:00-02:00; got 38.94 and missing keys)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
