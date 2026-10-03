# ppt-master

**Verdict: runs.** Argusic Score 73.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hugohe3/ppt-master, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ppt-master

## Pinned environment

- Project commit: `d3d81fe3cf4cc642de225159586308bbe98eeb4d`
- Test commit: `d3d81fe3cf4cc642de225159586308bbe98eeb4d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 3; wall time 15 to 77.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4.5 | 77.9 | 2 | 2 | [run](https://argusic.com/run/ee5839ab-f155-4a2d-be53-c0a917cc9b11) |
| 2 | pass | 100 | 14 | 15 | 1 | 1 | [run](https://argusic.com/run/81481ce7-97ca-4d42-9d3c-c016fe0b9409) |
| 3 | fail | 20 | n/a | 21.6 | 0 | 0 | [run](https://argusic.com/run/506978f5-3c43-46f4-9222-6643cd803791) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `pip install failed due to externally-managed-environment (Debian Python PEP 668)`
- 12 min: `Batch pytest collection fails on test_native_export_guards.py due to module/package name collision (svg_to_pptx.py flat file shadows svg_to_pptx/ package), breaking relative imports in svg_to_pptx/animation_config.py`

Attempt 2:

- `test_native_export_guards.py collection fails under full 'pytest tests/' suite due to a relative-import in svg_to_pptx/animation_config.py that depends on package context , 37 tests pass when the file is run individually`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
