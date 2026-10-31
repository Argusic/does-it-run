# vcspull

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/vcs-python/vcspull, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vcspull

## Pinned environment

- Project commit: `8dc40abfa5201622c7c5aa3bb8db2f366de9cba8`
- Test commit: `8dc40abfa5201622c7c5aa3bb8db2f366de9cba8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 7.1 to 7.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 7.1 | 2 | 2 | [run](https://argusic.com/run/26260b90-c0cd-4340-bf46-32dd0e20a49d) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `pip install failed: externally-managed-environment prevents system-wide Python package installation`
- 0.5 min: `2 doctest failures: CodeCommitImporter requires aws CLI, runtime_dep_smoketest.exercise_cli requires vcspull on subprocess PATH`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
