# PharosRAG

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Laurent00TT/PharosRAG, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/pharosrag

## Pinned environment

- Project commit: `162c7ca3e975440d0f345d0faca9194b4705d774`
- Test commit: `162c7ca3e975440d0f345d0faca9194b4705d774`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 5.9 to 22.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2 | 5.9 | 2 | 2 | [run](https://argusic.com/run/f3385102-2ef8-44f4-a7e6-b0be4559e91b) |
| 2 | pass with mocks | 92 | 0.2 | 22.2 | 3 | 3 | [run](https://argusic.com/run/9c38c110-b7d8-4578-942d-c598db3d5531) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `pip not installed in container (no python3-pip, no ensurepip)`
- 0.5 min: `Cannot start pharos serve with local GPU model (no GPU, no model files in container)`

Attempt 2:

- 0.2 min: `externally-managed-environment prevents system-wide pip install`
- 3 min: `pharos serve requires GPU model scripts at ~/models/Qwen3-VL-Embedding-8B/scripts which don't exist (no GPU in container)`
- 2 min: `remote module _verify_server checks that os.path.basename(dense_model_path) matches the server's model_dense field, so default path basename ~/models/... must match`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
