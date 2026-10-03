# harness-anything

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yb2460/harness-anything, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/harness-anything

## Pinned environment

- Project commit: `dcb3e516dee1e7b4c83e1909a07062a0bb8dea0a`
- Test commit: `dcb3e516dee1e7b4c83e1909a07062a0bb8dea0a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 22.9 to 27.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 55 | 27.5 | 6 | 6 | [run](https://argusic.com/run/899e54bf-3b77-44c7-a049-33258fc66b81) |
| 2 | pass | 100 | 1 | 22.9 | 3 | 3 | [run](https://argusic.com/run/b1ac7df6-03c2-42c8-9980-c0ef37e07a73) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Externally-managed Python environment blocked system pip`
- 8 min: `6 Zotero import tests failed: _resolve_target made real HTTP calls when no collection_ref given`
- 5 min: `4 Zotero test_agent_harness tests failed: wrong HARNESS_ROOT level and missing files`
- 5 min: `11 Photoshop tests failed: unconditional import pythoncom (Windows-only)`
- 10 min: `Illustrator setup.py broken: referenced non-existent README, wrong package`
- 3 min: `Illustrator project.py + Photoshop export.py unconditional COM imports`

Attempt 2:

- `Zotero agent_harness tests expected missing packaging files`
- `Zotero ImportCoreTests 6 failures due to missing get_selected_collection HTTP mock`
- `Photoshop tests failed: pythoncom/pywintypes missing (Windows-only deps)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
