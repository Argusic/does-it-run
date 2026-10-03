# astron-rpa

**Verdict: runs.** Argusic Score 88.2 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/iflytek/astron-rpa, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/astron-rpa

## Pinned environment

- Project commit: `1becb94dab8de093655d60c5a89a1ce9ec455ad6`
- Test commit: `1becb94dab8de093655d60c5a89a1ce9ec455ad6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services, no run possible
- Valid runs: 3; wall time 9.1 to 22.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 2 | pass | 100 | 14 | 22.1 | 11 | 11 | [run](https://argusic.com/run/3c2fc22e-4410-4f0b-80e4-ab503dfd4b9a) |
| 2 | pass with mocks | 84.73 | 12 | 9.1 | 11 | 7 | [run](https://argusic.com/run/bd51cbd1-7ce9-4832-bc5e-e068585b79d2) |
| 3 | fail | 80 | 22 | 9.8 | 11 | 11 | [run](https://argusic.com/run/03b42d69-76f6-4d73-9a94-6e36fee73057) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `Engine requires Python >=3.13, but container has Python 3.12`
- 1 min: `uv package manager not available`
- 2 min: `pnpm 9+ requires Node >=22, container has Node 18`
- 2 min: `Engine test_string.py: fill_string_to_length RIGHT uses str-as-int for slice index`
- `Engine test_data.py: missing Ciphertext class and get_shared_variable method (not implemented)`
- `Engine test_list.py, test_math.py: missing module implementation for random number with count`
- `Engine test_script.py: Script.module() API incompatibility (__env__ kwarg not supported)`
- `Engine test_encrypt.py: test_base64_encode uses local file path './a.txt' that doesn't exist`
- `Backend Python services (ai-service, openapi-service) require MySQL and Redis with real credentials`
- `Frontend electron-app postinstall fails - electron can't download/install in Linux container`
- `Frontend browser-plugin tests: 7/30 fail due to locale mismatch (Chinese vs English error messages)`

Attempt 2:

- 1 min: `uv not installed - required for engine and Python services`
- 3 min: `Node.js 18 too old; project requires >=22`
- 1 min: `pnpm not installed`
- 1 min: `electron-app postinstall fails - no Electron binary on Linux`
- 1 min: `Python 3.12 present, engine requires >=3.13`
- 1 min: `test.xlsx missing for openpyxl tests`
- 1 min: `a.txt missing for base64_encode test`
- `winreg import fails on Linux (browser-plugin test)`
- `Script.module() tests pass __env__ kwarg not accepted by function signature`
- `Various frontend debugger tests fail - chrome.debugger API not available in Node test runner`
- `Backend service tests need MySQL/Redis containers`

Attempt 3:

- 1 min: `Python 3.12 is system default, project requires >=3.13`
- 1 min: `uv package manager not found`
- 2 min: `pnpm not found (npm global install blocked by EACCES)`
- 3 min: `Node.js v18 installed, project requires >=22`
- 1 min: `Externally-managed Python env blocked pip install of uv`
- 1 min: `Test directories missing __init__.py causing pytest ModuleNotFoundError`
- `Engine tests: 21 pre-existing failures, 7 pre-existing errors (missing methods on DataProcess, missing pytest fixtures, undefined variables, missing test data files)`
- `Frontend tests: 7 pre-existing failures in background.debugger.test.js (mocked Chrome Debugger protocol tests)`
- `Docker not available in container`
- `Java JDK/Maven not installed`
- `Backend Python services (ai-service, openapi-service) require MySQL, Redis, and third-party API keys (AICHAT, XFYUN, JFBYM, CUA) at import time`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
