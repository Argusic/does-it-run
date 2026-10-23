# tms

**Verdict: runs.** Argusic Score 97.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xiweicheng/tms, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/tms

## Pinned environment

- Project commit: `d50a870a876c3517ccc97223795dca196a8b3c0e`
- Test commit: `d50a870a876c3517ccc97223795dca196a8b3c0e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.6 to 15.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 97.14 | 17 | 15.6 | 7 | 6 | [run](https://argusic.com/run/8561d2b8-6d41-4fe0-9508-53560870744a) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Java 8 (javac/java) not found in environment`
- 1 min: `Maven (mvn) not found in environment`
- 6 min: `MySQL not available , no mysqld or docker`
- 1 min: `spring.profiles.active invalid in profile-specific test properties file (SB 2.4+ regression)`
- 1 min: `Missing tms.blog.md2pdf.path placeholder in test config`
- 1 min: `SecurityConfig @Profile excluded test profile; test context loaded with no security`
- `6 pre-existing test failures due to hardcoded /Users/xiweicheng/temp/ paths and missing test2.docx on classpath , cannot create /Users without root`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
