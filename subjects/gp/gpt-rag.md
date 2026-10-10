# GPT-RAG

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Azure/GPT-RAG, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/gpt-rag

## Pinned environment

- Project commit: `324df2c24620c534ebb353c54eff6050ebb2f5ef`
- Test commit: `324df2c24620c534ebb353c54eff6050ebb2f5ef`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 6.3 to 6.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 18 | 6.3 | 3 | 3 | [run](https://argusic.com/run/587e8582-a0e6-4078-afe5-6516c5d7fe44) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `util/requirements.txt and config/requirements.txt pin conflicting azure-identity versions (1.23.0 vs 1.25.3), and pip-re Installing both files fails with ResolutionImpossible`
- 3 min: `scripts/postProvision.sh and scripts/preDeploy.sh report syntax errors under 'sh -n'`
- 4 min: `PowerShell 7 (pwsh) and Azure CLI (az)/azd are not installed in the container; hook tests for pwsh are skipped and live azd provisioning cannot run (no root to install)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
