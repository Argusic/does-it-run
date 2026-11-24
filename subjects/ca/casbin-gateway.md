# casbin-gateway

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/apache/casbin-gateway, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/casbin-gateway

## Pinned environment

- Project commit: `460b8af28785c874638b8e554599b5b0fd89383d`
- Test commit: `460b8af28785c874638b8e554599b5b0fd89383d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 7.1 to 9.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 9.9 | 1 | 1 | [run](https://argusic.com/run/4d6a88bb-1ebe-40e8-8232-ecd72c2c5bee) |
| 2 | fail | 20 | n/a | 7.1 | 0 | 0 | [run](https://argusic.com/run/9b5b5cb8-378d-485e-8a7d-d884726490ea) |

## What was observed on a clean machine

Attempt 1:

- `Desktop launcher fails: libwebkit2gtk-4.1.so.0 not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
