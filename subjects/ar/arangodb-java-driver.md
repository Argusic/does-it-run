# arangodb-java-driver

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/arangodb/arangodb-java-driver, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/arangodb-java-driver

## Pinned environment

- Project commit: `ea380b222f052d5fe44d12621f8cce8844d13a79`
- Test commit: `ea380b222f052d5fe44d12621f8cce8844d13a79`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.2 to 22.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 22.6 | 0 | 0 | [run](https://argusic.com/run/36cbae7d-6de9-441b-ae44-c23bc78d9b71) |
| 2 | pass | 100 | 14.5 | 13.2 | 5 | 5 | [run](https://argusic.com/run/4604ff1d-a8bb-4147-b37e-b95c72962b07) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `No Java JDK or Maven installed in container`
- 4 min: `No ArangoDB database available in container`
- 1 min: `arango.properties pointed at a private address:8529 (Docker internal network)`
- 3 min: `arangod kept dying after a few seconds when started as background child process`
- `JWT/auth tests fail with auth disabled on server`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
