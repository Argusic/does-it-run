# video-podcast-maker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Agents365-ai/video-podcast-maker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/video-podcast-maker

## Pinned environment

- Project commit: `33b8078e3e87c9626d39d144b4c901b4ebf16f74`
- Test commit: `33b8078e3e87c9626d39d144b4c901b4ebf16f74`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 7 | 2 | 2 | [run](https://argusic.com/run/c23d0d83-5933-4c98-b9a9-331cd19e840c) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed: externally managed environment (PEP 668)`
- 3 min: `Remotion 4.0.533 incompatible with react 18.3.1 and zod 3.23.0 , render failed with React export error`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
