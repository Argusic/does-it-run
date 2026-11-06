# firebase-ios-sdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/firebase/firebase-ios-sdk, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/firebase-ios-sdk

## Pinned environment

- Project commit: `e97426fc20f7b2bdd74c5a69c98391727407f3c4`
- Test commit: `e97426fc20f7b2bdd74c5a69c98391727407f3c4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 26.3 to 54.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 51.8 | 54.3 | 1 | 1 | [run](https://argusic.com/run/7a01185c-647f-4a65-a649-2095880f9030) |
| 2 | pass | 100 | 34 | 26.3 | 5 | 5 | [run](https://argusic.com/run/d75818c0-e480-474a-bec1-8750711704cc) |

## What was observed on a clean machine

Attempt 1:

- 11.5 min: `GCC 13 false-positive -Werror=maybe-uninitialized on Firestore/core/src/core/query.cc:319 causing build failure at 93%`

Attempt 2:

- 5 min: `Go missing, CMake configure failed`
- 1 min: `pip install --user six blocked (PEP 668 externally-managed environment)`
- 6 min: `Firestore emulator v1.20.2 requires Java 21+ (class file version 65.0)`
- 2 min: `make -j4 fails on shared-memory jobserver IPC in this container`
- 1 min: `Emulator stop left stale PID file because the process had already exited`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
