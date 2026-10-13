# mcp-nixos

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/utensils/mcp-nixos, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/mcp-nixos

## Pinned environment

- Project commit: `6a517811658c21f97bd7703b35546085117fc310`
- Test commit: `6a517811658c21f97bd7703b35546085117fc310`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 8.4 to 8.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 8.4 | 2 | 2 | [run](https://argusic.com/run/7cb9dc35-8e38-4ecd-9350-86507ee37744) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `NVF options source only found 64 options (broken parsing) because docs moved to JS-chunk loading`
- 2 min: `pip install failed due to externally-managed environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
