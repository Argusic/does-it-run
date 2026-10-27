# Sico

**Verdict: runs with mocks.** Argusic Score 89.1 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/Sico, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/sico

## Pinned environment

- Project commit: `ee477dd874c53c87e9be9343e883c3822a7cd666`
- Test commit: `ee477dd874c53c87e9be9343e883c3822a7cd666`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 44.2 to 44.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 89.14 | 4 | 44.2 | 7 | 6 | [run](https://argusic.com/run/5a8cd8ae-4126-4c1a-a835-e09b6b358bc8) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python 3.12 installed, requires >=3.13`
- 2 min: `Go compiler not found`
- `uv not found`
- `pnpm not found`
- `Node v18.19.1 does not match required v24.13.0`
- 1 min: `Missing @tailwindcss/oxide native binary for linux-x64-gnu`
- `Frontend packages/shared tests hang/timeout in environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
