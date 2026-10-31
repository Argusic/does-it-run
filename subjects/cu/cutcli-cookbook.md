# cutcli-cookbook

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/xuliang2024/cutcli-cookbook, licensed MIT, written in JavaScript.

Evidence and recordings: https://argusic.com/subject/cutcli-cookbook

## Pinned environment

- Project commit: `d95632886cd34d01a77aef7199ed68536aa0640c`
- Test commit: `d95632886cd34d01a77aef7199ed68536aa0640c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 1.7 to 1.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 1.7 | 3 | 3 | [run](https://argusic.com/run/f5ce0f44-948d-4e43-affc-0c1d91221959) |

## What was observed on a clean machine

Attempt 1:

- `example 02-image-slideshow-bgm: CDN image asset https://cutcli.com/assets/demo/scene-01.jpg returns HTTP 404`
- `example 04-easy-by-audio: CDN audio asset https://cutcli.com/assets/demo/bgm-light.mp3 returns HTTP 404`
- `example 05-keyframe-zoom-in: CDN image asset https://cutcli.com/assets/demo/scene-02.jpg returns HTTP 404`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
