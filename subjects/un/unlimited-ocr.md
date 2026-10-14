# Unlimited-OCR

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/baidu/Unlimited-OCR, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/unlimited-ocr

## Pinned environment

- Project commit: `92ad94b53a51950fea0416aced42331dfb4dd59e`
- Test commit: `92ad94b53a51950fea0416aced42331dfb4dd59e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 14.2 to 14.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 8 | 14.2 | 4 | 4 | [run](https://argusic.com/run/63485185-fc92-40a6-b8e7-70bb866e15bf) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `no uv on machine`
- 22 min: `SGLang server requires CUDA and none is present`
- 12 min: `infer.py crashed with 'SGLang server exited early' even though a healthy server was already up`
- 35 min: `remote-code mock model failed with DynamicCache error, tuple output, missing ModelOutput import, and malformed tokenizer.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
