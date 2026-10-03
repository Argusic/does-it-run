# smart-admin

**Verdict: could not verify.** Argusic Score 70 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/1024-lab/smart-admin, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/smart-admin

## Pinned environment

- Project commit: `2dbf3c285afbb187efb19630c4dd70664067cbc2`
- Test commit: `2dbf3c285afbb187efb19630c4dd70664067cbc2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 18 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 5.2 | 18 | 1 | 1 | [run](https://argusic.com/run/ada08e82-a9dd-4621-91e7-5f49ff14d0c5) |
| 2 | fail | 60 | 20 | 20.2 | 1 | 0 | [run](https://argusic.com/run/92b6613a-003b-4a64-a2f5-7b76bc2eca24) |

## What was observed on a clean machine

Attempt 1:

- `Java/Maven not available; backend (spring-boot) projects cannot be built or launched`

Attempt 2:

- `Java (JDK/Maven) not available in container , cannot build or run the Java backend modules (smart-admin-api-java17-springboot3, smart-admin-api-java8-springboot2) or execute the Java test class AdminApplicationTest.java`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
