# free-proxy-list

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gfpcom/free-proxy-list, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/free-proxy-list

## Pinned environment

- Project commit: `364a694e6f6fc858b6671a64e525267424f1494a`
- Test commit: `364a694e6f6fc858b6671a64e525267424f1494a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.8 to 6.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 14 | 6.8 | 2 | 2 | [run](https://argusic.com/run/a4f0453a-77c2-4cda-ac74-a8ccf10b6d65) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `Go toolchain not installed in container (no go binary, no apt without root)`
- 3 min: `Version truth: README says lists update hourly but repo action runs every hour, not relevant to run; first scratch run put README one level above list dir, so app's README rewrite silently no-op'd (error swallowed by _ = os.WriteFile)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
