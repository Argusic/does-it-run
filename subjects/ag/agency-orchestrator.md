# agency-orchestrator

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jnMetaCode/agency-orchestrator, licensed Apache-2.0, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/agency-orchestrator

## Pinned environment

- Project commit: `bed66133356bd859f4bf7459c0a9ed5580fb2203`
- Test commit: `bed66133356bd859f4bf7459c0a9ed5580fb2203`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 49.3 to 49.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 49.3 | 4 | 4 | [run](https://argusic.com/run/c581b920-ebd6-4cfb-902a-0872bdb359bd) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Node.js v18.19.1 too old (needs >=20)`
- `website/dist/ missing for web server SPA routing`
- `local-sdcpp.ts test fails: 2GB RAM insufficient for video model (needs >=24GB)`
- `Some tsx test files timeout in container (tsx cold start + limited RAM)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
