# Adrian

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/secureagentics/Adrian, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/adrian

## Pinned environment

- Project commit: `73c6c1c41f2e87a9070ef4fd62a00421d8ad2fcf`
- Test commit: `73c6c1c41f2e87a9070ef4fd62a00421d8ad2fcf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.3 to 17.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 19 | 17.9 | 6 | 6 | [run](https://argusic.com/run/743335ef-3b8a-4f25-a4a8-299b5b70d0aa) |
| 2 | pass | 100 | 5.2 | 8.3 | 4 | 4 | [run](https://argusic.com/run/c5512876-e4d0-4bcf-9804-d927ef05dc54) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not on PATH (installed in user site-packages)`
- 2 min: `Go not available; required for backend compilation`
- 1 min: `setup.py bootstrap failed: migrations not found at /app/migrations`
- 1 min: `setup.py bootstrap failed: GGUF file not found`
- `TypeScript SDK tests cannot run: Node 18 lacks styleText and vitest requires Node >=20`
- `Frontend standalone server name resolution (hostname not 127.0.0.1)`

Attempt 2:

- 0.5 min: `uv not on PATH after pip install (no shell reload)`
- 0.5 min: `uv venv created without pip binary`
- 1 min: `Go compiler not found in container`
- 0.5 min: `No root for apt system packages`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
