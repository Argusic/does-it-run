# DLSS5-Swapper

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rakanki911/DLSS5-Swapper, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/dlss5-swapper

## Pinned environment

- Project commit: `24bd2aca7a7451ce94e564366381e33cac9dcdba`
- Test commit: `24bd2aca7a7451ce94e564366381e33cac9dcdba`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 27.6 to 27.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 25 | 27.6 | 5 | 5 | [run](https://argusic.com/run/3eb213c3-dafd-4a60-9395-797515dc1ebb) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `api-override-ipc.test.js: on Linux, main.js install handler calls steam() to find Proton prefix which fails without stubs`
- 5 min: `history-ipc.test.js: same root cause as above`
- 5 min: `backend-profile.test.js: file-journal safePath() does not detect Windows backslash path traversal on Linux`
- 3 min: `payload-guidance.test.js: path.join uses / on Linux, tests expect backslashes`
- 4 min: `shader-compiler.test.js: retireOldShaderCompiler needs SystemRoot pointing to a System32 with D3DCompiler_47.dll`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
