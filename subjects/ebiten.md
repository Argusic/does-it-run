# ebiten

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/hajimehoshi/ebiten, licensed Apache-2.0, written in Go.

Evidence and recordings: https://argusic.com/subject/ebiten

## Pinned environment

- Project commit: `38f48794dd743407f49fdb906867bb69988f3505`
- Test commit: `38f48794dd743407f49fdb906867bb69988f3505`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.4 to 11.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 11.4 | 2 | 2 | [run](https://argusic.com/run/a308f074-5147-47f1-8741-4026c70ddd10) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Go binary not found in container (no go version)`
- 5 min: `TestPrograms/issue2737.go failed: panic due to no audio device (PulseAudio missing, ALSA no cards)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
