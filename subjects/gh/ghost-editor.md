# ghost-editor

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kurbaitaev/ghost-editor, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ghost-editor

## Pinned environment

- Project commit: `ce172726c36293722b08eb57b5b307d4f06389e8`
- Test commit: `ce172726c36293722b08eb57b5b307d4f06389e8`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 29.7 to 29.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 55 | 29.7 | 5 | 5 | [run](https://argusic.com/run/e095e266-570f-4526-973b-54e88ddcc56e) |

## What was observed on a clean machine

Attempt 1:

- 6 min: `ffmpeg/hyperframes need Node >= 22, system has Node 18.19.1; scripts/hf.sh --version failed with 'require Node.js >= 22'`
- 10 min: `system python3 is externally managed (PEP 668), pip install refused`
- 12 min: `python3 scripts/library_restore.py --sfx-only --music-only silently skipped both sections (flags are mutually exclusive in the script)`
- 14 min: `tests/test_cutout_fx.py assertion: last --release frame differs from source by 20.68 gray levels (test requires <1.5)`
- 8 min: `GEMINI_API_KEY required by doctor and QA scripts (real service)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
