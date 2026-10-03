# termscp

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/veeso/termscp, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/termscp

## Pinned environment

- Project commit: `4120311bf62e48e6a08ba322aad4e292ee36f434`
- Test commit: `4120311bf62e48e6a08ba322aad4e292ee36f434`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.9 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 8 | 8.9 | 2 | 1 | [run](https://argusic.com/run/48a3494d-cfb1-4138-88de-11f4088991e4) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain installed`
- 2 min: `Default build fails: libsmbclient-dev not found (pavao-sys requires smbclient.pc)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
