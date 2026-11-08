# stickman-video-director

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/kaomei/stickman-video-director, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/stickman-video-director

## Pinned environment

- Project commit: `8ced4737b8d2aa7e8e371a493e6b6add9885c0da`
- Test commit: `8ced4737b8d2aa7e8e371a493e6b6add9885c0da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 2; wall time 3.2 to 6.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 6.5 | 3 | 3 | [run](https://argusic.com/run/e488ad6e-f00f-4477-8392-7d606e489301) |
| 2 | pass | 100 | 0.5 | 3.2 | 2 | 2 | [run](https://argusic.com/run/64adf567-3cc7-4966-8187-53bd31f1fa68) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Doctor check required node >=20, got 18.19.1`
- 5 min: `Pillow missing and macOS hardcoded font paths in a6_finish.py`
- 3 min: `verify-voice-continuity.py git show origin/main failed (shallow clone)`

Attempt 2:

- 0.5 min: `System Node.js is v18.19.1 but project requires >=20; native canvas binaries installed correctly regardless`
- 0.1 min: `verify-voice-continuity.py referenced origin/main which doesn't exist in detached FETCH_HEAD checkout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
