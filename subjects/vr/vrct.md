# VRCT

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/misyaguziya/VRCT, licensed NOASSERTION, written in Python.

Evidence and recordings: https://argusic.com/subject/vrct

## Pinned environment

- Project commit: `429a593fca423b3cc30c7d22514f52f2ebc23685`
- Test commit: `429a593fca423b3cc30c7d22514f52f2ebc23685`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 23.2 to 24.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 23.2 | 0 | 0 | [run](https://argusic.com/run/b306d51b-22d4-49a6-b696-f6a11367ff8d) |
| 2 | pass | 100 | 48 | 24.8 | 6 | 6 | [run](https://argusic.com/run/513b3658-fdbf-4ddd-81eb-766d46c75ce0) |

## What was observed on a clean machine

Attempt 2:

- 8 min: `pyaudiowpatch==0.2.12.6 has no Linux wheel (Windows-only WASAPI PortAudio bindings)`
- 2 min: `src-ui/import uses lowercase vrct.svg but the file is uppercase VRCT.svg (Windows case-insensitive vs Linux case-sensitive FS)`
- 3 min: `models/clipboard/clipboard.py unconditionally tries ctypes.WinDLL for user32/kernel32 on all platforms`
- 3 min: `tools/chatbox_sample_player.py raises RuntimeError('Interactive playback requires Windows') unconditionally on non-Windows, even for --dry-run and --start which never call msvcrt`
- 1 min: `test_clipboard_focus_and_paste.py::test_copies_and_pastes_when_focus_succeeds expects focus/paste path that is gated on sys.platform == 'win32' and never runs on Linux`
- 5 min: `Tauri requires webkit2gtk-4.1, javascriptcoregtk-4.1, and libsoup-3.0 development libraries to build (missing system-wide)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
