# elephant-goldfish-model

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/elephant-goldfish-model, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/elephant-goldfish-model

## Pinned environment

- Project commit: `d651fe86c12dccc5272274e002674fb8eec4c547`
- Test commit: `d651fe86c12dccc5272274e002674fb8eec4c547`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 1 | 3 | 1 | 0 | [run](https://argusic.com/run/1188ee8a-65cc-476c-a072-021f8b994e3a) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Astro site build requires Node.js >=22.12.0, container has v18.19.1. No root to upgrade.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
