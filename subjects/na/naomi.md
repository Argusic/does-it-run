# Naomi

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/NaomiProject/Naomi, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/naomi

## Pinned environment

- Project commit: `5a5f3ce845aab08d027703e13007c182fd5d13f6`
- Test commit: `5a5f3ce845aab08d027703e13007c182fd5d13f6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 31.9 to 31.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 32 | 31.9 | 7 | 7 | [run](https://argusic.com/run/53847580-ff43-4e38-99d7-a69f84b6f91c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pip blocked by PEP 668 externally-managed-environment`
- 15 min: `UnicodeDecodeError 'ascii' codec can't decode byte 0xc3 when gettext parses de-DE.mo/fr-FR.mo (catalogs lacked charset header because fuzzy .po entries dropped the header)`
- 2 min: `ModuleNotFoundError: no module named 'mad' and 'jiwer' (install batch aborted earlier)`
- 3 min: `ModuleNotFoundError: no module named 'naomi.main' from Naomi console script`
- 5 min: `pyaudio/pyalsaaudio/pocketsphinx/webrtcvad could not build: no python3-dev headers or system libs, no root to apt install`
- 2 min: `AttributeError: 'Mic' object has no attribute 'say_sync' on launch in --local mode`
- 3 min: `interactive populate/settings wizard blocks non-interactive launch`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
