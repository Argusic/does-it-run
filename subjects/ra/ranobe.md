# ranobe

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ranobe-org/ranobe, licensed Unlicense, written in Java.

Evidence and recordings: https://argusic.com/subject/ranobe

## Pinned environment

- Project commit: `ec707199fbb82fe8039b727a82e6428c46c7a484`
- Test commit: `ec707199fbb82fe8039b727a82e6428c46c7a484`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 6.9 to 8.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 6.9 | 1 | 1 | [run](https://argusic.com/run/99dc860e-e29d-4784-8e35-4ba5a3d8ffe6) |
| 2 | fail | 80 | 7 | 8.5 | 2 | 2 | [run](https://argusic.com/run/5ec8e8d2-44f8-470e-b8c4-c7c0d5447583) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `downloader module referenced in settings.gradle but directory does not exist`

Attempt 2:

- 1 min: `settings.gradle included ":downloader" module that does not exist as a directory, causing Gradle sync failure`
- 1 min: `downloader product flavor fails to compile because ChapterUpdateScheduler class referenced from main source set is missing in downloader flavor source set`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
