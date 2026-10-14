# lx-netease-music-mobile

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/souvenp/lx-netease-music-mobile, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/lx-netease-music-mobile

## Pinned environment

- Project commit: `e8c7ec1417a1bd5d302964903973f70cc1fd97e8`
- Test commit: `e8c7ec1417a1bd5d302964903973f70cc1fd97e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19 to 19 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1 | 19 | 3 | 3 | [run](https://argusic.com/run/f8159b17-c23b-44e8-be55-789ef399504d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Metro bundler OOM-killed with default settings (only 770MB RAM available)`
- `No JVM / Android SDK present in container; Gradle and APK build cannot run`
- `npm audit reports 59 vulnerabilities (1 low, 16 moderate, 40 high, 2 critical)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
