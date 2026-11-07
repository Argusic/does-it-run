# SenseNova-Skills

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/OpenSenseNova/SenseNova-Skills, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/sensenova-skills

## Pinned environment

- Project commit: `5abde96fed2148aaf6a0ed55f0f4708f2b0845f5`
- Test commit: `5abde96fed2148aaf6a0ed55f0f4708f2b0845f5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 4.3 to 26.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 26 | 26.3 | 6 | 6 | [run](https://argusic.com/run/beee99fd-f9d0-4503-ab84-3231721d5cee) |
| 2 | pass with mocks | 92 | 34 | 4.3 | 2 | 2 | [run](https://argusic.com/run/cb6ecdd2-5c7d-4174-9078-41af700e3846) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Python PEP 668 externally-managed-environment blocked pip install`
- 4 min: `npm EACCES permission denied for global install`
- 2 min: `openclaw requires Node >=24.16, system had 18.19`
- 2 min: `Mock HTTP server process died when backgrounded via &, curl returned connection refused`
- 3 min: `Image gen client rejected data: URL protocol from mock`
- `PPT export tests: 2/11 fail (browser version mismatch - tests expect chromium-1208, installed is 1243)`

Attempt 2:

- 2 min: `pip install failed because OS Python environment is externally managed (PEP 668)`
- 18 min: `npm test failed on 3 tests because Playwright browser binaries were missing`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
