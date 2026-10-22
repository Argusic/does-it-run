# neonplan3d

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Mastershort/neonplan3d, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/neonplan3d

## Pinned environment

- Project commit: `4c8b353d246d82121d79313de2110e0aaba07aa9`
- Test commit: `4c8b353d246d82121d79313de2110e0aaba07aa9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3.2 | 6.6 | 1 | 1 | [run](https://argusic.com/run/119c8094-d584-4c1a-9b0f-e1349422e4be) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `async_unload_entry in __init__.py raised KeyError: 'frontend_extra_module_url' during test teardown when frontend component is mocked`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
