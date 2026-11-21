# webhookd

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ncarlier/webhookd, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/webhookd

## Pinned environment

- Project commit: `5ac66677bf7224191f1dfc51a875b09187d10beb`
- Test commit: `5ac66677bf7224191f1dfc51a875b09187d10beb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.1 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 4 | 2 | 2 | [run](https://argusic.com/run/871454be-f42a-4916-bfa3-68a6d5c044b9) |
| 2 | pass | 100 | 2.5 | 2.1 | 2 | 2 | [run](https://argusic.com/run/230c8759-e70c-4847-945a-82a06a72b3b3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not installed in container`
- 1 min: `/usr/local not writable for Go SDK extraction`

Attempt 2:

- 1 min: `golang-go compiler not available (no root on container); used pre-built binary instead`
- 0.1 min: `htpasswd file missing warning on startup`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
