# kubefwd

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/txn2/kubefwd, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/kubefwd

## Pinned environment

- Project commit: `a4dc4940bc8b4f033c97125bb5e6f301276dda52`
- Test commit: `a4dc4940bc8b4f033c97125bb5e6f301276dda52`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 6.9 to 16.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4 | 16.1 | 2 | 2 | [run](https://argusic.com/run/3945b60b-a4e0-47c7-af86-3ea731197708) |
| 2 | pass | 100 | 5 | 6.9 | 0 | 0 | [run](https://argusic.com/run/26f81b84-96c2-45f8-83f3-02f311d6e6ed) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.26 was not pre-installed in the container`
- `kubefwd needs root/sudo to run (requires /etc/hosts and loopback IP manipulation)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
