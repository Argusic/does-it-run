# ArchiveBox

**Verdict: runs.** Argusic Score 91.3 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/ArchiveBox/ArchiveBox, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/archivebox

## Pinned environment

- Project commit: `c50d974be5ca28a1d4a1eabf45f09b0c0616f33d`
- Test commit: `c50d974be5ca28a1d4a1eabf45f09b0c0616f33d`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 12.4 to 23.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 86.67 | 1.5 | 23.1 | 3 | 1 | [run](https://argusic.com/run/ed26032b-150a-4119-9c6a-94495baa3c5a) |
| 2 | pass | 96 | 2.5 | 12.4 | 5 | 4 | [run](https://argusic.com/run/362fc392-c02d-47b7-8f8e-9de79495f506) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `python-ldap build failed (missing lber.h system header) when using --all-extras`
- 2 min: `chromium binary cannot be installed (apt and playwright both need root)`
- 1 min: `wget and unzip binaries cannot be installed via apt (no root)`

Attempt 2:

- 0.5 min: `uv not found in system PATH at start`
- 1 min: `uv sync --dev --all-extras failed: psycopg-binary has no wheel for cp315`
- 0.5 min: `uv sync --dev --all-extras failed: python-ldap build needs lber.h system header`
- 1 min: `archivebox init --install fails: cannot install chromium (playwright) or unzip (apt) without root`
- `archivebox add hangs: requires chromium or wget which are not present`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
