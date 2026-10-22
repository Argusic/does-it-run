# show-me-the-story

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Nigh/show-me-the-story, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/show-me-the-story

## Pinned environment

- Project commit: `173b81e8347a6e1e71bd5c7248ab995abee31b65`
- Test commit: `173b81e8347a6e1e71bd5c7248ab995abee31b65`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.7 to 4.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 4.7 | 2 | 2 | [run](https://argusic.com/run/2f042404-0c95-45fe-8c4a-09c9297243a8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go 1.25.1 not installed in container`
- 1 min: `Frontend build failed: missing @tailwindcss/oxide native binding for linux-x64-gnu`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
