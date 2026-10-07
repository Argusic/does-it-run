# humanizer

**Verdict: could not verify.** Argusic Score 80 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/blader/humanizer, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/humanizer

## Pinned environment

- Project commit: `225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8`
- Test commit: `225a6f39ac85f76ee48dbad772ea4abe4ed6c9d8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 3.1 to 4.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 4 | 4.8 | 2 | 2 | [run](https://argusic.com/run/7ff18492-b4a2-47f6-9b68-cd996142f464) |
| 2 | fail | 80 | 2 | 3.1 | 0 | 0 | [run](https://argusic.com/run/a5c38561-1912-4cb9-88be-d8c5af62dc26) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `npx skills (latest v1.7.0) requires Node >=22.20.0; container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
