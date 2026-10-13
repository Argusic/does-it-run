# litiengine

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gurkenlabs/litiengine, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/litiengine

## Pinned environment

- Project commit: `ce91406988d92ab9b3b1950e7fcf66f80c5821f6`
- Test commit: `ce91406988d92ab9b3b1950e7fcf66f80c5821f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 14.4 to 14.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 14.4 | 2 | 2 | [run](https://argusic.com/run/61259354-1786-4734-8c47-c880edb7340f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `JDK 25 not installed`
- `No Gradle on PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
