# fscrawler

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dadoonet/fscrawler, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/fscrawler

## Pinned environment

- Project commit: `8b4db8435639daf83f52d887c5e88c937e4efb88`
- Test commit: `8b4db8435639daf83f52d887c5e88c937e4efb88`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 26.7 to 81.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 26.7 | 0 | 0 | [run](https://argusic.com/run/316f1362-22b7-42a1-ba28-f45a363e6c77) |
| 2 | pass | 100 | 55 | 81.5 | 2 | 2 | [run](https://argusic.com/run/908b45a6-196b-4c10-a1a1-814233bb4d78) |

## What was observed on a clean machine

Attempt 2:

- 25 min: `Default test discovery via 'mvn test -DskipIntegTests' reports Tests run: 0 across all modules due to RepeatExecutionTestEngine from randomizedtesting-jupiter interfering with surefire discovery`
- `FsSshPluginTest expects hardcoded file permission bits (33188/16877) but OS returns different values (33204/16893)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
