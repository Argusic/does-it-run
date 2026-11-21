# acl

**Verdict: runs.** Argusic Score 95 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/nfrechette/acl, licensed MIT, written in C++.

Evidence and recordings: https://argusic.com/subject/acl

## Pinned environment

- Project commit: `3ee568542eca4428e1041908b4a644b98e7885bd`
- Test commit: `3ee568542eca4428e1041908b4a644b98e7885bd`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 8.2 to 9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 2 | 9 | 2 | 1 | [run](https://argusic.com/run/5d5a6c5b-4a2c-480c-9e88-8a7cb388f8e7) |
| 2 | pass | 100 | 5 | 8.2 | 1 | 1 | [run](https://argusic.com/run/33a92ee6-4462-49b7-a11b-19786b828553) |

## What was observed on a clean machine

Attempt 1:

- `make.py:941 SyntaxWarning: invalid escape sequence '\.'`
- `decomp_data_v8.zip missing , decompression benchmark data not available`

Attempt 2:

- `Decompression test data (decomp_data_v8.zip) not found and no download URL configured; non-blocking`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
