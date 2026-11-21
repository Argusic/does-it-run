# CNEquity

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rootSunc/CNEquity, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cnequity

## Pinned environment

- Project commit: `05370ab722acaaf1cf4cebc8b4489aaa81d5083b`
- Test commit: `05370ab722acaaf1cf4cebc8b4489aaa81d5083b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 31.4 to 50.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 31.4 | 5 | 5 | [run](https://argusic.com/run/2fd049f4-b5dd-49a0-9878-ce058860e808) |
| 2 | fail | 20 | n/a | 50.2 | 0 | 0 | [run](https://argusic.com/run/145bed7c-c42d-48ee-bd17-7e31a5aa1548) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Missing babel module - test_i18n.py couldn't import`
- 1 min: `Missing zstandard module - snapshot archive tests failed`
- 10 min: `test_another_process_blocks_until_it_exits - scheduler lock failed because uuid.getnode() returns different MACs in child processes in container`
- 5 min: `test_loopback_accepts_ipv4_and_ipv6 - IPv6 loopback (::1) disabled in container, test tried to connect and failed`
- 2 min: `test_snapshot_archive_*.zst tests - zstd compression library not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
