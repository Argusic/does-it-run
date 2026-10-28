# client

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tetiva-app/client, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/run/800cb43e-a7ba-4627-b95c-f14c68f8c61e

## Pinned environment

- Project commit: `3eb9e14b47acfdc9a2f4c8e88339880a6a286b08`
- Test commit: `3eb9e14b47acfdc9a2f4c8e88339880a6a286b08`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 15.5 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 15.5 | 4 | 4 | [run](https://argusic.com/run/800cb43e-a7ba-4627-b95c-f14c68f8c61e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `go: not found`
- 5 min: `Wails CLI requires gtk4/webkitgtk-6.0 dev headers; no root for apt`
- 1 min: `frontend/dist missing for go:embed`
- `Flaky test prefix_linear_in_z_run exceeds 200ms under parallel load`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
