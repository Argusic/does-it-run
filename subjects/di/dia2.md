# dia2

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nari-labs/dia2, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/dia2

## Pinned environment

- Project commit: `8687268f4ed3ed20704638fd353b51491de3b476`
- Test commit: `8687268f4ed3ed20704638fd353b51491de3b476`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 11.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.6 | 11.7 | 3 | 3 | [run](https://argusic.com/run/441c0001-7627-49c1-870b-5c57c4c1c7aa) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `uv not found in PATH (installed via pip, but only accessible from /home/runner/.local/bin)`
- 3 min: `2B model (Dia2-2B, 7.68 GB safetensors) caused OOM kill under 8 GB cgroup memory limit on CPU`
- 2 min: `resolve_precision defaults to float32 on CPU regardless of dtype preference, exceeding 8 GB cgroup limit with 1B model (~4.3 GB weights + float32 model)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
