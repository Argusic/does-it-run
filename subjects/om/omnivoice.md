# OmniVoice

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/k2-fsa/OmniVoice, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/omnivoice

## Pinned environment

- Project commit: `08be0b4ccbac3e13e374e86fbfead4b4cac343e2`
- Test commit: `08be0b4ccbac3e13e374e86fbfead4b4cac343e2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 5.4 to 18 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 17.6 | 18 | 4 | 4 | [run](https://argusic.com/run/9d884d5d-8b02-4d6a-9fe7-a75b2c88da20) |
| 2 | pass | 100 | 5 | 5.4 | 4 | 4 | [run](https://argusic.com/run/c8d50ca3-9b4f-490f-8beb-c3cdfdeecb13) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip install failed: externally-managed-environment`
- 1 min: `LoRA tests failed: ModuleNotFoundError: No module named 'peft'`
- 2 min: `test_merge_lora_produces_deployable_model failed: audio_tokenizer not found in test checkpoint`
- 1 min: `test_merge_lora failed: shutil.copytree error from broken symlink in audio_tokenizer dir`

Attempt 2:

- 1 min: `pip install --user uv failed with externally-managed-environment (PEP 668)`
- 1 min: `huggingface_hub module path huggingface_hub.commands.huggingface_cli did not exist`
- 1 min: `pytest was not installed by the project`
- 3 min: `uv sync --locked rejected the committed uv.lock; lock also pinned omnivoice 0.1.5 while pyproject is 0.2.1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
