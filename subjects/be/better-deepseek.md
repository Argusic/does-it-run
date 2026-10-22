# better-deepseek

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/EdgeTypE/better-deepseek, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/better-deepseek

## Pinned environment

- Project commit: `c5449917276dd8053506d9f421ebe88cbf1336e4`
- Test commit: `c5449917276dd8053506d9f421ebe88cbf1336e4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.8 to 27.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 85.33 | 10 | 27.8 | 3 | 2 | [run](https://argusic.com/run/3301fdf0-94a6-44bc-af4c-df678ef68474) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Firefox binary present and no root to apt-install`
- 8 min: `Live MCP mock smoke hung on tools/call`
- 5 min: `No JDK: Android Gradle/Kotlin lane (android:test) cannot run in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
