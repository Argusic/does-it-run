# crate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crate/crate, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/crate

## Pinned environment

- Project commit: `66927f3454e76a63e902657630abba9617eb89d4`
- Test commit: `66927f3454e76a63e902657630abba9617eb89d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 27.2 to 44.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 44 | 44.9 | 4 | 4 | [run](https://argusic.com/run/239466dd-6a6e-4ea3-a4d9-bda4d32cf226) |
| 2 | pass | 100 | 36 | 36.6 | 1 | 1 | [run](https://argusic.com/run/75ab6b38-fb1b-4ab9-8769-53ffbb7b3525) |
| 3 | pass | 100 | 30 | 27.2 | 1 | 1 | [run](https://argusic.com/run/018c34d7-33fe-4c1e-8f48-909e25d81107) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Java runtime available on system`
- 5 min: `TcpTransportTest.testDefaultSeedAddresses* - 4 tests failing: expected IPv6 addresses but container has no IPv6 loopback`
- 10 min: `BlobIntegrationTest.testUploadInvalidSha1 - expects HTTP 400, gets HTTP 404`
- `BlobIntegrationTest.testParallelAccess - timed out after 3 minutes`

Attempt 2:

- 1 min: `forbiddenapis: java.lang.ClassNotFoundException: java.util.SequencedCollection when scanning Lists.class`

Attempt 3:

- 2 min: `JarHell in dist: duplicate crate-*.jar and crate-app-*.jar`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
