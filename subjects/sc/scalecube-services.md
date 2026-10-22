# scalecube-services

**Verdict: runs.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/scalecube/scalecube-services, licensed Apache-2.0, written in Java.

Evidence and recordings: https://argusic.com/subject/scalecube-services

## Pinned environment

- Project commit: `76d941b9df18db158b3f5b458e3eb586b4f29763`
- Test commit: `76d941b9df18db158b3f5b458e3eb586b4f29763`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.8 to 10.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 80 | 10.1 | 10.8 | 1 | 0 | [run](https://argusic.com/run/29e0a387-8c84-4774-b5f0-5566c7a4cc85) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `services-security: ServiceTokenTests fails because Docker socket unavailable (Testcontainers Vault container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
