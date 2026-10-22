# deepgram-python-sdk

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/deepgram/deepgram-python-sdk, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/deepgram-python-sdk

## Pinned environment

- Project commit: `c7c1b3fac4be6e08bb43475d82545cbea5974602`
- Test commit: `c7c1b3fac4be6e08bb43475d82545cbea5974602`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 30 | 7 | 4 | 4 | [run](https://argusic.com/run/7399c44a-9335-42ef-8399-76adb253d510) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install --user poetry blocked: externally-managed-environment (PEP 668), and no root`
- 1 min: `python3 -m venv /work/venv failed: Permission denied on /work`
- 22 min: `pytest aborted at startup: tests/conftest.py launches WireMock via 'docker compose', but docker and java are absent in the container`
- `mock bugs during bring-up: path-template regex mis-ordered escaping (unbalanced parenthesis), double body read on /__admin/requests/find (BrokenPipe), and hasExactly matcher compared the whole list instead of per item`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
