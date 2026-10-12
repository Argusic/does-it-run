# sandboxd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tastyeffectco/sandboxd, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/sandboxd

## Pinned environment

- Project commit: `6b1ddabad6f5741a43246782e1f9fcd1757865c3`
- Test commit: `6b1ddabad6f5741a43246782e1f9fcd1757865c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.4 to 12.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20.5 | 12.4 | 1 | 1 | [run](https://argusic.com/run/75bacb3a-d32c-4b65-9fc4-c63ff9cfeb01) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `cmd/sandboxd/main.go compilation: undefined 'instanceID' at line 479 and undefined 'cloudOrg' at line 677 , both caused by variable scoping errors in the gVisor resolv.conf block`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
