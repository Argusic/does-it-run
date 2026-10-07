# CLIProxyAPI

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/router-for-me/CLIProxyAPI, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/cliproxyapi

## Pinned environment

- Project commit: `a2976eb8a303f11b4ea5177bce9f9ff752634dfc`
- Test commit: `a2976eb8a303f11b4ea5177bce9f9ff752634dfc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.4 to 17.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8 | 17.4 | 2 | 2 | [run](https://argusic.com/run/9a2d8432-08aa-496c-be08-76b19b8680bb) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go compiler not installed in container`
- 3 min: `Test TestServiceCatalogStartupAndConfigReload failed (defer cleanup set Home.Enabled=true causing Devin catalog to be disabled)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
