# capsule-cinema

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JuneYaooo/capsule-cinema, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/capsule-cinema

## Pinned environment

- Project commit: `7d3a1083072013d535610a32aa9e7752f48ed8f0`
- Test commit: `7d3a1083072013d535610a32aa9e7752f48ed8f0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 4.1 to 4.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 4.1 | 3 | 3 | [run](https://argusic.com/run/fd99b20f-084e-407e-8708-43999eb6fddc) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `rsync not found , install_as_skill.sh failed with exit 127`
- 5 min: `Python externally-managed environment blocks system pip install`
- `capsule_consistency_lint reports 1 FAIL in x_lai_animal_fable.capsule (production_capabilities not subset of capabilities)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
