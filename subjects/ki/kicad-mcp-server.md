# KiCAD-MCP-Server

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mixelpixx/KiCAD-MCP-Server, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/kicad-mcp-server

## Pinned environment

- Project commit: `670d2a9c48e1588f2e07edaf656b5e301fc55a50`
- Test commit: `670d2a9c48e1588f2e07edaf656b5e301fc55a50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 5.4 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 5.4 | 1 | 1 | [run](https://argusic.com/run/1136b8b4-ba3e-437e-b2e8-093ce723a58a) |
| 2 | pass with mocks | 92 | 22 | 22 | 3 | 3 | [run](https://argusic.com/run/6807d83b-ef16-4d34-8461-b22eaf176c9d) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python refused pip install (externally-managed-environment)`

Attempt 2:

- 8 min: `Tests/test_project_save_overwrite.py: monkeypatch setattr(SaveBoard) fails after any prior test does delattr on the shared MagicMock. Root cause: bare MagicMock treats setattr+delattr as permanent deletion.`
- 4 min: `Tests/test_add_mounting_hole.py: fresh_pcbnew_mock fixture calls pcbnew.reset_mock() which blows away LIB_ID, FootprintLoad etc. that the module-level __getattr__ had previously created.`
- 3 min: `Tests/test_edit_component_footprint_exchange.py: _make_component_commands calls _pcbnew_stub.reset_mock() which destroys FootprintLoad and LIB_ID.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
