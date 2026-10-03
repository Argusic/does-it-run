# printfilm

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yi1108/printfilm, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/printfilm

## Pinned environment

- Project commit: `cdcd1f73d6671544b13716ca8d0c5ef1d76e11e7`
- Test commit: `cdcd1f73d6671544b13716ca8d0c5ef1d76e11e7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.9 to 13.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 13 | 13.9 | 3 | 3 | [run](https://argusic.com/run/ad997deb-ddba-4a7f-90f9-99772e2920f1) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `test_fragment_video_estimate: billing estimates assumed 2x ratio between 480p and 720p for seedance-2-5, but VENDOR_VIDEO_YUAN_5S_BY_RES has 3.36 vs 7.56 (2.25x)`
- 1 min: `test_kepu_phase_billing: same 2x ratio assumption in HD doubles 480p preview test`
- 1 min: `test_kepu_shot_edit_demote: narration edit demotion expected SCRIPT_READY but code correctly returns VIDEO_READY (videos still valid, only audio needs refresh)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
