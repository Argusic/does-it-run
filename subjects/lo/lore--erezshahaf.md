# Lore

**Verdict: runs with mocks.** Argusic Score 52.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ErezShahaf/Lore, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/run/ef0ae91f-abcf-4813-ad92-233a294ee348

## Pinned environment

- Project commit: `2403e99e98eac57ca1a77a7cbc68337c4355a9dd`
- Test commit: `2403e99e98eac57ca1a77a7cbc68337c4355a9dd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 10 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 10 | 0 | 0 | [run](https://argusic.com/run/ef0ae91f-abcf-4813-ad92-233a294ee348) |
| 2 | pass with mocks | 85.33 | 12 | 13.4 | 3 | 2 | [run](https://argusic.com/run/eeecfda0-1038-45e1-a407-2d26a9dd1e3b) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `vite build failed: Cannot find native binding for @tailwindcss/oxide (npm optional-dependency bug on Node 18)`
- 1 min: `Electron aborts: SUID sandbox helper not configured (no root in container)`
- `Engine warnings (EBADENGINE): packages require Node >=20, container has Node 18.19.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
