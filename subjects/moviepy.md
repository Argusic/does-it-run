# moviepy

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Zulko/moviepy, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/moviepy

## Pinned environment

- Project commit: `211e4b15f6ce4f34a6a9efbfff40590e43a68f77`
- Test commit: `211e4b15f6ce4f34a6a9efbfff40590e43a68f77`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 17.7 to 17.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.5 | 17.7 | 2 | 1 | [run](https://argusic.com/run/6cb46cdc-66c5-4a9e-ab4e-659f5e1dc73f) |

## What was observed on a clean machine

Attempt 1:

- `Flaky test: test_write_videofiles_with_temp_audiofile_path fails under full suite run (temp file race), passes in isolation`
- `DeprecationWarning: setting shape on numpy array at moviepy/video/io/ffmpeg_reader.py:228 deprecated in NumPy 2.5`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
