# RAGLight

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Bessouat40/RAGLight, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/raglight

## Pinned environment

- Project commit: `155cee5d8f06685357a2608213493d0cb49d06f3`
- Test commit: `155cee5d8f06685357a2608213493d0cb49d06f3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 5.7 to 9.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 5.7 | 3 | 3 | [run](https://argusic.com/run/b2a58a9a-e5ca-41d7-b703-9edfcf02edd0) |
| 2 | pass with mocks | 92 | 6 | 9.6 | 4 | 4 | [run](https://argusic.com/run/194186f5-0b9c-4487-ab6b-f52779c17b65) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv package manager not available in base Python installation`
- 1 min: `raglight package not installed after 'uv sync --all-extras'`
- 1 min: `Relative import errors when running 'python -m unittest discover' on test subdirectories (from ..test_config import TestsConfig fails when subpackage is not a top-level package)`

Attempt 2:

- 1 min: `uv not on PATH / not installed in unprivileged container`
- 1 min: `raglight package itself not importable after uv sync (module not found)`
- 1 min: `tests failed to import when run as flat discovery because tests use relative imports (..test_config)`
- 1 min: `my initial mock_ollama.py crashed with NameError: name 'true' is not defined`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
