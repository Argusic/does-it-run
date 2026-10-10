# GoModel

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ENTERPILOT/GoModel, licensed MIT, written in Go.

Evidence and recordings: https://argusic.com/subject/gomodel

## Pinned environment

- Project commit: `ce1d38659afbecaad791be5c6a20a5715a723232`
- Test commit: `ce1d38659afbecaad791be5c6a20a5715a723232`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 8.3 to 8.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 8.3 | 3 | 3 | [run](https://argusic.com/run/f25d3c23-5c40-4c58-993b-e82c8582cda6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Go 1.27.1 not installed`
- 1 min: `Frontend static/dist missing for Go embed compilation`
- 2 min: `TestResolveProviders_NoProvidersNoEnvVars failed: OPENROUTER_API_KEY leaked from container env into applyProviderEnvVars`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
