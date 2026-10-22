# jafka

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/adyliu/jafka, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/jafka

## Pinned environment

- Project commit: `a8500130130ae22087fbcb5c9e605ee1dfd824c1`
- Test commit: `a8500130130ae22087fbcb5c9e605ee1dfd824c1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.7 to 8.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 8.7 | 2 | 2 | [run](https://argusic.com/run/203c93ec-8736-4f53-8da3-566dfc4d7646) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No JDK or Maven in container , downloaded OpenJDK 11 and Apache Maven 3.8.8`
- 0.5 min: `jackson-core 2.9.8 incompatible with jackson-databind 2.12.6.1 , ClassNotFoundException: JacksonFeature`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
