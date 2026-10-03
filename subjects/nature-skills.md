# nature-skills

**Verdict: runs.** Argusic Score 97.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Yuan1z0825/nature-skills, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/nature-skills

## Pinned environment

- Project commit: `bd4e415c1dcaf6df4ca701f8f8492a97e4b49921`
- Test commit: `bd4e415c1dcaf6df4ca701f8f8492a97e4b49921`
- Worker image digests: `sha256:33ceb71981b602c1a7443a53469e4dba065f7503eab3078a2d7a57a2ab987517`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services, real run
- Valid runs: 3; wall time 9.7 to 22 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 3 | 22 | 5 | 5 | [run](https://argusic.com/run/7477d157-4cb1-420c-a45e-a109a75ff727) |
| 2 | pass | 100 | 8 | 9.7 | 3 | 3 | [run](https://argusic.com/run/f93fdf14-296e-4b37-b66e-e7c698088632) |
| 3 | pass | 100 | 2.3 | 13 | 3 | 3 | [run](https://argusic.com/run/e2388c2d-10fc-4b30-a495-182c00003723) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `npx skills CLI requires Node >= 22.20.0 (only Node 18.19.1 available)`
- 2 min: `PyYAML not available for validate-skill-metadata.py and validate-workflows.py`
- 1 min: `pip not available in base Python (no ensurepip, externally-managed environment)`
- 5 min: `nature-image2ppt: 11/165 tests fail , require LibreOffice/soffice for PDF rendering (not available in container)`

Attempt 2:

- 2 min: `npx skills CLI requires Node.js >=22.20.0, but system has v18.19.1 (no nvm/fnm available to upgrade)`
- 1 min: `PyYAML not available in system Python; several validation scripts depend on it`

Attempt 3:

- 1.2 min: `npx skills requires Node >=22 but 18.19.1 is installed`
- 0.8 min: `rsync binary not found (no root to apt install)`
- 0.3 min: `PyYAML and pytest not in system Python`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
