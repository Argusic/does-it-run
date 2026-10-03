# dbeaver

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dbeaver/dbeaver, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/dbeaver

## Pinned environment

- Project commit: `b59edd36ff94abfea48f5151a5ea10b3791137f0`
- Test commit: `b59edd36ff94abfea48f5151a5ea10b3791137f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 23 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 23 | 3 | 3 | [run](https://argusic.com/run/6aa7fb03-62cc-458e-b7c5-2c4c15db346b) |
| 2 | pass | 100 | 24 | 33 | 5 | 5 | [run](https://argusic.com/run/df188d40-5879-4536-8abf-35b92eccd88f) |
| 3 | pass | 100 | 27 | 27.8 | 7 | 7 | [run](https://argusic.com/run/e1b4919a-1c60-4c60-a0e7-2689d36fe215) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Java and Maven not pre-installed in container`
- 3 min: `Dependency repos dbeaver-common and datadam-api not present`
- 1 min: `Root POM parent relativePath pointed to ../dbeaver-common which didn't exist at that path`

Attempt 2:

- 3 min: `Missing Java 21 and Maven , neither was installed on the system`
- 2 min: `Sibling repos (dbeaver-common, datadam-api) not cloned , required by aggregate POM`
- 1 min: `Parent POM version mismatch , dbeaver root pom.xml referenced 2.8.0-SNAPSHOT, but dbeaver-common was 2.9.0-SNAPSHOT`
- 1 min: `Aggregate POM sibling paths (../../../dbeaver-common) resolved to /work/ which is not writable`
- 1 min: `Compilation failure: ApplicationCSSManager.java used removed API ExtendedDocumentCSS/getDocumentCSS (Eclipse 2026-09 dropped them)`

Attempt 3:

- 2 min: `Java 21 (JDK) not found in environment`
- 1 min: `Maven not found in environment`
- 3 min: `Missing dependency repositories dbeaver-common and datadam-api`
- 1 min: `Tycho 5.0.4 requires Maven >= 3.9.9 (had 3.9.8)`
- 1 min: `OSGi MANIFEST.MF Bundle-Version must use .qualifier suffix for SNAPSHOT builds`
- 1 min: `Aggregate POM module paths resolve to non-writable /work/ directory`
- 1 min: `datadam-api parent version mismatch (2.9.0-SNAPSHOT vs dbeaver's 2.8.0-SNAPSHOT)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
