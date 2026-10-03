# fastrtc

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gradio-app/fastrtc, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/fastrtc

## Pinned environment

- Project commit: `f9395ea2c6515bcb52230de19362ca73e1661855`
- Test commit: `f9395ea2c6515bcb52230de19362ca73e1661855`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 6.6 to 6.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 6.6 | 1 | 1 | [run](https://argusic.com/run/e07b13fe-51aa-49ba-b3de-992b1739a066) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_tts_long_prompt failed: ModuleNotFoundError for 'kokoro_onnx'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
