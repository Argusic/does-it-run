# osm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/paulmach/osm, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/osm

## Pinned environment

- Project commit: `4f398c4aa98299befea02dc78d1c29d5e31ab4c9`
- Test commit: `4f398c4aa98299befea02dc78d1c29d5e31ab4c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.5 to 1.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 1.2 | 1.5 | 1 | 1 | [run](https://argusic.com/run/f9a6ba3d-8c74-4d98-a992-638fed5a2871) |

## What was observed on a clean machine

Attempt 1:

- 0.8 min: `CGO build fails because zlib1g-dev is not installed (no root to install packages). Go requires pkg-config for zlib via the DataDog/czlib library.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
