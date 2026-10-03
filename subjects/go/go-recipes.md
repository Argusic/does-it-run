# go-recipes

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nikolaydubina/go-recipes, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/go-recipes

## Pinned environment

- Project commit: `a954f17ee3ef96a7834dd287ea5ab27c4731ed68`
- Test commit: `a954f17ee3ef96a7834dd287ea5ab27c4731ed68`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 2.7 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 2.5 | 2.8 | 1 | 1 | [run](https://argusic.com/run/3b93d9e0-f34f-4f88-9abb-657689c18b0a) |
| 2 | fail | 80 | 0.1 | 2.7 | 0 | 0 | [run](https://argusic.com/run/e7389726-270d-4964-910b-58fcd87c51ff) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `Go toolchain not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
