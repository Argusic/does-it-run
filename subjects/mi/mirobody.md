# mirobody

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/thetahealth/mirobody, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/mirobody

## Pinned environment

- Project commit: `ff399ad427640d927007582f9c0a0f90dece2016`
- Test commit: `ff399ad427640d927007582f9c0a0f90dece2016`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 3.8 to 7.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 3.8 | 0 | 0 | [run](https://argusic.com/run/aab2a98f-0249-4ab1-a032-76b1c1d26b14) |
| 2 | pass | 100 | 6 | 7.6 | 1 | 1 | [run](https://argusic.com/run/56f20508-322a-4b7a-9bbf-5a98deb9a2cb) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `Git LFS not installed in container; 4 terminology data files (17 MB LOINC bundle, 1.2 MB en_parts, 1 MB zh_CN_parts, 790 KB CPIC genotypes) were LFS pointer stubs at checkout`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
