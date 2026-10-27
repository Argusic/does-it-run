# Libra

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NetX-lab/Libra, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/libra

## Pinned environment

- Project commit: `a1e1619144b67abcc9f65fb3e325a096106c1e09`
- Test commit: `a1e1619144b67abcc9f65fb3e325a096106c1e09`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28 to 28 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 28 | 7 | 7 | [run](https://argusic.com/run/6673d5e8-5a5d-459d-a7f3-581e4388123b) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `examples/test_single_gpu.py tried to write to hardcoded /path/to/user/test_weights (PermissionError)`
- 5 min: `examples/test_code_agent.py imported extract_code_block from wrong module (code_executor has it as a method, module-level fn is in code_reward)`
- 2 min: `examples/test_code_agent.py test_code_agent_workflow used deprecated asyncio.get_event_loop() (RuntimeError: no event loop in thread)`
- 1 min: `requirements.txt pyarrow>=15.0.0 resolved to pyarrow 26 which requires numpy>=2, conflicting with repo's pinned numpy<2.0`
- 1 min: `tests/conftest.py missing , 3 test files (homogeneous_rollout_baseline, production_ehp_ab_config, r2e_patch_harness) import from scripts/ and env/ top-level dirs not on sys.path`
- `cmake==3.26.4 has no cp312 wheel (only py2.py3-none tags); pip reports 'not supported on this platform'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
