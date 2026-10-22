# cmd2

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/python-cmd2/cmd2, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/cmd2

## Pinned environment

- Project commit: `579d47c162f1aeff2bfb300ecfbd93f28411429e`
- Test commit: `579d47c162f1aeff2bfb300ecfbd93f28411429e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.7 to 3.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 3.7 | 1 | 1 | [run](https://argusic.com/run/34369868-c004-44c7-83ea-da45daf7742c) |

## What was observed on a clean machine

Attempt 1:

- 1.5 min: `test_find_editor_not_specified failed because no common editors (vim, vi, emacs, nano, etc.) exist in this container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
