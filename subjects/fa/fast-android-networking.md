# Fast-Android-Networking

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amitshekhariitbhu/Fast-Android-Networking, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/fast-android-networking

## Pinned environment

- Project commit: `508e7c5b4338591b2f42bb6e526cfd3f0b8f8ed7`
- Test commit: `508e7c5b4338591b2f42bb6e526cfd3f0b8f8ed7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.9 to 23.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 23 | 23.9 | 4 | 4 | [run](https://argusic.com/run/4a6b0d59-f946-4e81-93c8-6571f3d8eaf3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK available in container`
- 3 min: `No Android SDK available`
- 5 min: `No KVM hardware acceleration available`
- `ARM system images not supported by QEMU2 emulator`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
