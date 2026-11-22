# awl

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/anywherelan/awl, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/awl

## Pinned environment

- Project commit: `c731a10f9103342365e19f86cd6daee1550f5ce7`
- Test commit: `c731a10f9103342365e19f86cd6daee1550f5ce7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 7.1 to 8.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 8.9 | 2 | 2 | [run](https://argusic.com/run/8259a161-2716-4135-8906-1562aef4092f) |
| 2 | pass | 100 | 7 | 7.1 | 3 | 3 | [run](https://argusic.com/run/4a4fd8a6-0c59-4ff0-bf0e-7f18366e09fa) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go not installed in container`
- 0.5 min: `Build fails: //go:embed static requires static/ directory`

Attempt 2:

- 2 min: `Go 1.26 not installed in container`
- 1 min: `Missing 'static' directory for embed.FS`
- `Server cannot create TUN device (no root)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
