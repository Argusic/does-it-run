# minimind

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jingyaogong/minimind, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/minimind

## Pinned environment

- Project commit: `f659b55761b754d306bd140573493a6543cafd7f`
- Test commit: `f659b55761b754d306bd140573493a6543cafd7f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12 to 12.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5 | 12 | 2 | 2 | [run](https://argusic.com/run/3671ba3f-914b-4447-99b9-6aab7c72bcf0) |
| 2 | pass | 100 | 12 | 12.6 | 4 | 4 | [run](https://argusic.com/run/e3c70a0c-8e5d-49fd-8dec-f5601dfdb214) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `System Python is externally managed (PEP 668); pip install to system Python fails`
- 2 min: `ujson==5.1.0 failed to build from source: missing Python.h (no python3-dev headers); no root to install system packages`

Attempt 2:

- 1 min: `pip install blocked by PEP 668 externally-managed-environment`
- 1 min: `ujson wheel build failed: missing Python.h development headers (unable to compile C extension)`
- 5 min: `Model weights (full_sft_768.pth, pretrain_768.pth) not found in ./out/`
- 3 min: `Training scripts crashed with huggingface_hub error 'Repo id must use alphanumeric chars' for path '../model' and PermissionError on '../checkpoints'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
