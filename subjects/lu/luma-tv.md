# luma-tv

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/0xProbabillity/luma-tv, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/luma-tv

## Pinned environment

- Project commit: `8ce68387cb690786445ffde8d1d1776d07fb6997`
- Test commit: `8ce68387cb690786445ffde8d1d1776d07fb6997`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.9 to 4.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 12 | 4.9 | 4 | 3 | [run](https://argusic.com/run/6212ea27-eef8-4562-9543-f6f9109b324c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `java/javac not found (JDK absent in container)`
- 3 min: `Android SDK absent (no aapt2/d8/apksigner/build-tools 36.0.0, no android-34)`
- 2 min: `build.sh: line 31: zip: command not found`
- `No adb and no Android TV/device/emulator in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
