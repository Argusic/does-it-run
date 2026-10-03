# dia

**Verdict: could not verify.** Argusic Score 50 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nari-labs/dia, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/dia

## Pinned environment

- Project commit: `876125e461a03b157ec905b0fe8b57a0f8b9e7a0`
- Test commit: `876125e461a03b157ec905b0fe8b57a0f8b9e7a0`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 9.5 to 52.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 50 | 4 | 52.7 | 2 | 2 | [run](https://argusic.com/run/dbdbc36e-4c9a-4f88-8d59-642a173ecd25) |
| 2 | fail | 50 | 3.2 | 9.5 | 2 | 2 | [run](https://argusic.com/run/389a963e-3a6b-4646-8c56-0bba5a2ab9b9) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Externally managed Python environment (PEP 668) prevents system-wide pip install`
- 3 min: `OOM kill (signal 9) during Dia.from_pretrained due to double allocation of 6.4GB float32 model exceeding 7.5GB cgroup limit`

Attempt 2:

- 0.5 min: `PEP 668 externally-managed-environment blocked system-wide pip install`
- 1.5 min: `OOM while loading Dia-1.6B-0626 model weights on 755MB RAM container`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
