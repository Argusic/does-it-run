# agency-orchestrator

**Verdict: runs with mocks.** Argusic Score 82 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jnMetaCode/agency-orchestrator, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agency-orchestrator

## Pinned environment

- Project commit: `bed66133356bd859f4bf7459c0a9ed5580fb2203`
- Test commit: `bed66133356bd859f4bf7459c0a9ed5580fb2203`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 11.2 to 49.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 49.3 | 4 | 4 | [run](https://argusic.com/run/c581b920-ebd6-4cfb-902a-0872bdb359bd) |
| 2 | pass with mocks | 72 | 8 | 11.2 | 3 | 0 | [run](https://argusic.com/run/b33a3b41-64c9-45a3-b509-8f93d3f3e824) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (needs >=20)`
- `website/dist/ missing for web server SPA routing`
- `local-sdcpp.ts test fails: 2GB RAM insufficient for video model (needs >=24GB)`
- `Some tsx test files timeout in container (tsx cold start + limited RAM)`

Attempt 2:

- 10 min: `web-server.ts: SPA deep route returns 503 (website/dist not built, no frontend)`
- 5 min: `local-sdcpp.ts: ffmpeg filter 'color=c=red' argument format incompatible with installed ffmpeg version`
- 5 min: `concat-step.ts, e2e-video.ts, verify-video.ts: tests hang (likely ffmpeg/proc deadlock in CI container)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
