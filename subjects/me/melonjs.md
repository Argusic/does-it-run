# melonJS

**Verdict: could not verify.** Argusic Score 35.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/melonjs/melonJS, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/melonjs

## Pinned environment

- Project commit: `88402bc76f70b6ae1324512414ee132148d63fa8`
- Test commit: `88402bc76f70b6ae1324512414ee132148d63fa8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 28.7 to 87.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 87.1 | 0 | 0 | [run](https://argusic.com/run/1e0f17fe-6fe3-40ac-a436-0d79e63ad242) |
| 2 | fail | 35.71 | 3 | 28.7 | 7 | 2 | [run](https://argusic.com/run/3f185778-0859-4add-a337-ed0abee71e83) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Container had Node.js v18 but project requires >=24`
- `drawmesh_bench.spec.js timeout: SwiftShader software rasterization too slow (test timed out at 45s, needed ~198s)`
- `renderable-transform.spec.js hook timeout: beforeAll creating WebGL context took >90s on SwiftShader`
- `font.spec.js wordWrap test: expected measureText width <=100, got 110 (DejaVu Sans metrics different from Arial)`
- `text-gradient.spec.js: gradient top-color comparison fails due to font-rendering differences in headless Chromium`
- `trigger_level_change.spec.js: async race condition causes 3 loads instead of expected 1 in constrained env`
- 1 min: `Playwright browsers not installed`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
