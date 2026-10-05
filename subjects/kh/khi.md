# khi

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GoogleCloudPlatform/khi, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/khi

## Pinned environment

- Project commit: `d402902ffbc2141a1c79e7f8283e46de9b3bd303`
- Test commit: `d402902ffbc2141a1c79e7f8283e46de9b3bd303`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 13.8 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/4dfc6fc2-7e77-4942-833a-c2f1d2135da4) |
| 2 | pass | 100 | 8 | 13.8 | 4 | 4 | [run](https://argusic.com/run/ac2ceeb1-f167-4c42-ab93-fde24a68414d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Go compiler not installed; required Go 1.26.0`
- 1 min: `Node.js 18.x installed but 26.7.0 required`
- 1 min: `gcloud CLI not installed; cloud logging tests fail without credentials`
- 2 min: `No Chrome browser installed; frontend tests cannot run`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
