# ratel

**Verdict: could not verify.** Argusic Score 0 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ratel-ai/ratel, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ratel

## Pinned environment

- Project commit: `99aee29b51a658a22017536f783527daacec9b88`
- Test commit: `99aee29b51a658a22017536f783527daacec9b88`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 32 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 0 | 32 | 32 | 3 | 0 | [run](https://argusic.com/run/fe365999-c1e8-4f98-a3cb-a2774ca853d3) |
| 2 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/28079daa-7701-4cfd-906d-1ded6b243836) |

## What was observed on a clean machine

Attempt 1:

- `Python native addons (ratel-sdk-python-native, ratel-rankers-python-native) fail to link: missing -lpython3.12 (python3-dev not installed; no root to install it)`
- `Next.js web app build OOM-killed at ~326MB during 'Collecting page data' (container cgroup memory limit). Full production build cannot complete.`
- `Docker not available in container; docker-compose based standard install path not testable.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
