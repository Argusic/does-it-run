# mousiki

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/itzender5820/mousiki, licensed Apache-2.0, written in C++.

Evidence and recordings: https://argusic.com/subject/mousiki

## Pinned environment

- Project commit: `3a08e896c99dbeb5716a339ce69e39d2692ee6cc`
- Test commit: `3a08e896c99dbeb5716a339ce69e39d2692ee6cc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.9 to 5.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2.5 | 5.9 | 4 | 4 | [run](https://argusic.com/run/ee2ea0db-2ddd-4f83-94fb-8b793f30c169) |
| 2 | pass | 100 | 2 | 3.9 | 0 | 0 | [run](https://argusic.com/run/745660bf-b2c7-46ee-8ad5-03266288b1a2) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `yt-dlp not installed in base container`
- 0.3 min: `Python requests package missing for lyrics fetcher`
- 0.5 min: `ALSA and PulseAudio development headers not installed (no root for apt install)`
- 0.1 min: `PEP 668 blocks pip install --user in system Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
