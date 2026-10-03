# Vision-Agents

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/GetStream/Vision-Agents, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/vision-agents

## Pinned environment

- Project commit: `902db86438aab03fb64aa7e6ea3afdcc867a3e80`
- Test commit: `902db86438aab03fb64aa7e6ea3afdcc867a3e80`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 41.9 to 41.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 41.9 | 3 | 3 | [run](https://argusic.com/run/dd9710f3-bd53-473a-aa0c-349300a3de1a) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `No space left on device while extracting torch/CUDA/nvidia wheels (triton, nvidia-cublas, torch) during full uv sync --all-extras --dev`
- 2 min: `Docker daemon not available , 10 tests in test_agent_launcher.py and 16 tests in test_redis_store.py raise DockerException on collection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
