# engram

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Gentleman-Programming/engram, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/engram

## Pinned environment

- Project commit: `e108c2f5fbbe9b805351f4e9326184ccfc4f4d13`
- Test commit: `e108c2f5fbbe9b805351f4e9326184ccfc4f4d13`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.2 to 28.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 5.2 | 0 | 0 | [run](https://argusic.com/run/8a5e7f87-50aa-4c5f-bc34-4f5a2873f985) |
| 2 | pass | 100 | 2 | 28.5 | 1 | 1 | [run](https://argusic.com/run/510cd7c7-f2d2-4c8e-9696-c25918195fba) |
| 3 | pass | 100 | 5 | 7.9 | 1 | 1 | [run](https://argusic.com/run/e6fcebf7-8ea7-4c34-b1b3-67a2d3a1f32b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Go compiler not found in container`

Attempt 3:

- 3 min: `Go 1.25.10 not installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
