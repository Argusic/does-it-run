# timezone-boundary-builder

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/evansiroky/timezone-boundary-builder, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/timezone-boundary-builder

## Pinned environment

- Project commit: `a34f364b8f487e25efb32ea3379d617c1f5f5e24`
- Test commit: `a34f364b8f487e25efb32ea3379d617c1f5f5e24`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 1.9 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 1.9 | 1 | 1 | [run](https://argusic.com/run/1354bbde-d0c0-4eae-ace1-804651ad9266) |
| 2 | pass with mocks | 92 | 0.2 | 6.4 | 1 | 1 | [run](https://argusic.com/run/ab7073d1-2e93-44d1-b75f-7afe72a196e6) |

## What was observed on a clean machine

Attempt 1:

- `Minor npm deprecation warnings for 8 packages (no functional impact)`

Attempt 2:

- 0.5 min: `node index.js --included_zones crashes with TypeError: Cannot read properties of undefined when --skip_1970_zones or --skip_now_zones is used together with --included_zones or --excluded_zones, because zoneCfg1970/zoneCfgNow are empty objec`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
