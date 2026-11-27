# ai-design-skills

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/elayadesign/ai-design-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-design-skills

## Pinned environment

- Project commit: `4fdcdd52f15eda09da1257c303c860c13e0c879f`
- Test commit: `4fdcdd52f15eda09da1257c303c860c13e0c879f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.8 to 2.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.3 | 2.8 | 2 | 2 | [run](https://argusic.com/run/0e6462d6-c431-42f7-931f-68333f55c00c) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npx skills CLI (v1.9.0) requires Node.js >=22.20.0; system has v18.19.1`
- 0.3 min: `pip install fails due to PEP 668 externally-managed-environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
