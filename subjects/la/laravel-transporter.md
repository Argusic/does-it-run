# laravel-transporter

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JustSteveKing/laravel-transporter, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/laravel-transporter

## Pinned environment

- Project commit: `4118514194e5e7c3d9863bd57a2391206f3e0f69`
- Test commit: `4118514194e5e7c3d9863bd57a2391206f3e0f69`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.3 to 3.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 5 | 3.3 | 2 | 1 | [run](https://argusic.com/run/f333352a-184c-40b5-a82c-052361535a94) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `php: not found in container, and system package install denied (no root)`
- 1 min: `phpstan 2.3.1 rejects removed config key checkMissingIterableValueType and static CLI can't load phpstan turbo ext; run with level 9 left 24 pre-existing errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
