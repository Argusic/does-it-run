# MacNativeGames

**Verdict: runs with mocks.** Argusic Score 86 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ly05010419/MacNativeGames, licensed MIT, written in C.

Evidence and recordings: https://argusic.com/subject/macnativegames

## Pinned environment

- Project commit: `30a1b93d0776150fbaffd7c20f9a5ca0841c21c9`
- Test commit: `30a1b93d0776150fbaffd7c20f9a5ca0841c21c9`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, run with mocked services
- Valid runs: 2; wall time 15 to 31.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 29 | 31.2 | 8 | 8 | [run](https://argusic.com/run/571c1b4d-c4b4-422a-820a-a87492ff340b) |
| 2 | pass with mocks | 92 | 6.8 | 15 | 8 | 8 | [run](https://argusic.com/run/17f73a48-b963-4b48-9a40-04e17db753dd) |

## What was observed on a clean machine

Attempt 1:

- `clonefile() syscall not available on Linux (APFS/macOS only)`
- `st_birthtime not available in os.stat on Linux`
- `xcrun command not found (Xcode tools not on Linux)`
- 1 min: `Missing cryptography module`
- 3 min: `Missing compression.zstd (Python 3.14 stdlib)`
- 2 min: `.venv/bin/python fails on Linux (sys.prefix has python3 not python)`
- 2 min: `codesign command not found (macOS code signing)`
- 1 min: `MergeWithBuildPatch tests ran with stub zstd and failed`

Attempt 2:

- 1.2 min: `build_app.clonefile() failed on Linux because clonefile(2) is macOS-only (undefined symbol: clonefile in libc)`
- 0.5 min: `test_app_game_data.py used os.stat_result.st_birthtime which does not exist on Linux`
- 0.3 min: `test_data_bundle.py used subprocess.run(['xcrun', '--find', 'clang']) at module level as skipUnless check, crashing when xcrun not found`
- 0.3 min: `test_mod_manifest.py used importlib.util.find_spec('compression.zstd') which raises ModuleNotFoundError on Python < 3.14`
- 1.5 min: `test_updates.py symlinked .venv to sys.prefix (/usr) but /usr/bin is read-only; also called step_app without patching data_bundle which runs codesign`
- 0.8 min: `test_build_mod.py's mergeable_overlays() failed because make_romfs_patches imports compression.zstd at module level`
- 0.5 min: `test_botw_import.py called step_app which invoked data_bundle and then codesign (macOS-only)`
- 0.5 min: `games/botw/scripts/location_markers.py imported sarc_members from make_romfs_patches at module level, which fails without compression.zstd`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
