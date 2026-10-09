# splash

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/incoai/splash, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/splash

## Pinned environment

- Project commit: `c64a578fcfaa059023a2ca57230d4aead134b73b`
- Test commit: `c64a578fcfaa059023a2ca57230d4aead134b73b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 24.8 to 34 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 14.5 | 24.8 | 4 | 4 | [run](https://argusic.com/run/ea20fe38-b351-4d6b-a506-5d329db2cc9d) |
| 2 | pass with mocks | 92 | 1 | 34 | 4 | 4 | [run](https://argusic.com/run/aeb31795-79bb-46ab-a15b-ea8c8bc6f9c3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `xcrun not found (no macOS SDK/Xcode on Linux x86_64); native C++/Metal binary cannot compile`
- 1 min: `lockf not found (macOS utility) , test_makefile fails on Linux`
- 1 min: `pip install blocked by externally-managed-environment`
- 3 min: `Test isolation issues , several suites hang when run as complete suites due to pre-existing patching conflicts`

Attempt 2:

- `Native Metal engine requires macOS (Apple Silicon) + Xcode`
- `test_package.py: 13 failures - Apple Silicon check in install.sh`
- `test_makefile.py: 3 failures - requires xcrun and lockf (macOS)`
- `test_build_identity.py: 1 failure - requires xcrun`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
