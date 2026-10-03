# shattered-pixel-dungeon

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/00-Evan/shattered-pixel-dungeon, licensed GPL-3.0, written in Java.

Evidence and recordings: https://argusic.com/subject/shattered-pixel-dungeon

## Pinned environment

- Project commit: `7b8b845a76fe76c6b7c031ae9e570852411f56db`
- Test commit: `7b8b845a76fe76c6b7c031ae9e570852411f56db`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 4.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 6 | 0 | 0 | [run](https://argusic.com/run/db06bd7b-2ea9-4db5-9986-cd76558dd552) |
| 2 | pass | 100 | 4 | 11.7 | 0 | 0 | [run](https://argusic.com/run/579a7ecd-9869-4e98-a510-06ee4c84b109) |
| 3 | fail | 80 | 7 | 4.7 | 2 | 2 | [run](https://argusic.com/run/235aa94a-0dbd-4f6f-b4e3-6cbc0dd2693a) |

## What was observed on a clean machine

Attempt 3:

- 2 min: `No Java runtime installed in container`
- 1 min: `Gradle could not delete stale build directory`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
