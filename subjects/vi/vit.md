# vit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/LucasHJin/vit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/vit

## Pinned environment

- Project commit: `472b94039b5c314bda67136432ea70be5f516215`
- Test commit: `472b94039b5c314bda67136432ea70be5f516215`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 1.5 to 3.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 11 | 1.5 | 3 | 3 | [run](https://argusic.com/run/61bef28b-79a8-45cd-891a-b470fde2dd78) |
| 2 | pass | 100 | 1.5 | 3.1 | 3 | 3 | [run](https://argusic.com/run/461970e6-0ccf-409a-91a7-41f97af1ef79) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `Externally-managed Python environment blocked system-wide pip install`
- 1 min: `git commit failed with 'Author identity unknown' in test fixture`
- 1 min: `git init default branch is 'master' but tests reference 'main'`

Attempt 2:

- 0.2 min: `pip install failed: externally-managed-environment`
- 0.1 min: `git commit failed: Author identity unknown`
- 0.1 min: `git checkout main failed: pathspec 'main' did not match`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
