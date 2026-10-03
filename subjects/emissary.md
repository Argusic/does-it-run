# emissary

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/emissary-ingress/emissary, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/emissary

## Pinned environment

- Project commit: `d6eb1ba441cbab2fd6cd5b126488242aaa506429`
- Test commit: `d6eb1ba441cbab2fd6cd5b126488242aaa506429`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 8 | 21 | 2 | 1 | [run](https://argusic.com/run/0f471bef-c86e-499f-8ac1-fb27c9e56eaa) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go not pre-installed; downloaded Go 1.25.0 tarball to ~/go_bootstrap`
- `Python integration tests require Docker for envoy config validation; not available`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
