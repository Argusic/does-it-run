# quotio

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nguyenphutrong/quotio, licensed MIT, written in Rust.

Evidence and recordings: https://argusic.com/subject/quotio

## Pinned environment

- Project commit: `dfa5beeb59cd169d98b25331f72c3149c713cae2`
- Test commit: `dfa5beeb59cd169d98b25331f72c3149c713cae2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 12.1 to 14 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 19 | 14 | 4 | 4 | [run](https://argusic.com/run/1d0d508e-b1c1-457c-a94c-7dd4d25ccd37) |
| 2 | pass with mocks | 92 | 10 | 12.1 | 2 | 2 | [run](https://argusic.com/run/2745b09b-0314-4278-9b2a-0810fc6a02d8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npm global install EACCES /usr/local/lib/node_modules`
- 15 min: `19 suite tests failed: hard-coded /usr/bin/sqlite3 missing (NotFound)`
- 1 min: `quotio serve --port rejected (Invalid arguments)`
- 2 min: `serve default returned 503 credential_storage_unavailable on Linux`

Attempt 2:

- 1 min: `Rust toolchain not installed in container`
- 2 min: `sqlite3 CLI binary not present at /usr/bin/sqlite3 (hardcoded in test/fixture code) causing 19 test failures`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
