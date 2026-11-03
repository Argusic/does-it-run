# khazix-skills

**Verdict: runs.** Argusic Score 97.5 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KKKKhazix/khazix-skills, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/khazix-skills

## Pinned environment

- Project commit: `4f2db09802736ac8130ddf8dd6121435b5a41b55`
- Test commit: `4f2db09802736ac8130ddf8dd6121435b5a41b55`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 4.5 to 5.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 5.2 | 5.4 | 0 | 0 | [run](https://argusic.com/run/8ca9e7cf-7383-48a4-b0fe-08166b6b6e32) |
| 2 | pass | 95 | 5 | 4.5 | 4 | 3 | [run](https://argusic.com/run/dc85643f-db18-4522-b14f-68e86363df07) |

## What was observed on a clean machine

Attempt 2:

- 1 min: `AIHOT installer failed with 'runtime package must contain exactly 6 files' because the live v2.0.0 package now contains 3 files.`
- 1 min: `hv-analysis dependencies were missing: ModuleNotFoundError for markdown and weasyprint.`
- 2 min: `Generated PDF had garbled Chinese text because no CJK font was installed and WeasyPrint substituted DejaVu Sans.`
- 1 min: `storage-analyzer/scan.py returned unsupported_platform for linux.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
