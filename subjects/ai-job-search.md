# ai-job-search

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MadsLorentzen/ai-job-search, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/ai-job-search

## Pinned environment

- Project commit: `42ba4b475a8a2fb2d4aa333348850d8c5e1d5886`
- Test commit: `42ba4b475a8a2fb2d4aa333348850d8c5e1d5886`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 4; wall time 4.1 to 9.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 20 | 4.1 | 3 | 3 | [run](https://argusic.com/run/38a48ccf-0875-4eac-80a0-62461ec1689e) |
| 1 | pass | 100 | 4.5 | 5.4 | 5 | 5 | [run](https://argusic.com/run/f66eb912-6a5c-4343-a5b3-03162ea71fa7) |
| 2 | pass | 100 | 16 | 9.2 | 4 | 4 | [run](https://argusic.com/run/545f5b8e-f26d-4200-8766-9ddd751524e2) |
| 3 | pass | 100 | 20 | 8.3 | 4 | 4 | [run](https://argusic.com/run/ea1709f1-2bef-47f0-ac95-92e5e5261b5a) |

## What was observed on a clean machine

Attempt 1:

- `LaTeX (lualatex, xelatex) not installed in container`
- `PyYAML not available (pip not accessible in minimal Python environment)`

Attempt 1:

- 2 min: `bun was not installed`
- 2.5 min: `Missing bun dependencies in 4 of 6 skill CLIs (jobbank-search, jobindex-search, jobnet-search, jobdanmark-search)`
- `PyYAML not installed causing lint_skills.py to fail standalone and 1 test skipped`
- `robots_check.py needs a URL argument , fails with UNCONFIRMED when no URL provided`
- `LaTeX (lualatex/xelatex) not available for PDF compilation`

Attempt 2:

- 2 min: `Bun binary not on $PATH , test helpers call Bun.spawn(["bun",...]) and fail with ENOENT`
- 6 min: `LaTeX/lualatex/xelatex not installed , required for CV/cover-letter compilation`
- 1 min: `pip install pypdf blocked by externally-managed-environment`
- 1 min: `Bun install via shell script failed , unzip missing`

Attempt 3:

- 3 min: `Bun curl installer failed: unzip not installed`
- 1 min: `PyYAML not installed (6 tests skipped)`
- `LaTeX not available (lualatex/xelatex not found)`
- `salary_data.json not found`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
