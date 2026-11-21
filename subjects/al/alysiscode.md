# AlysisCode

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/AlysisAi/AlysisCode, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/alysiscode

## Pinned environment

- Project commit: `e2d5d4df2201db324658500fdcb05d347440c29d`
- Test commit: `e2d5d4df2201db324658500fdcb05d347440c29d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 9.8 | 2 | 2 | [run](https://argusic.com/run/392a5a44-5765-4733-b34d-89a534fc3203) |

## What was observed on a clean machine

Attempt 1:

- `test_turn_end_file_evidence.py::test_removing_files_git_does_not_track_ends_the_turn - fs_delete on untracked files did not remove them`
- `test_turn_end_file_evidence.py::test_one_missing_file_in_a_list_does_not_undo_the_others - fs_delete with missing file in list failed to delete present files`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
