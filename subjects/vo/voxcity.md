# VoxCity

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kunifujiwara/VoxCity, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/voxcity

## Pinned environment

- Project commit: `fa212656305328a9a657973bae26f352bfe813bc`
- Test commit: `fa212656305328a9a657973bae26f352bfe813bc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 15.2 to 19.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 15.2 | 0 | 0 | [run](https://argusic.com/run/62929487-aa0b-4296-ad6c-c2909e7f519f) |
| 2 | pass | 100 | 6 | 19.2 | 3 | 3 | [run](https://argusic.com/run/84a7dbad-c172-4c24-863e-7e06e0196bcc) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `ModuleNotFoundError: No module named taichi on collection of simulator_gpu tests`
- 2 min: `ImportError: No boolean backend for trimesh (pip install manifold3d or blender)`
- 1 min: `ValueError could not convert string to float 'a' in ad-hoc solar test (Astral returns DataFrame, not tuples)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
