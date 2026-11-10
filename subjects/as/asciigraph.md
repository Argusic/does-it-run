# asciigraph

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/guptarohit/asciigraph, licensed BSD-3-Clause, written in Go.

Evidence and recordings: https://argusic.com/subject/asciigraph

## Pinned environment

- Project commit: `3934c9cdf72ac4806f3a2ef77004b62d1e236028`
- Test commit: `3934c9cdf72ac4806f3a2ef77004b62d1e236028`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.1 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 6.6 | 1 | 1 | [run](https://argusic.com/run/14f8f67c-0c56-418b-88b9-506b97fdc820) |
| 2 | pass | 100 | 1 | 1.1 | 0 | 0 | [run](https://argusic.com/run/d37a4a82-9387-4b42-b605-b919ec927680) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Go compiler not pre-installed in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
