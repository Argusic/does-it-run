# hyperfide

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Sidiora-Labs/hyperfide, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/hyperfide

## Pinned environment

- Project commit: `29731ee31f35afefb76f5bae876833dd808661d4`
- Test commit: `29731ee31f35afefb76f5bae876833dd808661d4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 12.4 | 3 | 3 | [run](https://argusic.com/run/6e9712b3-ddcd-412a-8fc1-4bf2be239367) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `libsqlite3-dev and libcurl4-openssl-dev headers not installed system-wide (no root)`
- 1 min: `sqlite3 CLI tool not in PATH for integration tests`
- 15 min: `8 integration tests (57,58,59,62,63,65,66,67,69,78) fail due to missing -I/tmp/dev_include in their Makefile-less C compilation commands`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
