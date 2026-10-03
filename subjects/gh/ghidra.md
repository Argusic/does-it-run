# ghidra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NationalSecurityAgency/ghidra, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/ghidra

## Pinned environment

- Project commit: `04c4a202939a2686c95731dc9ffde9ae4233cccf`
- Test commit: `04c4a202939a2686c95731dc9ffde9ae4233cccf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 22.1 to 45.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 22.1 | 0 | 0 | [run](https://argusic.com/run/e46f4f09-2bf7-4a94-b8e1-8e3ead9baded) |
| 2 | pass | 100 | 18 | 45.6 | 1 | 1 | [run](https://argusic.com/run/bd3b9c49-045c-40bc-964a-db63b538d9e1) |
| 3 | pass | 100 | 34 | 36.7 | 3 | 3 | [run](https://argusic.com/run/96594b89-ab82-44ec-a6f5-bd02392b2cf7) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `:Base:test Gradle task failed with java.nio.file.NoSuchFileException on binary results file (Gradle infrastructure issue). All 2584 tests individually passed in logs.`

Attempt 3:

- 2 min: `No JDK found in environment`
- 2 min: `Build failed: invalid source release 25 when using JDK 21`
- `ghidraRun scripts had no execute permission after zip extraction`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
