# mycompany

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lsfusion-solutions/mycompany, licensed Apache-2.0, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/mycompany

## Pinned environment

- Project commit: `e9d4c84858878249cd75beb07d76f83b38b679fb`
- Test commit: `e9d4c84858878249cd75beb07d76f83b38b679fb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 44.7 to 44.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29.1 | 44.7 | 4 | 4 | [run](https://argusic.com/run/cd0323c5-c5aa-450d-87c8-3daf323ac823) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No JDK or Maven installed - downloaded Amazon Corretto JDK 17.0.21 and Apache Maven 3.9.16`
- 3 min: `No PostgreSQL installed - extracted version 15.4 binaries from embedded-postgres-binaries Maven artifact`
- 2 min: `Corrupted commons-codec-1.11.jar on classpath caused 'zip END header not found' during server init`
- 3 min: `inotify max_user_instances=128 limit caused 'too many open files' error on subsequent server starts`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
