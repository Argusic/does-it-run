# CarConnectivity

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tillsteinbach/CarConnectivity, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/carconnectivity

## Pinned environment

- Project commit: `1e5c1736108d47b543d3b28bbf9a52b057d57fe0`
- Test commit: `1e5c1736108d47b543d3b28bbf9a52b057d57fe0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 13.2 to 13.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 9 | 13.2 | 7 | 7 | [run](https://argusic.com/run/d0dd1be8-b8c7-47a1-8398-2426468bec89) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install refused: externally-managed-environment (PEP 668), no root available`
- 5 min: `initial pip install -e .[all] failed: ResolutionImpossible, plugin/connector pins require carconnectivity>=0.11.10 while repo tree resolves dev versions`
- `mock connector TypeError: BaseConnector.__init__ missing log and api_log`
- 1 min: `mock connector AttributeError: Connector has no attribute log`
- 1 min: `TypeError: You cannot set this attribute. Attribute is not mutable.`
- `first mock fetch did not populate garage (new vehicle each call)`
- `make lint's bare 'flake8' scans .venv site-packages and fails`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
