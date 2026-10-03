# osmnx

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/gboeing/osmnx, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/osmnx

## Pinned environment

- Project commit: `74e68ce2200b23c04f6ec2a864a6c24859bbf08d`
- Test commit: `74e68ce2200b23c04f6ec2a864a6c24859bbf08d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 75 to 75 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.25 | 75 | 3 | 3 | [run](https://argusic.com/run/1ba6b80a-f80a-457c-b898-452790a55bf2) |

## What was observed on a clean machine

Attempt 1:

- 25 min: `Overpass API (overpass-api.de) unreachable from this container - all Overpass-dependent tests would hang waiting for connection`
- 8 min: `test_elevation: 'numpy.ndarray.squeeze()' on single-element raster sample reduces to a 0-d array, causing 'TypeError: iteration over a 0-d array' in '_query_raster' multiprocessing path`
- 15 min: `Mock-generated street grid data lacks 'maxspeed', 'lanes', 'highway' type diversity required by test_routing and the consolidate step in test_elevation`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
