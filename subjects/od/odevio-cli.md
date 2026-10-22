# Odevio-CLI

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Odevio/Odevio-CLI, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/odevio-cli

## Pinned environment

- Project commit: `f54272e6005c8553cb8b11582d412cd869077f31`
- Test commit: `f54272e6005c8553cb8b11582d412cd869077f31`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 43.3 to 43.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 42 | 43.3 | 8 | 8 | [run](https://argusic.com/run/8c5ef56f-35aa-404f-b181-d9f2f3c7c3a8) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `externally-managed-environment blocked system pip install`
- 1 min: `missing tests/fixture.py (gitignored)`
- 15 min: `no mock backend - tests call production URL`
- 3 min: `415 Unsupported Media Type from Flask expecting JSON when client sends form-encoded`
- 2 min: `204 empty body caused JSON decode errors in cleanup`
- 1 min: `mock key generation (T001) mismatched test expectation (001)`
- 2 min: `prompt() calls blocked in non-TTY test runner`
- 3 min: `output format mismatches between mock 403 handler and test expectations`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
