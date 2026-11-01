# opensource-clipping

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NaufalRizqullah/opensource-clipping, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/opensource-clipping

## Pinned environment

- Project commit: `4a478dff3dacd293eeb5e28335aa7c81d78b8f50`
- Test commit: `4a478dff3dacd293eeb5e28335aa7c81d78b8f50`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 21 to 21 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 5 | 21 | 3 | 3 | [run](https://argusic.com/run/3d1988c6-5969-4209-9c92-f5977fc4fdb6) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `torchaudio 2.11.1 from NVIDIA index missing AudioMetaData and info() , caused pyannote.audio import failure`
- 1 min: `AV library av-19.x has incompatible API 'metadata_errors' keyword arg for faster-whisper`
- `Whisper fails to download model via background thread after interpreter shutdown when using TestClient (API jobs); works fine standalone`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
