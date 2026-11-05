# speech_recognition

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Uberi/speech_recognition, licensed BSD-3-Clause, written in Python.

Evidence and recordings: https://argusic.com/subject/speech-recognition

## Pinned environment

- Project commit: `8075e8f76acdac58fcf6ac41a104172f51349e98`
- Test commit: `8075e8f76acdac58fcf6ac41a104172f51349e98`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 4.3 to 6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 4.3 | 0 | 0 | [run](https://argusic.com/run/d7f3fb02-0509-48a9-adf8-4856b345e261) |
| 2 | pass with mocks | 92 | 75 | 6 | 4 | 4 | [run](https://argusic.com/run/244bafe8-a254-4ff7-a5ec-75e112fe4a1d) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `PEP 668 externally-managed-environment blocked system pip install`
- 10 min: `sprc CLI crashed: No module named 'tqdm' (undeclared dependency)`
- 8 min: `whisper-local tests failed collection: No module named 'whisper'/'faster_whisper' (importorskip without reason)`
- 10 min: `sprc download vosk crashed with FileNotFoundError on unexpected archive layout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
