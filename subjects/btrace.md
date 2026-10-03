# btrace

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/btraceio/btrace, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/btrace

## Pinned environment

- Project commit: `a1b6b59c34768659116029041985b9c9546f8983`
- Test commit: `a1b6b59c34768659116029041985b9c9546f8983`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 33.9 to 33.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 33.9 | 2 | 2 | [run](https://argusic.com/run/45ea682d-6da9-4aac-b3e2-77aeced750aa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `No Java JDK installed in container; needed JDK 8, 11, 21, 24 for multi-toolchain build`
- 2.5 min: `Issue884PublishedFatAgentE2ETest failed because forked Gradle processes didn't inherit toolchain config`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
