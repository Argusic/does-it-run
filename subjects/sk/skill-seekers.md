# Skill_Seekers

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/yusufkaraaslan/Skill_Seekers, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/skill-seekers

## Pinned environment

- Project commit: `f3972efa33fa79634b96936acf1fac321cdcf7c1`
- Test commit: `f3972efa33fa79634b96936acf1fac321cdcf7c1`
- Worker image digests: `sha256:4c3d41857be3a23db294bd830ae20afa2e3aa328c9b1acf1b30add6628aa2c66`, `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 5.7 to 11.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 15 | 11.7 | 1 | 1 | [run](https://argusic.com/run/aae6fe3b-3715-40a6-934e-b1ffaa2768af) |
| 2 | pass | 100 | 6 | 10.5 | 2 | 2 | [run](https://argusic.com/run/69645c54-68fd-4fc0-8d98-664fbc507038) |
| 3 | pass | 100 | 8 | 5.7 | 2 | 2 | [run](https://argusic.com/run/ff1e5163-5f66-470c-a4e9-326e158392cb) |

## What was observed on a clean machine

Attempt 1:

- `test_video_setup.py::TestVenv::test_create_venv_in_tempdir fails because python3.12-venv (ensurepip) is not installed in the container`

Attempt 2:

- 1 min: `Externally managed Python environment prevented system-wide install`
- 1 min: `CLI entry point 'skill-seekers' not on PATH, causing test subprocess failures (15 tests)`

Attempt 3:

- 1 min: `Externally managed Python , needed virtual environment`
- 2 min: `Pytest not resolved via dependency-groups on first install pass`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
