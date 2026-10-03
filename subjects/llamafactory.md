# LlamaFactory

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hiyouga/LlamaFactory, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/llamafactory

## Pinned environment

- Project commit: `d6bb97ddff5d752d8b05aa099a168127c7253562`
- Test commit: `d6bb97ddff5d752d8b05aa099a168127c7253562`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 13.6 to 39.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 8.5 | 26.6 | 0 | 0 | [run](https://argusic.com/run/39fbf7c5-70e4-4832-bdfa-6d2ed3b7d399) |
| 2 | pass | 100 | 30 | 13.6 | 0 | 0 | [run](https://argusic.com/run/1ef51cb2-b762-4ef2-b663-1ffebaf724d0) |
| 3 | pass with mocks | 92 | 16 | 39.7 | 4 | 4 | [run](https://argusic.com/run/b54e9553-3795-4fa6-8493-96e26754d088) |

## What was observed on a clean machine

Attempt 3:

- `No CUDA GPU available; torch.cuda.is_available() returned False`
- `Tests requiring large model downloads (Qwen3-8B, Gemma-4, Phi-4) hang due to download time/size`
- `test_render_messages_remote requires downloading 'llamafactory/v1-sft-demo' dataset from Hugging Face hub, which hangs`
- `tests/model/, tests/train/, tests/e2e/ require model forward passes that are too slow on CPU (tiny model forward pass times out at 30s)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
