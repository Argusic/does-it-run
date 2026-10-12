# chatWeb

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/SkywalkerDarren/chatWeb, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/chatweb

## Pinned environment

- Project commit: `2e5e1addf422e587635739fbc590c712beda8271`
- Test commit: `2e5e1addf422e587635739fbc590c712beda8271`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 15.1 to 15.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 20 | 15.1 | 5 | 5 | [run](https://argusic.com/run/ff5cee78-3058-4480-8466-955acd82bf92) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install fails: externally-managed-environment (PEP 668)`
- 1 min: `psycopg2 fails to build: pg_config not found`
- 2 min: `xxhash.xxh3_128_hexdigest() TypeError: xxhash v4 requires bytes not strings`
- 1 min: `demo.launch(show_api=False) TypeError: Gradio 6.x removed show_api parameter`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
