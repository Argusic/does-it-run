# mesh

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gentics/mesh, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/mesh

## Pinned environment

- Project commit: `9ddc9bae48c5e8bba5fc0490d811c29a7f8d0cd6`
- Test commit: `9ddc9bae48c5e8bba5fc0490d811c29a7f8d0cd6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 34.5 to 34.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 34.5 | 4 | 4 | [run](https://argusic.com/run/52523b57-15fe-41ca-b99e-62fbc7fb775b) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `No Java or Maven pre-installed in container`
- 1 min: `Gentics Nexus repos (repo.gentics.com) return 401 Unauthorized; parent POM com.gentics:maven-parent:5.1.1 reference blocked`
- `Server requires database connector module (HSQLDB/MariaDB) on classpath via ServiceLoader; standalone JAR fails with 'Could not instantiate a database connector'`
- `Performance tests (7) error with NoMeshTestContextProvider , need running Mesh instance; index query counting tests (9) fail without Elasticsearch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
