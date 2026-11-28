# kinocut

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KyaniteLabs/kinocut, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/kinocut

## Pinned environment

- Project commit: `2c7cd936e9b6da28fc9d042ab211125d7acaf79f`
- Test commit: `2c7cd936e9b6da28fc9d042ab211125d7acaf79f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 57.8 to 57.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 57.8 | 1 | 1 | [run](https://argusic.com/run/bd119ed0-a69b-4040-bec5-f567cca32fef) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_compat_matrix_skeleton.py::test_cli_ground_truth_run_end_to_end failed initially because OPENROUTER_API_KEY was set in the container environment, which the receipt writer's detect_cloud_keys() treats as a cloud credential`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
