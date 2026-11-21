# Rapid-MLX

**Verdict: runs with mocks.** Argusic Score 85.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/raullenchai/Rapid-MLX, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/rapid-mlx

## Pinned environment

- Project commit: `d50fd75b778e34b69c47782484813bb67289a479`
- Test commit: `d50fd75b778e34b69c47782484813bb67289a479`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 23.3 to 79.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 78.67 | 9.7 | 79.5 | 3 | 1 | [run](https://argusic.com/run/2ef712cb-2a83-4eab-a821-5b21f4fbb8dd) |
| 2 | pass with mocks | 92 | 0.5 | 23.3 | 5 | 5 | [run](https://argusic.com/run/f8774a65-fe3c-40fa-ab7b-08759544fdba) |

## What was observed on a clean machine

Attempt 1:

- 35 min: `tests/headless_mlx/conftest.py installs MLX stubs but find_spec returns True for pip-installed mlx even when libmlx.so cannot load on Linux x86_64, causing 51 collection errors`
- `test_audio_path_shaped_model.py fails with 503 instead of 404 on Linux , pre-existing test design issue; the mlx-audio runtime cannot import on Linux so the server returns 503 (service unavailable) for audio routes instead of 404 for unknow`
- `test_version_check.py has 2 pre-existing failures in symlink detection checks , environment-specific test logic assumes specific pip install path patterns`

Attempt 2:

- `MLX shared library (libmlx.so) not available on Linux x86_64 , this project requires Apple Silicon macOS for inference`
- `test_version_check.py: two tests failed due to Linux symlink detection differences`
- `test_vllm_mlx_shim.py: shim star-import triggers mlx.core import`
- `test_grammar_processor_558.py: 13 failures/8 errors , grammar processor fixtures import mlx.core`
- `193 test files collect with import errors due to top-level mlx.core imports`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
