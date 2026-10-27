# ID-V2V

**Verdict: runs with mocks.** Argusic Score 71 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Eyeline-Labs/ID-V2V, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/id-v2v

## Pinned environment

- Project commit: `b9df1e501b2561c445923cbed13b5ff8770c0e7a`
- Test commit: `b9df1e501b2561c445923cbed13b5ff8770c0e7a`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 8.6 to 9.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 2.8 | 8.6 | 1 | 1 | [run](https://argusic.com/run/4a528cd6-4c48-433e-b2df-3acd2615f4c5) |
| 2 | pass with mocks | 92 | 55 | 9.8 | 4 | 4 | [run](https://argusic.com/run/bfd9b7eb-18d7-4661-ab2f-a0be5910a4e8) |

## What was observed on a clean machine

Attempt 1:

- 0.3 min: `david_runtime/__init__.py __all__ listed ONNX_EP and ModelNotFoundError without importing them; ModelError referenced but does not exist in codebase`

Attempt 2:

- 8 min: `uv was not installed in the container`
- 14 min: `pack_per_frame_instances crashed on SAM3 tracker outputs lacking scores/boxes or with per-object (H,W) masks (KeyError/shape errors)`
- 9 min: `save_sam3_per_frame_folders left empty frame folders without sam3Mask_id_all.png, which would break downstream orig_pixel`
- 2 min: `uv sync regenerated uv.lock (revision 3 to 5, cosmetic URL changes)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
