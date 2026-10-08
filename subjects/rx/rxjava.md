# RxJava

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ReactiveX/RxJava, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/rxjava

## Pinned environment

- Project commit: `846acd6921acf906b1cc0e42c6cebf75b474744e`
- Test commit: `846acd6921acf906b1cc0e42c6cebf75b474744e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35 to 35 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 35 | 2 | 2 | [run](https://argusic.com/run/f82a7fde-65c3-40ac-a7de-de76e0c29c25) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Java JDK available in the container (no apt root, no pre-installed JDK)`
- 1 min: `Gradle requires Java 26 for compilation, Gradle itself needs a Java runtime`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
