# s3-proxy

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/oxyno-zeta/s3-proxy, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/s3-proxy

## Pinned environment

- Project commit: `91139410df6fc1c90c0ebe0255ead7bb954ccab8`
- Test commit: `91139410df6fc1c90c0ebe0255ead7bb954ccab8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.2 to 2.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 2.2 | 0 | 0 | [run](https://argusic.com/run/5ec87e01-68d3-468a-a38e-c2a791da31ef) |

## What was observed on a clean machine

No error was recorded during the valid runs.

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
