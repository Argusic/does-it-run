# CLI-Anything

**Verdict: runs.** Argusic Score 94.7 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/HKUDS/CLI-Anything, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/cli-anything

## Pinned environment

- Project commit: `810c18b0d1ab9b234bc996c9fd999318523a3ef0`
- Test commit: `810c18b0d1ab9b234bc996c9fd999318523a3ef0`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 4; wall time 1.9 to 6.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 3.3 | 1 | 1 | [run](https://argusic.com/run/d09623dd-2cfb-4e15-80df-f0249619e0d8) |
| 1 | pass with mocks | 78.67 | 1 | 3.1 | 3 | 1 | [run](https://argusic.com/run/e5b09cec-1746-4f0d-84f2-fad0d698c747) |
| 2 | pass | 100 | 18 | 6.4 | 3 | 3 | [run](https://argusic.com/run/114498db-056a-453b-8e02-31d2ed2685c5) |
| 3 | pass | 100 | 0.1 | 1.9 | 0 | 0 | [run](https://argusic.com/run/4b1a83fd-5673-48d9-8d0a-37b59cc712f2) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip not available in base system environment`

Attempt 1:

- `GIMP is not installed (not available without root) , 4 E2E tests in gimp harness fail`
- `Blender is not installed (not available without root) , 13 E2E tests in blender harness fail`
- 0.5 min: `numpy not installed initially , required by gimp e2e tests`

Attempt 2:

- 2 min: `System Python externally managed (PEP 668) , pip install -e failed`
- 1 min: `Pillow not installed; test_full_e2e.py import error for gimp`
- 1 min: `numpy not installed; test_full_e2e.py import error for gimp`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
