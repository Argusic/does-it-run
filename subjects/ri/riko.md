# riko

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nerevu/riko, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/riko

## Pinned environment

- Project commit: `dcfa9f2bd4ba0c6da5646cd9842d9e2d3630eb8f`
- Test commit: `dcfa9f2bd4ba0c6da5646cd9842d9e2d3630eb8f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 25.9 to 25.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 25.9 | 7 | 7 | [run](https://argusic.com/run/801e4c53-fe78-4e67-88c6-3a69d015b31a) |

## What was observed on a clean machine

Attempt 1:

- 0.1 min: `Missing tzdata package for zoneinfo timezone data`
- 0.1 min: `pytest binary not found by manage.py test CLI (shutil.which fails in .venv)`
- 2 min: `Ruff 0.16.5 formatting drift: multi-line imports, Literal quote style, trailing comma handling changed vs committed generated files`
- 0.5 min: `run-pipe and benchmark scripts not in PATH for subprocess tests`
- 0.1 min: `test_codegen_renders_top_level_count expected double-quoted count="first" but ruff 0.16.5 outputs single-quoted count='first'`
- 0.1 min: `Hash-dependent doctests and tests fail without PYTHONHASHSEED set`
- 0.2 min: `Three pipeline JSON files with pipe:<hash> namespace references generate invalid Python (colon in identifier)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
