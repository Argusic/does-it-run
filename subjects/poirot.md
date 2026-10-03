# poirot

**Verdict: runs with mocks.** Argusic Score 56 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HezaoHezao/poirot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/poirot

## Pinned environment

- Project commit: `86bf279ad90c180f0ba696755620dd7d6661465e`
- Test commit: `86bf279ad90c180f0ba696755620dd7d6661465e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 27.2 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 27.2 | 0 | 0 | [run](https://argusic.com/run/19250f1c-0824-4321-aeba-70c02d0b7965) |
| 2 | pass with mocks | 92 | 30 | 29.7 | 6 | 6 | [run](https://argusic.com/run/0756d27d-8cd8-4f13-9042-a20a61c9e23d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `test_expert_mode_true_activates_profile expected max_loop_steps==8 but EXPERT_PROFILE sets it to 100`
- 2 min: `test_call_llm_uses_prompt_template expected Chinese prompt text but template was English`
- 8 min: `cross-test shutil.which mock leak caused pi_installer tests to fail`
- 2 min: `test_windows_msvcrt failed because msvcrt attr doesn't exist on Linux`
- 1 min: `test_initial_state_field_count missing recalled_memories and memory_updates keys`
- 4 min: `test_bash_output_truncation used python not python3 (exit code 127)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
