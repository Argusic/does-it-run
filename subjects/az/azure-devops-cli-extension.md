# azure-devops-cli-extension

**Verdict: runs with mocks.** Argusic Score 84.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azure/azure-devops-cli-extension, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/azure-devops-cli-extension

## Pinned environment

- Project commit: `4d49a4b367fdba19442bfccf07e9516a8a3dd857`
- Test commit: `4d49a4b367fdba19442bfccf07e9516a8a3dd857`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 4.9 to 67.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 8 | 4.9 | 0 | 0 | [run](https://argusic.com/run/40da9812-5b30-4707-8d56-f9ea7ec7a142) |
| 2 | pass with mocks | 88.67 | 30 | 67.7 | 6 | 5 | [run](https://argusic.com/run/391f8a70-ee20-4847-a943-44cab75ee3b0) |

## What was observed on a clean machine

Attempt 2:

- 5 min: `dev_setup.py requirements omitted azure-cli-testsdk and msrestazure needed by the test suite`
- 5 min: `azure-cli-testsdk uses inspect.getargspec which Python 3.12 removed`
- 30 min: `VCR integration recordings reference old API URL shapes and replay fails against the current generated SDK`
- 10 min: `SDK OPTIONS/cache route templates lacked project-scoped paths for git/wit/refs/imports, so URLs omitted the project segment`
- 15 min: `Mock lacked correct semantics for work items (AreaPath project, id propagation, delete 404), refs filter, import request route variants, and policy endpoints`
- `23 integration scenarios (pipelines, wiki, security, boards query/relation/area/iteration, team, user, invoke, PR policies/reviewers, variable groups) still fail against the mock`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
