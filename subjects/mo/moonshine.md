# moonshine

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moonshine-software/moonshine, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/subject/moonshine

## Pinned environment

- Project commit: `b33726f35dfcc516aeb18a5e9c9f3c513c5c8b57`
- Test commit: `b33726f35dfcc516aeb18a5e9c9f3c513c5c8b57`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 14.2 to 26.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 14.2 | 3 | 3 | [run](https://argusic.com/run/3b368ddf-dcc0-4cc9-bdde-4bebe8911612) |
| 2 | pass with mocks | 92 | 22 | 26.7 | 4 | 4 | [run](https://argusic.com/run/63241da0-c0b3-4d9f-9a72-a059eafd648e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `No PHP or Composer installed in container`
- 2 min: `Node.js v18 too old for project dependencies (requires v22+)`
- 1 min: `Corrupted vendor config file vendor/orchestra/testbench-core/laravel/config/moonshine.php had trailing garbage lines causing ParseError`

Attempt 2:

- 3 min: `Container has no PHP interpreter`
- 1 min: `No Composer available`
- 1 min: `Tests configured for MySQL which is not available`
- 1 min: `Missing APP_KEY for Laravel encryption`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
