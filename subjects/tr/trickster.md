# trickster

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/trickstercache/trickster, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/trickster

## Pinned environment

- Project commit: `b3e628249433bd86ae052f391caac507eeb3e3d7`
- Test commit: `b3e628249433bd86ae052f391caac507eeb3e3d7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.6 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 12.6 | 2 | 2 | [run](https://argusic.com/run/6018b831-433b-4d81-8b94-fe8e19b635b7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27+ not installed in container`
- 1 min: `Initial config used frontends/origins (wrong YAML structure)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
