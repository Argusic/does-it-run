# douyin-to-obsidian

**Verdict: runs with mocks.** Argusic Score 72 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/llm-xiaoye/douyin-to-obsidian, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/douyin-to-obsidian

## Pinned environment

- Project commit: `eba5f7482585f180f867024f400b5680ab9950f7`
- Test commit: `eba5f7482585f180f867024f400b5680ab9950f7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 3 to 3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 72 | 4 | 3 | 3 | 0 | [run](https://argusic.com/run/944cfefa-7529-451c-9d6f-3490f4a20c55) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `mlx-metal==0.32.2 not installable on Linux x86_64 (macOS Apple Silicon dependency)`
- 0.5 min: `Chrome browser not available on Linux for cookie-based Douyin access`
- 0.5 min: `Swift/Xcode not available on Linux for Apple Vision OCR`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
