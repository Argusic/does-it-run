# ghidra-mcp

**Verdict: runs.** Argusic Score 89 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bethington/ghidra-mcp, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/ghidra-mcp

## Pinned environment

- Project commit: `1e0211388d9fc1f85876b69b3343d1bd563c3b85`
- Test commit: `1e0211388d9fc1f85876b69b3343d1bd563c3b85`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 3.2 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 87 | 4 | 8.9 | 4 | 3 | [run](https://argusic.com/run/1201b327-5eef-4e1b-8636-22c2e33110d7) |
| 2 | pass | 100 | 3 | 3.2 | 2 | 2 | [run](https://argusic.com/run/7cf27e1a-c0ef-41f2-8cdc-38c859cb0883) |
| 3 | pass | 80 | 0.25 | 5.5 | 1 | 0 | [run](https://argusic.com/run/4de99dc5-936e-4889-9dbf-5ac7965de483) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `uv not installed`
- 2.5 min: `JAVA_HOME not set, 5 gradle tests fail`
- 0.5 min: `mvn not found`
- 0.5 min: `Maven build fails: 15 Ghidra 12.1.2 SDK deps not in Maven Central`

Attempt 2:

- 2 min: `JDK 21 not installed`
- 1 min: `uv not installed`

Attempt 3:

- `5 gradle tests (test_gradle_tasks.py) fail , no Java available in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
