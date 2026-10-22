# Audar-ASR-V1

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AudarAI/Audar-ASR-V1, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/audar-asr-v1

## Pinned environment

- Project commit: `9751231eb7c5039441611626840465dab8878174`
- Test commit: `9751231eb7c5039441611626840465dab8878174`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.9 to 26.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 26.2 | 26.9 | 7 | 7 | [run](https://argusic.com/run/842802a6-c3e7-4afd-92a9-504fe998e70d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python environment externally managed - could not install system-wide`
- 5 min: `transformers 5.20.x changed validate_token_ids ordering - Qwen3ASRConfig.thinker_config not set before super().__init__()`
- 2 min: `@check_model_inputs() decorator signature changed in transformers 5.x`
- 5 min: `ROPE_INIT_FUNCTIONS no longer has "default" rope_type key in transformers 5.x`
- 2 min: `Qwen3ASRThinkerConfig missing pad_token_id/eos_token_id attributes`
- 2 min: `cache_position is None in prepare_inputs_for_generation during generation loop`
- 3 min: `create_causal_mask() got unexpected keyword argument in transformers 5.19.x`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
