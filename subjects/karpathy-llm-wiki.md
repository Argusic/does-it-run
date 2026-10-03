# karpathy-llm-wiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Astro-Han/karpathy-llm-wiki, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/karpathy-llm-wiki

## Pinned environment

- Project commit: `eafcc77001e496cc43499e4923b663aec722c813`
- Test commit: `eafcc77001e496cc43499e4923b663aec722c813`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 3.4 | 1 | 1 | [run](https://argusic.com/run/e0bc1d6b-3266-45e8-b8da-1c486ea410c3) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `npx add-skill requires Node.js >=22.20.0, container has v18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
