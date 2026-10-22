# restic-backup-docker

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/lobaro/restic-backup-docker, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/restic-backup-docker

## Pinned environment

- Project commit: `47d29529e9dded28c71dccabb35b454f517a136f`
- Test commit: `47d29529e9dded28c71dccabb35b454f517a136f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 5 | 6 | 4 | 2 | [run](https://argusic.com/run/86a2aa1c-76db-461d-9134-bb7f17125dfd) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Docker not available in container (no root)`
- 2 min: `/var/log/ not writable by runner user`
- 1 min: `Scripts use bash syntax but /bin/sh is dash`
- 1 min: `crond binary not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
