# biscuit

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tomlin7/biscuit, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/biscuit

## Pinned environment

- Project commit: `85c5beb0c624c1885d994c63bb1a24ce19599467`
- Test commit: `85c5beb0c624c1885d994c63bb1a24ce19599467`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 12.3 to 12.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 12 | 12.3 | 5 | 5 | [run](https://argusic.com/run/7cd3d2b6-9455-4b93-8c81-8eb466dd94c0) |

## What was observed on a clean machine

Attempt 1:

- 4 min: `Python 3.12 system build lacks _tkinter module (Tk not compiled in)`
- 2 min: `tkextrafont declared win32-only in pyproject.toml but imported unconditionally in src/biscuit/settings/settings.py; cannot install on Linux (requires scikit-build + C toolchain)`
- 0.5 min: `pytest-asyncio listed in dependency groups but not installed by pip install -e .[dev]`
- 1.5 min: `Tk event binding '<Control-\\>' is invalid keysym in headless Xvfb`
- 0.5 min: `biscuit-extensions subrepo cloned at runtime contains tests/e2e/conftest.py with wrong paths, breaking pytest collection`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
