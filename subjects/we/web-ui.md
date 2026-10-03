# web-ui

**Verdict: runs with mocks.** Argusic Score 80.6 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/browser-use/web-ui, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/web-ui

## Pinned environment

- Project commit: `61962296c38a0d064e0ba02c827192b7a81d1819`
- Test commit: `61962296c38a0d064e0ba02c827192b7a81d1819`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 16.2 to 16.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 80.57 | 3 | 16.2 | 7 | 3 | [run](https://argusic.com/run/c525a635-374e-4f88-b415-b6019e7c4ad0) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python 3.12 removed distutils - browser_settings_tab.py used from distutils.util import strtobool`
- 1 min: `test_llm had parameter 'config' which pytest treated as a missing fixture`
- 5 min: `LLM API tests failed because no API keys were configured`
- `Google test still fails (test_google_model) - uses gRPC to real Google servers not mockable via HTTP`
- `IBM test fails (test_ibm_model) - requires WATSONX_USERNAME and talks to real IBM cloud, pydantic validation fails before any request`
- `test_connect_browser uses headless=False and empty user_data_dir causing EACCES on empty path`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
