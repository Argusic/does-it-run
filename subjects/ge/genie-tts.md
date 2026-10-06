# Genie-TTS

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/High-Logic/Genie-TTS, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/genie-tts

## Pinned environment

- Project commit: `d347fd0f8683e9a362b69f59fa0a4799ddb5e828`
- Test commit: `d347fd0f8683e9a362b69f59fa0a4799ddb5e828`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.5 to 9.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 38 | 9.5 | 3 | 3 | [run](https://argusic.com/run/a2f16490-db32-4c28-8744-dd831f6f0b69) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `jieba_fast build failed: Python.h not found (python3-dev not installed, cannot install system packages)`
- 3 min: `eunjeon build failed: mecab-config not found`
- 2 min: `onnxruntime 1.30.0 (default install) pthread_setaffinity_np warnings in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
