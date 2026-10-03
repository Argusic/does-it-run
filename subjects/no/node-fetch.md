# node-fetch

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/node-fetch/node-fetch, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/node-fetch

## Pinned environment

- Project commit: `8b3320d2a7c07bce4afc6b2bf6c3bbddda85b01f`
- Test commit: `8b3320d2a7c07bce4afc6b2bf6c3bbddda85b01f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.4 to 4.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.32 | 4.4 | 1 | 1 | [run](https://argusic.com/run/811375ef-aa53-42ee-9088-41522e0b9e14) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `IPv6 test fails - EADDRNOTAVAIL address not available ::1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
