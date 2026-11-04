# ida-pro-mcp

**Verdict: runs with mocks.** Argusic Score 83.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mrexodia/ida-pro-mcp, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ida-pro-mcp

## Pinned environment

- Project commit: `fab3505ee2405ef4e87dcd370418ea7d661f5bdf`
- Test commit: `fab3505ee2405ef4e87dcd370418ea7d661f5bdf`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.7 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 82 | 0.25 | 3.7 | 2 | 1 | [run](https://argusic.com/run/ab0c2e74-4000-4102-85a7-d22c403d3dcf) |
| 2 | pass with mocks | 85.33 | 5 | 4.1 | 3 | 2 | [run](https://argusic.com/run/e1ebccb4-671b-4d04-981e-ff66ab36daa1) |

## What was observed on a clean machine

Attempt 1:

- `ida-mcp-test command fails at import idapro: needs IDA Pro native library (libidalib.so) with IDADIR set`
- `pip install -e .[dev] ignores [dependency-groups.dev] in pyproject.toml; dev deps not auto-installed`

Attempt 2:

- 2 min: `uv binary not on PATH; pip3 install uv needed`
- 1 min: `pip3 install rejected by PEP 668 externally-managed-environment guard`
- `idapro requires libidalib.so from a commercial IDA Pro installation; libidalib.so not present in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
