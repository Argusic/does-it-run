# kronotop

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kronotop/kronotop, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/kronotop

## Pinned environment

- Project commit: `892d218985b4d338604cdf4e307838220ecf8f09`
- Test commit: `892d218985b4d338604cdf4e307838220ecf8f09`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 35.2 to 35.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 34.9 | 35.2 | 5 | 5 | [run](https://argusic.com/run/e41eac73-fc3d-4c30-b248-41b4f58349ac) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `No JDK 25 in container`
- 7 min: `No FoundationDB installed`
- 15 min: `fdbcli --exec hung on initial connect`
- 8 min: `FDB server kept dying before configuration persisted`
- 3 min: `Kronotop server exited after startup with MemberAlreadyRunningException`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
