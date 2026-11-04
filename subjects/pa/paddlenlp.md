# PaddleNLP

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PaddlePaddle/PaddleNLP, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/paddlenlp

## Pinned environment

- Project commit: `3f87dac9b719f75399f92f8bf634ae2ef0611832`
- Test commit: `3f87dac9b719f75399f92f8bf634ae2ef0611832`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8 to 21.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 7 | 8 | 0 | 0 | [run](https://argusic.com/run/f15af7c4-3312-412a-adfa-2259ed1e7adc) |
| 2 | pass | 100 | 1.5 | 21.8 | 2 | 2 | [run](https://argusic.com/run/f3512285-71da-4ef3-9b8f-67c126664f93) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `huggingface_hub 2.4.0 removed 'repo_type_and_id_from_hf_id' API; import fails at startup`
- 0.5 min: `test_glue.py PearsonAndSpearman.assertEqual fails on float rounding (0.9985229081857803 vs 0.9985229081857804)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
