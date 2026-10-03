# lingbot-map

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Robbyant/lingbot-map, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/lingbot-map

## Pinned environment

- Project commit: `849e690bb086103637e44b1e91878d9d43a8bf0c`
- Test commit: `849e690bb086103637e44b1e91878d9d43a8bf0c`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 8.9 to 20.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 80 | 3.2 | 8.9 | 1 | 1 | [run](https://argusic.com/run/e07d5045-4fe1-45f2-aecd-93221232843a) |
| 2 | fail | 20 | n/a | 20.2 | 0 | 0 | [run](https://argusic.com/run/6effdb81-9b38-443a-b9a1-bbd933791cf4) |

## What was observed on a clean machine

Attempt 1:

- 0.5 min: `min(scale_frames, S_true) in lingbot_map/aggregator/stream.py lines 340/353 raises RuntimeError when S_true/S_global is a tensor with >1 element`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
