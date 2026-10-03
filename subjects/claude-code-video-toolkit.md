# claude-code-video-toolkit

**Verdict: runs.** Argusic Score 90 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/digitalsamba/claude-code-video-toolkit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/claude-code-video-toolkit

## Pinned environment

- Project commit: `f91608aa3750304195322387515e8284ca617f0b`
- Test commit: `f91608aa3750304195322387515e8284ca617f0b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 16.4 to 16.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 12 | 16.4 | 2 | 1 | [run](https://argusic.com/run/178e078f-6f40-4816-b2a5-05ab26c76655) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `scripts/migrate_to_codex.py: write_text function referenced but not defined in _migrate_common.py, causing NameError`
- `product-demo template render fails: missing public/audio/background-music.mp3 (expected , template needs user assets)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
