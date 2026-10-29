# miu

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kenjinote/miu, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/miu

## Pinned environment

- Project commit: `28f44b02e35eb6b9b2bf39551d61b62e4d8906df`
- Test commit: `28f44b02e35eb6b9b2bf39551d61b62e4d8906df`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.2 to 7.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 4 | 7.2 | 2 | 0 | [run](https://argusic.com/run/3d6c53bc-376b-4497-9d2e-3e74feb1d261) |

## What was observed on a clean machine

Attempt 1:

- `Main app miu cannot build on Linux - it targets only Windows (Win32 API), macOS (CoreFoundation), iOS/iPadOS, and Android (Android NDK). No Linux build target exists in the project.`
- `2 of 8 CED unittests fail on Linux (EasyTests and UTF8UTF8Tests): encoding detection returns CP1252 (63) instead of expected UTF8 (22) due to platform locale differences`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
