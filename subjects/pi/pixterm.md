# pixterm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/eliukblau/pixterm, licensed MPL-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/pixterm

## Pinned environment

- Project commit: `24a1aedad1a99b2177808bfd72b23e27318989f6`
- Test commit: `24a1aedad1a99b2177808bfd72b23e27318989f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.9 to 2.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 2.9 | 1 | 1 | [run](https://argusic.com/run/29d3ec3b-cd90-43ee-b61a-672c5e27ec7a) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go compiler not present in container (go: not found)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
