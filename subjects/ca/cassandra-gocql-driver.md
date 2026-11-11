# cassandra-gocql-driver

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/cassandra-gocql-driver, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/cassandra-gocql-driver

## Pinned environment

- Project commit: `00fc2909c64a7529fe49fb31b0fa8662342ebe69`
- Test commit: `00fc2909c64a7529fe49fb31b0fa8662342ebe69`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 6.6 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 1.5 | 6.6 | 0 | 0 | [run](https://argusic.com/run/728a88c8-2b07-40b4-a3d7-c2f32acbe7bd) |
| 2 | pass | 100 | 2 | 7.8 | 1 | 1 | [run](https://argusic.com/run/4693a312-e2a1-4ad0-96cf-c75b60eea20d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go 1.22.2 compiler not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
