# DSHA

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/DSH-APP/DSHA, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/dsha

## Pinned environment

- Project commit: `bdb647c331c4d6c11b5632afdb901c50510720ea`
- Test commit: `bdb647c331c4d6c11b5632afdb901c50510720ea`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.3 to 17.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 16 | 17.3 | 2 | 1 | [run](https://argusic.com/run/f4ae3651-66b1-4fd4-af00-44017d1939c5) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Gradle Android build requires full SDK license acceptance and asset generation (dsh-runtime.bin, offline-rootfs.tar.gz, etc.) that depend on CI tooling`
- 8 min: `AGP 9.1+s Android SDK license acceptance files require exact SHA-1 hash naming matching the license text in repository2-3.xml, which was resolved after debugging the hash computation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
