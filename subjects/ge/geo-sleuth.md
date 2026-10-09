# geo-sleuth

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Oldcircle/geo-sleuth, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/geo-sleuth

## Pinned environment

- Project commit: `e753bb3aad19b7ffd0d31ec52f921867df73eced`
- Test commit: `e753bb3aad19b7ffd0d31ec52f921867df73eced`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.2 to 23.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 95 | 6 | 23.2 | 4 | 3 | [run](https://argusic.com/run/62036df1-4337-4fa0-9350-6bd7bd8673c4) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not installed; scripts require uv run`
- 3 min: `sun.py compass crashed on single-value --hfov 65 (ValueError: not enough values to unpack)`
- 2 min: `sat_scan.py grid crashed on a 0-cell bbox (ValueError: need at least one array to concatenate)`
- 3 min: `gazetteer.py info/children and osm.py need OSM Overpass, unreachable from this container's egress (Apache error page retried 3x)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
