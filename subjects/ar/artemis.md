# artemis

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/google/artemis, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/artemis

## Pinned environment

- Project commit: `371aa6df56880643da57b30da936e9812fb0ec66`
- Test commit: `371aa6df56880643da57b30da936e9812fb0ec66`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 26.4 to 61 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 26.4 | 3 | 3 | [run](https://argusic.com/run/90a7909c-c473-4392-b3c0-a4bff4a1a833) |
| 2 | pass with mocks | 92 | 67 | 61 | 8 | 8 | [run](https://argusic.com/run/3e0f07ba-3f0b-4af7-9326-06e97ca990c3) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `adb_server_manifest fixture descriptions mismatch MCP v1.29.0 indentation`
- 3 min: `subprocess.CREATE_NEW_PROCESS_GROUP does not exist on Linux in device_utils test`
- 3 min: `video frame count assertion 43-47 fails; actual frames 77`

Attempt 2:

- 15 min: `VisualStepSummarizer.__init__ crashed without an API key: except-branch re-called get_google_llm() after the first call failed, and logger calls used printf-style args unsupported by ArtemisLogger`
- 6 min: `Unit tests using MagicMock providers hit 'Unknown LLM provider' exception`
- 10 min: `Generated FastMCP tool schemas for ADB server drifted from the pinned fixture: 6 docstrings were indented/missing blank lines and contained a literal backslash-n`
- 5 min: `subprocess.CREATE_NEW_PROCESS_GROUP/DETACHED_PROCESS are absent on Linux, breaking device utils import and one unit test`
- 4 min: `render_timeline_clip raised when callers passed a str output path instead of Path`
- 8 min: `test_unified_controller_video.py relied on hardcoded decoded frame counts/indices that vary by codec/OpenCV build (77 frames decoded for a clip ffmpeg reports as 34-45)`
- 4 min: `Showcase UI auto-rebuild fails: 'ng build' requires Node ^22.22.3 but container Node is v18.19.1; no root to upgrade`
- 15 min: `No real Google API key, Android device, or scrcpy in the container; adb daemon comes from the bundled adbutils binary`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
