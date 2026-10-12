# themes

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/warpdotdev/themes, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/themes

## Pinned environment

- Project commit: `4154072de03bea5dd070afa947ba6a6f2310ed5d`
- Test commit: `4154072de03bea5dd070afa947ba6a6f2310ed5d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 2.4 to 2.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 3 | 2.4 | 1 | 1 | [run](https://argusic.com/run/a9fd5056-746d-459c-8ee9-40f2660be832) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `gen_theme_previews.py line 171 passed output_dir instead of input_dir to get_color_dict(), causing FileNotFoundError`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
