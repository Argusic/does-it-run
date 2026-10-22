# para

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Erudika/para, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/para

## Pinned environment

- Project commit: `dc9522c9bd2b37faf6d0d1f8eabcaee9bcb57ae2`
- Test commit: `dc9522c9bd2b37faf6d0d1f8eabcaee9bcb57ae2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 18.9 to 18.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 18.9 | 2 | 2 | [run](https://argusic.com/run/c6210244-65b5-4d18-af5f-09c02c6da8b0) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `No Java or Maven installed in container`
- 0.2 min: `Fatjar without lucene profile uses MockSearch which throws UnsupportedOperationException`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
