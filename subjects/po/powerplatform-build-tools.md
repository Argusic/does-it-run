# powerplatform-build-tools

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/powerplatform-build-tools, licensed MIT, written in TypeScript.

Evidence and recordings: https://argusic.com/subject/powerplatform-build-tools

## Pinned environment

- Project commit: `6e6fea90d7d117f4c4890fc21612941572e9c766`
- Test commit: `6e6fea90d7d117f4c4890fc21612941572e9c766`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7.4 to 7.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 7 | 7.4 | 3 | 3 | [run](https://argusic.com/run/807ba96f-b582-4cf4-8969-059222d6d8e6) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `npm install failed with E401 - @microsoft/powerplatform-cli-wrapper requires GitHub Packages auth`
- 1 min: `gulp compile crashed with JavaScript heap OOM (2GB default limit exceeded by webpack)`
- `Functional and component tests require PA_BT_ORG_PASSWORD env var (Power Platform credentials)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
