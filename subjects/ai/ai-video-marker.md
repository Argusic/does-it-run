# ai-video-marker

**Verdict: runs.** Argusic Score 93.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lanqiao-Luca/ai-video-marker, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-video-marker

## Pinned environment

- Project commit: `c1dc8a21e2033605fda3cccde81777b3a64ad88a`
- Test commit: `c1dc8a21e2033605fda3cccde81777b3a64ad88a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 2.3 to 4.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 4.6 | 2 | 2 | [run](https://argusic.com/run/2dc2458c-9a0e-42bc-8b47-7b48efcdc67a) |
| 2 | pass | 86.67 | 6.4 | 2.3 | 3 | 1 | [run](https://argusic.com/run/92cf1bc6-d92a-48ab-a42d-cda4ba32c665) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `Harbor asset PNG file SHAs differ due to Pillow 11.3 compression change (pixel data identical)`
- 3 min: `Pixel baseline AST fingerprint mismatch from Python 3.12 ast.dump() differences (all 1056 frames still identical)`

Attempt 2:

- 0.1 min: `Pillow 11.3.0 cannot be installed system-wide (externally managed env); worked around by creating a venv`
- 10 min: `test_asset_kit_can_be_regenerated_and_reused_without_overwrite fails: regenerated harbor asset SHA256 values differ from shipped manifest.json in all 12 PNGs`
- 10 min: `test_all_original_frames_and_drawing_functions_are_preserved fails: pixel_drawing.py AST fingerprint does not match source-frame-baseline.json`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
