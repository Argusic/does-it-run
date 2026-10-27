# dataCompare

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dromara/dataCompare, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/datacompare

## Pinned environment

- Project commit: `906df90c8d881f5a6ff9dcb819578e1a8eb022c8`
- Test commit: `906df90c8d881f5a6ff9dcb819578e1a8eb022c8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 23.5 to 23.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 14 | 23.5 | 3 | 3 | [run](https://argusic.com/run/2fe3f79c-560a-43ea-84aa-6ea79c4681eb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `XqTest.java had unclosed Javadoc comment preventing test compilation`
- 5 min: `No MySQL/MariaDB available for database initialization`
- 8 min: `No Java/Maven runtime in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
