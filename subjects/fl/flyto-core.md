# flyto-core

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/flytohub/flyto-core, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/flyto-core

## Pinned environment

- Project commit: `f1d9c5ccfc232d87d649ce08e0d5292b84cbf9c7`
- Test commit: `f1d9c5ccfc232d87d649ce08e0d5292b84cbf9c7`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 54.2 to 54.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 12 | 54.2 | 3 | 3 | [run](https://argusic.com/run/bfa2bf3e-b098-4f8e-ba68-dcfcd27c554e) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `test_artifact_mutation_through_open_descriptor_is_detected failed , same-length write did not change fstat size`
- 2 min: `jsdom@29.1.1 requires Node >=20, container has Node 18.19`
- `ping binary not found in container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
