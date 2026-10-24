# Whisper-TikTok

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MatteoFasulo/Whisper-TikTok, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/whisper-tiktok

## Pinned environment

- Project commit: `5a0cdeef5262238bd90430ddd4a30eaaec73d4d3`
- Test commit: `5a0cdeef5262238bd90430ddd4a30eaaec73d4d3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 7 to 7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5.9 | 7 | 3 | 3 | [run](https://argusic.com/run/58ebf6f3-2c64-4be5-bdf9-5b5b503f2231) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `subprocess.Popen in command_executor.py passed command string without shell=True, treating entire string as executable name`
- 0.5 min: `yt-dlp -o '%(id)s.%(ext)s' format string unquoted in video_downloader.py; shell interpreted %(id)s as subshell syntax`
- 0.7 min: `Edge TTS streaming API returned 403 (WSS handshake rejected) from container, blocking TTS synthesis step`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
