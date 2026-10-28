# AutoSwarm-Shadow-Adapter

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AhmadHassan-BTed/AutoSwarm-Shadow-Adapter, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/autoswarm-shadow-adapter

## Pinned environment

- Project commit: `69d27ddcd626b93566261d8363f99f79731a36a7`
- Test commit: `69d27ddcd626b93566261d8363f99f79731a36a7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.2 to 3.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 3.2 | 1 | 1 | [run](https://argusic.com/run/b24030ab-a137-4ddf-904c-8427b86eae5d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Frontend static build (frontend/dist) was not present, so the root route returned a JSON fallback instead of the React portal`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
