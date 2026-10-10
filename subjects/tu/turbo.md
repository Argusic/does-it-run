# turbo

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/didi/turbo, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/turbo

## Pinned environment

- Project commit: `4cac6b00af0f70351b3e3ef5a69527e380ab01e2`
- Test commit: `4cac6b00af0f70351b3e3ef5a69527e380ab01e2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 22.2 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 22.2 | 2 | 2 | [run](https://argusic.com/run/b642facd-a8f6-4021-a85b-b85c2ded6abf) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `Engine JUnit 4 tests skipped (no Vintage Engine), no H2 test config`
- 1 min: `BaseTest had no runnable methods, caused InvalidTestClass error on Surefire`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
