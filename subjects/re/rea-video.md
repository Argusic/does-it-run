# rea-video

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/JuneYaooo/rea-video, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/rea-video

## Pinned environment

- Project commit: `c6cbc9185bae31ab479c2a80327160ae5fba3f32`
- Test commit: `c6cbc9185bae31ab479c2a80327160ae5fba3f32`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 9.3 to 25.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 22 | 9.3 | 0 | 0 | [run](https://argusic.com/run/6472638e-51fd-4fb7-a460-8318fac3f0b1) |
| 2 | pass | 100 | 5 | 25.4 | 3 | 3 | [run](https://argusic.com/run/b44d76c7-3ec5-4ce1-a72d-52d82bf94f27) |

## What was observed on a clean machine

Attempt 2:

- 3 min: `Externally managed Python environment blocked direct pip install`
- 2 min: `pytest not installed`
- 1 min: `jsonschema not installed, causing test_capabilities_valid failure`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
