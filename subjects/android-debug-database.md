# Android-Debug-Database

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/amitshekhariitbhu/Android-Debug-Database, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/android-debug-database

## Pinned environment

- Project commit: `bf149df61f03e7191f0a0cc71dfb2352f91173b2`
- Test commit: `bf149df61f03e7191f0a0cc71dfb2352f91173b2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11.2 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 13 | 14 | 5 | 5 | [run](https://argusic.com/run/2b6577a5-5a8a-4626-95fc-df15d7e6b530) |
| 2 | pass | 100 | 8 | 11.2 | 5 | 5 | [run](https://argusic.com/run/a14cfea6-d4a7-4367-838e-70ad43f2601d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Lint error in sample-app CarDBHelper.java: getColumnIndex can return -1 (Range)`
- 2 min: `Lint error in sample-app-encrypt CarDBHelper.java: getColumnIndex can return -1 (Range)`
- 1 min: `Lint error in sample-app-encrypt ContactDBHelper.java: getColumnIndex can return -1 (Range)`
- 1 min: `Lint error in sample-app-encrypt PersonDBHelper.java: getColumnIndex can return -1 (Range)`
- 1 min: `Lint error in sample-app ContactDBHelper.java: getColumnIndex can return -1 (Range)`

Attempt 2:

- 3 min: `Missing JDK - java command not found`
- 4 min: `Missing Android SDK - SDK location not found`
- 1 min: `lint error: getColumnIndex may return -1 in CarDBHelper.java (sample-app and sample-app-encrypt)`
- 0.5 min: `lint error: getColumnIndex may return -1 in ContactDBHelper.java (sample-app and sample-app-encrypt)`
- 0.5 min: `lint error: getColumnIndex may return -1 in PersonDBHelper.java (sample-app-encrypt)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
