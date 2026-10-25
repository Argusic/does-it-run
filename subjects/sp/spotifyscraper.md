# SpotifyScraper

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AliAkhtari78/SpotifyScraper, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/spotifyscraper

## Pinned environment

- Project commit: `9cbf05aa4963bac3684bb941270dcb62fc851ab7`
- Test commit: `9cbf05aa4963bac3684bb941270dcb62fc851ab7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.1 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.1 | 1 | 1 | [run](https://argusic.com/run/405723f7-b790-41f4-bcbb-78be3ebfbffb) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `mcp 2.3.0 installed by default is incompatible with the project's FastMCP import (mcp<2 required by pyproject.toml but pin was ignored by pip dependency resolution)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
