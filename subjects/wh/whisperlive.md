# WhisperLive

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/collabora/WhisperLive, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/whisperlive

## Pinned environment

- Project commit: `99cbc1c33b35c372b4790975f819dfde62f3e74a`
- Test commit: `99cbc1c33b35c372b4790975f819dfde62f3e74a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 10.7 to 10.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 6 | 10.7 | 4 | 4 | [run](https://argusic.com/run/31a1c20b-8765-4012-a90e-41d1f3814369) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `PyAudio build failed: missing python3-dev and portaudio19-dev (no root access for apt)`
- 1 min: `Missing test dependency: jiwer module not installed`
- 1 min: `VAD model download failed: wget not available in container`
- 1 min: `test_vad_extended.py mocked subprocess.run instead of urllib.request.urlretrieve after the code change`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
