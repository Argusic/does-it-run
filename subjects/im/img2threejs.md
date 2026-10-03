# img2threejs

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/img2threejs/img2threejs, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/img2threejs

## Pinned environment

- Project commit: `6e60b5e22419464b4853e01ddb6c0e6f6659a733`
- Test commit: `6e60b5e22419464b4853e01ddb6c0e6f6659a733`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 28.7 to 28.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0 | 28.7 | 1 | 1 | [run](https://argusic.com/run/10f2e903-8c77-41d2-be67-728c6a2f9744) |

## What was observed on a clean machine

Attempt 1:

- 5 min: `test_vertex_paint.TypeScriptParity.test_python_and_typescript_agree_on_every_sample_point failed because Node 18 does not support --experimental-strip-types (requires Node >=22)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
