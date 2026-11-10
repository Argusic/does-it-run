# termscp

**Verdict: runs.** Argusic Score 91 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/veeso/termscp, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/termscp

## Pinned environment

- Project commit: `4120311bf62e48e6a08ba322aad4e292ee36f434`
- Test commit: `4120311bf62e48e6a08ba322aad4e292ee36f434`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 8.9 to 43.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 8 | 8.9 | 2 | 1 | [run](https://argusic.com/run/48a3494d-cfb1-4138-88de-11f4088991e4) |
| 2 | pass | 100 | 43 | 43.4 | 2 | 2 | [run](https://argusic.com/run/ecfaf53d-b7ca-4b89-aa25-e9e8d0aaa191) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No Rust toolchain installed`
- 2 min: `Default build fails: libsmbclient-dev not found (pavao-sys requires smbclient.pc)`

Attempt 2:

- 5 min: `Missing system packages: libdbus-1-dev, libsmbclient-dev. Cannot install without root.`
- `auto_update test fails because GitHub reports v1.2.2 as latest release, but test was written for v1.2.0 being latest and expects AlreadyUptodate result.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
