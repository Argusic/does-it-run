# OpenRA

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenRA/OpenRA, licensed GPL-3.0, written in C#.

Evidence and recordings: https://argusic.com/subject/openra

## Pinned environment

- Project commit: `8eac2bb69061b02b974beeae8f7feaab860610c0`
- Test commit: `8eac2bb69061b02b974beeae8f7feaab860610c0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 10 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12.9 | 13.4 | 1 | 1 | [run](https://argusic.com/run/cfc11d40-0f7f-412e-b0e1-0ed12bcda538) |
| 2 | pass | 100 | 1.5 | 10 | 0 | 0 | [run](https://argusic.com/run/15be4611-2b91-478a-acc8-28d32132d89e) |
| 3 | pass | 100 | 1 | 10 | 0 | 0 | [run](https://argusic.com/run/7457d4dd-b857-48e7-8d75-8d8a4636e555) |

## What was observed on a clean machine

Attempt 1:

- `Utility check-yaml on 'all' mods fails: No node with key 'Cursors' - CheckCursors lint pass requires per-mod invocation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
