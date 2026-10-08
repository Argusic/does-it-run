# SoniTranslate

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/R3gm/SoniTranslate, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sonitranslate

## Pinned environment

- Project commit: `70b6390a413bd092c2a6249438f4d75bc5be7093`
- Test commit: `70b6390a413bd092c2a6249438f4d75bc5be7093`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 21.7 to 21.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 28 | 21.7 | 5 | 5 | [run](https://argusic.com/run/d42ef0d1-6c98-44de-93ac-b90e2553a097) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `huggingface_hub HfFolder import error (gradio 4.19.2 incompatible with huggingface_hub >=1.0)`
- 3 min: `pyworld failed to build from source (no python3-dev / Python.h)`
- 6 min: `Jinja2/starlette version conflict: TypeError: unhashable type: 'dict' in starlette templating`
- 2 min: `Missing modules: soundfile, librosa, pkg_resources`
- 1 min: `faiss-cpu==1.7.3 not available for Python 3.12`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
