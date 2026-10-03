# memory-os

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ClaudioDrews/memory-os, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/memory-os

## Pinned environment

- Project commit: `e03db1f1c83e94fdb2007c90d232c6c852c0f274`
- Test commit: `e03db1f1c83e94fdb2007c90d232c6c852c0f274`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 8.1 to 35.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 8.1 | 3 | 3 | [run](https://argusic.com/run/9a5c4a80-c986-4aad-b49e-02a5af7bf280) |
| 2 | pass with mocks | 92 | 3 | 35.2 | 5 | 5 | [run](https://argusic.com/run/8cdf3bee-d3a6-43c2-97f9-a021776fc758) |

## What was observed on a clean machine

Attempt 1:

- `Docker not available - cannot start Qdrant, Redis, or ARQ worker`
- `Hermes Agent not installed - cannot load Icarus plugin in its intended runtime`
- `pip install blocked by externally-managed-environment (Debian PEP 668)`

Attempt 2:

- 3 min: `state.py _parse_frontmatter_scalar returns YAML-quoted strings when yaml unavailable (outside venv) , causes has_entry_ref to fail`
- 1 min: `parsing.py fallback YAML parser doesn't strip double quotes from values`
- 1 min: `obsidian.py 'from .state import _parse_head' fails when loaded standalone via importlib.util`
- 2 min: `fabric-retrieve.py SQLite index stores empty 'title' column instead of frontmatter 'summary'`
- 1 min: `test-plugin.sh subprocess.run hardcodes 'python3' which lacks venv deps (yaml library)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
