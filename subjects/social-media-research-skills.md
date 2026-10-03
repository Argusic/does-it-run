# social-media-research-skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ScrapeCreators/social-media-research-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/social-media-research-skills

## Pinned environment

- Project commit: `64ba7b4dea71e130d2712ffb6c1c1024b3b7c4b2`
- Test commit: `64ba7b4dea71e130d2712ffb6c1c1024b3b7c4b2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 2.8 | 2 | 2 | [run](https://argusic.com/run/0cc8adf4-5c55-40bd-b8da-724c7e54d2c4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PyYAML not installed; validate-skills.py fails`
- 2 min: `npx skills requires Node >=22.20.0 but system has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
