# ha-linky

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/bokub/ha-linky, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/ha-linky

## Pinned environment

- Project commit: `99419a30e879c2a7fa379558ba0c2493a27092e1`
- Test commit: `99419a30e879c2a7fa379558ba0c2493a27092e1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 11.5 to 16.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11.5 | 0 | 0 | [run](https://argusic.com/run/be096c55-e99b-48a3-89fc-adbd0c78f1fb) |
| 2 | pass with mocks | 92 | 0.1 | 16.9 | 2 | 2 | [run](https://argusic.com/run/d5390719-4c84-439c-b652-1ace43a9abe5) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Tests failed because container timezone (UTC) differs from test expectations (Europe/Paris) - 8 tests failed with timezone-offset date mismatches`
- 2 min: `Config path hardcoded to /data/options.json, preventing non-root app launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
