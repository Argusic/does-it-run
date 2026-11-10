# netbeans

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/netbeans, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/netbeans

## Pinned environment

- Project commit: `4d2a85c0e27052ba3f66a868748b7e93859a6fb6`
- Test commit: `4d2a85c0e27052ba3f66a868748b7e93859a6fb6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 30.8 to 38.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 27 | 30.8 | 2 | 2 | [run](https://argusic.com/run/477a7c2b-634f-4e56-ac2a-60485d8a7517) |
| 2 | fail | 80 | 37 | 38.1 | 3 | 3 | [run](https://argusic.com/run/13d9c32f-b6ef-4ca2-bb8c-362997221992) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `JDK 21+ not installed in container`
- 1 min: `Apache Ant not installed in container`

Attempt 2:

- 5 min: `JDK 21 and Apache Ant not found in container; had to download and install both from Adoptium/Temurin and Apache mirrors (no root access for apt)`
- 1 min: `First JDK download (143MB) was truncated; tar extraction failed with 'unexpected end of file'`
- 15 min: `Full test suite (test-platform, commit-validation, all-nozip, test-basic) all timed out producing no visible output after 5+ minutes each; test harness uses 'subant' which runs jUnit tests inside the full IDE, each module one at a time, tak`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
