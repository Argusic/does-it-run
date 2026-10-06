# greenmask

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GreenmaskIO/greenmask, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/greenmask

## Pinned environment

- Project commit: `d34cce1ee80538533c68a7bdbd9797aed1aaff82`
- Test commit: `d34cce1ee80538533c68a7bdbd9797aed1aaff82`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 6.7 to 9.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 6 | 6.7 | 5 | 5 | [run](https://argusic.com/run/de31e782-c199-4b9a-97d5-6507e2b7d54f) |
| 2 | pass with mocks | 92 | 6 | 9.7 | 2 | 2 | [run](https://argusic.com/run/99c85a41-e0fa-4a35-b509-b6811fc12c33) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not pre-installed; downloaded Go 1.27.1 from go.dev`
- `Docker unavailable , tests requiring PostgreSQL containers fail (internal/db/postgres/context, restorers, utils)`
- `Integration tests (tests/integration/*) require external flags (-tempDir, -pgBinPath, -storageS3Endpoint, GREENMASK_BIN_PATH) not provided`
- `Azure storage tests fail , need real Azure credentials`
- `SSH storage tests fail , need SSH server`

Attempt 2:

- 2 min: `Go compiler not found in container`
- `Docker not available , 4 test packages (context, restorers, utils, azure, ssh) fail because Testcontainers cannot start PostgreSQL/Azure/SSH containers`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
