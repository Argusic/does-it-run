# innodb-java-reader

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/alibaba/innodb-java-reader, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/innodb-java-reader

## Pinned environment

- Project commit: `9866b27eefdc61ed6f3282a68ce1948d462d6751`
- Test commit: `9866b27eefdc61ed6f3282a68ce1948d462d6751`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 5.7 to 5.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 5.7 | 3 | 3 | [run](https://argusic.com/run/ed850660-b358-4042-ae7d-91315ba01fc8) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `PMD violation: HashMap initialization without capacity in TableDefUtil.java`
- 0.5 min: `Java compilation error: 'bool' is not a valid type in InnodbReaderBootstrapTest.java`
- 0.5 min: `Java compilation error: void cannot be converted to boolean in InnodbReaderBootstrapTest.java`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
