# VibeVoice

**Verdict: runs.** Argusic Score 94 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/microsoft/VibeVoice, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vibevoice

## Pinned environment

- Project commit: `16fb2cb1217c9934a886e1948ffb06120caa2df5`
- Test commit: `16fb2cb1217c9934a886e1948ffb06120caa2df5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 17.3 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 13 | 17.3 | 3 | 3 | [run](https://argusic.com/run/689470ae-83af-4123-b0ab-231d32bc4d9d) |
| 2 | pass | 96 | 2 | 26.9 | 5 | 4 | [run](https://argusic.com/run/976c2c51-e806-45e0-821a-0a3227255265) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip install -e . refused on system Python: externally-managed-environment (PEP 668)`
- 4 min: `Gradio launch produced empty log and exited when started from a non-interactive shell (first attempt)`

Attempt 2:

- 1 min: `'python' and the 'time' shell utility were absent; creating a virtualenv at /work/venv failed with permission denied.`
- 9 min: `Bundled voice presets failed safe torch.load because BaseModelOutputWithPast and the legacy DynamicCache layout were incompatible with PyTorch 2.6+/Transformers 4.57.`
- 1 min: `ASR CLI --help crashed because torch.backends.xpu did not exist in the installed PyTorch.`
- 3 min: `Real ASR checkpoint tokenizer rejected its list-valued extra_special_tokens under Transformers 4.57.`
- 6 min: `Real 7B ASR checkpoint load was OOM-killed in float32 and BFloat16 because the container cgroup is limited to 8 GB and the checkpoint is 15.5 GB.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
