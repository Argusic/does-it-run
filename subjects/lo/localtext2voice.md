# LocalText2Voice

**Verdict: runs.** Argusic Score 58 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/estebanstifli/LocalText2Voice, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/localtext2voice

## Pinned environment

- Project commit: `83a186f54dac5a607a957de83de39277c7ba061b`
- Test commit: `83a186f54dac5a607a957de83de39277c7ba061b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 17.1 to 31.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 17.1 | 0 | 0 | [run](https://argusic.com/run/21c85106-c041-40d6-b008-cc2b9f999508) |
| 2 | pass | 96 | 5 | 31.2 | 5 | 4 | [run](https://argusic.com/run/8ccb4cdb-8852-4520-97d7-6088cd9c4d23) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `tests/test_mcp_stdio_bridge.py referenced .venv/Scripts/python.exe (Windows path) which does not exist on Linux`
- 5 min: `app/core/storyboard_credentials.py used Windows-only DPAPI which crashed Linux tests requiring credential storage`
- 3 min: `tests/test_video_storyboard_renderer.py hardcoded Windows ffmpeg/ffmpeg.exe path that doesn't exist on Linux`
- 2 min: `tests/test_video_storyboard_settings_ui.py removeprefix("file:///") incorrectly stripped the path separator leaving a non-existent relative path`
- 10 min: `Qt Multimedia QMediaPlayer/QAudioOutput segfault on startup because libpipewire is installed but no PipeWire daemon runs in the container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
