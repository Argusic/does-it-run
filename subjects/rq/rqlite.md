# rqlite

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rqlite/rqlite, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/rqlite

## Pinned environment

- Project commit: `7eb7e54b14df25628c17eb68fc77b4d797d5b869`
- Test commit: `7eb7e54b14df25628c17eb68fc77b4d797d5b869`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 17 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.5 | 22 | 0 | 0 | [run](https://argusic.com/run/dea82bd0-54ac-49da-b9dc-35a8456fe516) |
| 2 | pass | 100 | 16.4 | 17 | 7 | 7 | [run](https://argusic.com/run/0b773d1c-778a-4fc5-9812-0da40cd2902d) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go toolchain was not installed or on PATH; 'go version' returned 'go: not found', blocking the documented 'go install ./...' workflow.`
- `'/usr/bin/time' was unavailable while timing the install ('/usr/bin/time: No such file or directory').`
- `'/bin/sh' did not support 'set -o pipefail', so an initial install command exited 2 before invoking Go.`
- 8 min: `'Test_Geopoly' failed because its expected JSON hardcoded '\ufffd' while Go 1.27.3 encoded the same replacement character as literal UTF-8.`
- 2 min: `The first rqlited verification process exited when its launching command session ended, so curl and rqlite received connection failures.`
- 1 min: `Python requests was missing, preventing the bundled system_test/e2e suite from importing helpers.`
- 2 min: `The first single-node E2E run had two FileNotFoundError errors for system_test/e2e/testdata/1000-numbers.db.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
