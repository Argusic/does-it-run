# ragflow

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/infiniflow/ragflow, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ragflow

## Pinned environment

- Project commit: `313ca90f6abd7682fe8523e16fd67b3653a3fa84`
- Test commit: `313ca90f6abd7682fe8523e16fd67b3653a3fa84`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 26.4 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 80 | 39.7 | 7 | 7 | [run](https://argusic.com/run/10bc0432-eb19-4d88-8cab-c3208f5e1066) |
| 2 | pass with mocks | 92 | 25 | 26.4 | 4 | 4 | [run](https://argusic.com/run/5d1fb3c9-06af-4673-bdf2-9933f63e3f3d) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Missing clang++ (required by build.sh)`
- 2 min: `Missing ld.lld (required to link Chromium-built pdfium)`
- 3 min: `Missing libpcre2-8.a (required by C++ tokenizer static library)`
- 2 min: `Missing cmake >= 4.0 (CMakeLists.txt requires 4.0)`
- 2 min: `Frontend build required node >= 20.19 (system had 18.19)`
- 1 min: `Frontend build OOM with default Node heap`
- `Python SDK module missing for 4 test files`

Attempt 2:

- 5 min: `graspologic dependency from gitee.com unreachable`
- 5 min: `pytest config options asyncio_default_fixture_loop_scope and asyncio_mode not supported by installed pytest-asyncio 1.3.0`
- 10 min: `Go tests cannot build: ld.lld not found and librag_tokenizer_c_api.a not prebuilt`
- `quart-auth 0.11.0 incompatible with quart 0.23.1 (request_ctx removed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
