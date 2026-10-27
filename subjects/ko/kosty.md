# kosty

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kosty-cloud/kosty, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kosty

## Pinned environment

- Project commit: `f3076558cae7e0d119c4128701e2aa1cad3335a5`
- Test commit: `f3076558cae7e0d119c4128701e2aa1cad3335a5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 10.2 to 10.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 10.2 | 4 | 4 | [run](https://argusic.com/run/edc7e87a-3cd0-472f-92e1-fb434efefa48) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip blocked by PEP 668 (externally-managed-environment)`
- 1 min: `moto server mode missing flask (moto[pickle,s3] without [server])`
- 4 min: `kosty iam check-root-access-keys crashed with TypeError: unexpected keyword argument 'org_admin_account_id' (signature missing common options)`
- 5 min: `kosty lb check-no-healthy-targets crashed with TypeError: unexpected keyword argument 'max_workers'/'config_manager'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
