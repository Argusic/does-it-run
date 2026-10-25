# picollm

**Verdict: could not verify.** Argusic Score 55 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Picovoice/picollm, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/picollm

## Pinned environment

- Project commit: `b769979404cfc7ac3d1e5908b16fc6e2f2197d1f`
- Test commit: `b769979404cfc7ac3d1e5908b16fc6e2f2197d1f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 7.9 to 13.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 30 | 5 | 7.9 | 1 | 0 | [run](https://argusic.com/run/6d7722d4-545b-4ce8-bcd6-59631452731f) |
| 2 | fail | 80 | 8 | 13.6 | 1 | 1 | [run](https://argusic.com/run/9a6e0d02-d3e8-46fc-a403-788d222cb910) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `No valid .pvllm model files bundled in the repo; library fails pv_picollm_init with 'Failed to read from file' on any non-model input.`

Attempt 2:

- 1 min: `C demo build failed initially: missing stb_image.h submodule`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
