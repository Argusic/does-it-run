# pi-dynamic-workflows

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/QuintinShaw/pi-dynamic-workflows, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/pi-dynamic-workflows

## Pinned environment

- Project commit: `4b3027b39c7fa8a2f0c00e7652afef23a2fca426`
- Test commit: `4b3027b39c7fa8a2f0c00e7652afef23a2fca426`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 5.8 to 7.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 0.1 | 7.8 | 2 | 2 | [run](https://argusic.com/run/e3315543-ae53-4661-aca7-6a4e885f3064) |
| 2 | pass with mocks | 92 | 10 | 5.8 | 1 | 1 | [run](https://argusic.com/run/432378d1-bf2a-4e4e-8141-33648788923c) |

## What was observed on a clean machine

Attempt 1:

- 60 min: `Node v18.19.1 is below the project's implicit requirement (Node 22+). Dependencies import with syntax: 'with { type: "json" }' (Node 20+), '/v' regex flag (Node 20+), 'import.meta.dirname' (Node 21+), and '\p{RGI_Emoji}' property (Node 20+)`
- `npm run check (biome + tsc) passes, npm run build passes. Full test suite cannot execute: 38/52 test files blocked by Node 18, 244 tests pass, 16 fail from /v regex in @earendil-works/pi-tui.`

Attempt 2:

- 4 min: `System Node.js 18.19.1 too old for @earendil-works/pi-ai dependency (requires Node>=20 for import...with syntax)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
