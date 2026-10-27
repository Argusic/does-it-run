# umple

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/umple/umple, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/umple

## Pinned environment

- Project commit: `f721ae11a5598d9b2387f14c96df7ef5cb0242b6`
- Test commit: `f721ae11a5598d9b2387f14c96df7ef5cb0242b6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.4 to 44.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 96 | 38 | 44.4 | 5 | 4 | [run](https://argusic.com/run/88f0a4c6-605e-4223-896a-8fa6b9a39945) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `txl (TXL source transformation compiler) not installed on container; needed for Python codegen beta`
- 4 min: `Java 17 JDK not pre-installed in container`
- 2 min: `Apache Ant not pre-installed in container`
- 12 min: `Stable compiler jar (umple-1.37.1.8672.ffc0b7ae3) generates parser code referencing firstLineIndent and grammarResult attributes not declared in source .ump models`
- `Tests show 'Unable to locate umple file: dist/gradle/test/workingDir/...' failures (working directory mismatch) and expected-vs-actual warning code mismatches (901 vs 1510)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
