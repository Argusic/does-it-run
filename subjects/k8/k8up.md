# k8up

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k8up-io/k8up, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/k8up

## Pinned environment

- Project commit: `67048d8754bd585bbe33da4e6c56372312ebdd05`
- Test commit: `67048d8754bd585bbe33da4e6c56372312ebdd05`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.9 to 11.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 11.9 | 3 | 3 | [run](https://argusic.com/run/98c316dd-0ee3-428e-b391-10fc082314ab) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in environment`
- 1 min: `MinIO download URL (dl.min.io) returned 410 Gone`
- 2 min: `MinIO process management issues in ephemeral shell sessions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
