# Windows-MCP

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/CursorTouch/Windows-MCP, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/windows-mcp

## Pinned environment

- Project commit: `1ea8690a6d9bfa55abb24d534f6a30590acf47d5`
- Test commit: `1ea8690a6d9bfa55abb24d534f6a30590acf47d5`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 3; wall time 24 to 65 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 64.4 | 8 | 8 | [run](https://argusic.com/run/d86648d2-58e2-4c8d-bd09-3892730047b0) |
| 2 | pass with mocks | 92 | 18 | 65 | 4 | 4 | [run](https://argusic.com/run/b15bf66e-c7c0-4010-9f1a-06ae03dd0dc3) |
| 3 | pass with mocks | 92 | 10 | 24 | 5 | 5 | [run](https://argusic.com/run/d1876e72-6aaa-4c3e-8bfd-19d1ea9e9ed7) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pywin32, comtypes, dxcam have no Linux wheels; uv sync fails`
- 2 min: `uia/enums.py calls os.sys.getwindowsversion() and ctypes.windll at module level on Linux`
- 2 min: `uia/__init__.py unconditionally imports core/patterns/controls/events that need comtypes`
- 1 min: `uia/exceptions.py imports _ctypes.COMError (Windows-only)`
- 1 min: `desktop/utils.py imports pywintypes at module level`
- 1 min: `vdm/__init__.py unconditionally imports comtypes`
- 1 min: `powershell/service.py imports winreg unconditionally`
- 3 min: `21 test files import Windows-only modules at module level`

Attempt 2:

- 10 min: `pywin32 has no Linux wheel , cannot install via uv`
- 2 min: `fastmcp 4.x installed (project pins 3.4.7) , Context not found`
- `2 flash_overlay tests fail importing windows_mcp.uia which needs msvcrt`
- `~16 test files can't collect on Linux (need winreg/msvcrt for powershell/uia imports)`

Attempt 3:

- 3 min: `Windows-only dependencies (pywin32, comtypes, dxcam, mss, uiautomation) have no Linux wheels; stubs created in .venv site-packages`
- 1 min: `Python 3.14 required but system has 3.12; uv installs 3.14.7`
- 2 min: `uv sync fails on pywin32 (no Linux wheel)`
- 3 min: `src/ files have Windows-only API calls at module level (getwindowsversion, ctypes.windll, _ctypes.COMError, winreg)`
- `4 tests fail on Linux (platform-specific): test_cli_legacy_flags (schtasks.exe), test_iserror_compliance (COM), test_selfpipe_guard (socket/event loop)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
