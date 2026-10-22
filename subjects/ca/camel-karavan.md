# camel-karavan

**Verdict: could not verify.** Argusic Score 35 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/camel-karavan, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/camel-karavan

## Pinned environment

- Project commit: `ad0147f49200c0be7843ce7ee3995d416ca04714`
- Test commit: `ad0147f49200c0be7843ce7ee3995d416ca04714`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.8 to 26.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 29 | 26.4 | 3 | 3 | [run](https://argusic.com/run/db5dd4c9-2e8c-4795-a5ac-625dede7d1ac) |
| 2 | fail | 20 | n/a | 9.8 | 0 | 0 | [run](https://argusic.com/run/9c7d9802-9c40-42ff-81d2-0623acd2aa11) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java runtime installed`
- 2 min: `karavan-app pom.xml requires Java 25 but JDK 17 was initially used`
- 1 min: `No root access; cannot install system packages via apt`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
