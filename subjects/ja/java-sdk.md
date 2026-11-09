# java-sdk

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modelcontextprotocol/java-sdk, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/java-sdk

## Pinned environment

- Project commit: `c7fef64f92a99c8c758b1aa634f92868d7c2963b`
- Test commit: `c7fef64f92a99c8c758b1aa634f92868d7c2963b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 15.3 to 23.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 15.3 | 1 | 1 | [run](https://argusic.com/run/123cbc12-a55b-46e7-9464-363ccdd82d12) |
| 2 | pass | 100 | 5 | 23.7 | 2 | 2 | [run](https://argusic.com/run/9724309e-5e47-465e-ac1f-216cdf5452f4) |

## What was observed on a clean machine

Attempt 1:

- `Docker not installed - 12 integration tests that require Testcontainers could not run`

Attempt 2:

- 2 min: `No JDK installed (java: not found)`
- `12 integration tests fail: Docker not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
