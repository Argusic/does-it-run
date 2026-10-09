# whisper-ctranslate2

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Softcatala/whisper-ctranslate2, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/whisper-ctranslate2

## Pinned environment

- Project commit: `7c06913255bea6f630b6d1357e99dc0c3bfa1819`
- Test commit: `7c06913255bea6f630b6d1357e99dc0c3bfa1819`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 22.5 to 22.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 93.33 | 6 | 22.5 | 3 | 2 | [run](https://argusic.com/run/fa827a7f-169c-434e-a833-65414d0c8c7f) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System pip install blocked by PEP 668 externally-managed environment`
- 3 min: `av 19.0.1 removed the metadata_errors kwarg, breaking faster-whisper 1.2.1 audio decode (TypeError open() got unexpected keyword argument 'metadata_errors')`
- 1 min: `e2e test_transcribe_diarization failed: HF_TOKEN unset and pyannote.audio/torch not installed for gated pyannote/speaker-diarization-community-1 model`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
