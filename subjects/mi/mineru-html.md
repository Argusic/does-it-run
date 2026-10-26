# MinerU-HTML

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/opendatalab/MinerU-HTML, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mineru-html

## Pinned environment

- Project commit: `73cf266690befd209cae7e6fdff9716d5b31a976`
- Test commit: `73cf266690befd209cae7e6fdff9716d5b31a976`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.5 to 15.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 15.5 | 2 | 2 | [run](https://argusic.com/run/46bee207-de87-4986-a953-57ce97b7e832) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `selectolax 1.0 removed the parser backend; from selectolax.parser import HTMLParser fails with ImportError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
