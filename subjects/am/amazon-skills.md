# Amazon-Skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nexscope-ai/Amazon-Skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/amazon-skills

## Pinned environment

- Project commit: `0f3b13fa0e5ed0a9f3d600dc18518bc76ddd813b`
- Test commit: `0f3b13fa0e5ed0a9f3d600dc18518bc76ddd813b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.7 | 1 | 1 | [run](https://argusic.com/run/fb0f1c85-9fb9-4df5-9b13-3d5d89a1cb64) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `npx skills@latest requires Node>=22, container has Node 18`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
