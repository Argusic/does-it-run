# panel-graphic-walker

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/panel-extensions/panel-graphic-walker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/panel-graphic-walker

## Pinned environment

- Project commit: `2a892dc62b3ebfc5c658e5df280e92a418e07c16`
- Test commit: `2a892dc62b3ebfc5c658e5df280e92a418e07c16`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 9.8 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 10 | 9.8 | 4 | 4 | [run](https://argusic.com/run/0343f600-73f6-4a7c-ab51-2c923e52110b) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `Externally managed Python environment blocks system-wide pip install`
- 6 min: `hatchling build hook requires esbuild and fails with npm peer dependency conflict (@kanaries/graphic-walker requires react>=19.0.0 but panel pins react@18.3.1)`
- 1 min: `ModuleNotFoundError: editables, ibis-framework, aiohttp`
- `test_graphic_walker_apps.py: exec_with_return does not set __file__, causing NameError in examples using Path(__file__).parent`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
