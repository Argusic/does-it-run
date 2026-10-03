# taskiq

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/taskiq-python/taskiq, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/taskiq

## Pinned environment

- Project commit: `a00e4b0030f5ada13068da8644048867967aeda4`
- Test commit: `a00e4b0030f5ada13068da8644048867967aeda4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 3.4 to 3.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.4 | 3 | 3 | [run](https://argusic.com/run/f554c08d-053a-4ae2-91b7-d42a84729617) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `externally-managed-environment blocked system-wide pip`
- 0.5 min: `versioningit could not find a git tag for version resolution`
- 0.5 min: `opentelemetry, msgpack, cbor2, orjson, psutil, tzdata packages missing for tests`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
