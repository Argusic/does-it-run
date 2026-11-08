# cds

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ovh/cds, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/cds

## Pinned environment

- Project commit: `efa68e88c86a1dc90f9b0fe4f941ffe6775e2368`
- Test commit: `efa68e88c86a1dc90f9b0fe4f941ffe6775e2368`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 35.7 to 42.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 42.3 | 4 | 4 | [run](https://argusic.com/run/59fcd7a5-4086-42c8-9905-a2db037daddb) |
| 2 | pass with mocks | 92 | 30 | 35.7 | 4 | 4 | [run](https://argusic.com/run/ba132f5c-8055-4984-88f3-2a3e4e9ca9d4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No Go toolchain in container`
- 2 min: `No PostgreSQL available`
- 1 min: `No Redis available`
- 1 min: `SQL migrations failed on PG 9.3 (no jsonb type)`

Attempt 2:

- 3 min: `Go compiler not found in container`
- 1 min: `Makefile build_all_engine targets cross-compile for 8 OS/arch combos, taking forever`
- 2 min: `Kubernetes plugin build failure: non-constant format string in call to fail()`
- 3 min: `Angular UI requires Node.js >=20.19, system has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
