# addok

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/addok/addok, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/addok

## Pinned environment

- Project commit: `d928b9e4f6ec83ee907e19788d2f48fa42d407da`
- Test commit: `d928b9e4f6ec83ee907e19788d2f48fa42d407da`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 13.4 to 13.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 42 | 13.4 | 4 | 4 | [run](https://argusic.com/run/3ce89028-aef1-4fd5-840a-9a0c5bfebb20) |

## What was observed on a clean machine

Attempt 1:

- 10 min: `pip install -e ".[dev]" failed: python-geohash 0.8.5 has no prebuilt wheel and its C extension needs Python.h; the container has no /usr/include/python3.12 headers and no python3-dev (no root to apt install)`
- 20 min: `First 'addok serve' attempt answered /health 200 but died after ~1 minute with no traceback; investigation showed the process was replaced by an exec-session parent and left running on port 7878, causing later duplicate-launch "Address alre`
- 5 min: `Housenumber search: query '221b' or '221' returns no results unless the query also contains the street name, and with '221b baker street' the label is the street label, not '221B Baker Street'`
- `Linux username is 'runner' but the README documents a /etc/addok/addok.conf path; the CLI lacks permission to write there`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
