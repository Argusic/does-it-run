# fontbakery

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/fonttools/fontbakery, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/fontbakery

## Pinned environment

- Project commit: `9a85e003d36ebfbbfe68c6d362e5db5a6434332c`
- Test commit: `9a85e003d36ebfbbfe68c6d362e5db5a6434332c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.8 to 3.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 3.8 | 1 | 1 | [run](https://argusic.com/run/d944e863-1761-4af0-8dac-edec28107e8d) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_checks_opentype_cff.py::test_check_cff_strings failed with AttributeError: charset - newer fontTools no longer raises UnicodeDecodeError for CFF fonts with non-ASCII strings, so cff_analysis condition tries to access CharStrings which`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
