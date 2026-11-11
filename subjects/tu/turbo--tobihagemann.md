# turbo

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tobihagemann/turbo, licensed MIT, written in Shell.

Evidence and recordings: https://argusic.com/run/34461dfe-5af2-4979-98f8-aa5d646d48a9

## Pinned environment

- Project commit: `a75a1681c98be0f4f0f8b715980005c34fd4d146`
- Test commit: `a75a1681c98be0f4f0f8b715980005c34fd4d146`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4 to 4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 4 | 3 | 3 | [run](https://argusic.com/run/34461dfe-5af2-4979-98f8-aa5d646d48a9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `bubblewrap (bwrap) not available on PATH; workspace-write sandbox fails with kernel namespace error`
- `gh (GitHub CLI) not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
