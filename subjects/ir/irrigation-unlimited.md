# irrigation_unlimited

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/rgc99/irrigation_unlimited, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/irrigation-unlimited

## Pinned environment

- Project commit: `05a5eaa7a7d8ad43bf3f903ce19490ac7f34ce8e`
- Test commit: `05a5eaa7a7d8ad43bf3f903ce19490ac7f34ce8e`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 81.9 to 81.9 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 4 | 81.9 | 4 | 4 | [run](https://argusic.com/run/b973557f-a880-47b2-bd0b-088aafb5cef6) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `pinned pytest-homeassistant-custom-component==0.13.329 requires Python>=3.14; only Python 3.12 present, so pip install failed`
- 7 min: `transient failure of tests/test_reload.py::test_service_reload_extend_shrink on the first full-suite run (event drift after config reload); no code changes present, isolated reruns and three subsequent full-suite runs all passed green`
- 1 min: `black --check (repo's CI style gate) flagged 5 integration files as needing reformatting`
- 2 min: `Home Assistant boot emits non-fatal turbojpeg camera error (native lib missing, no root); earlier config-dir discards during HA boot testing were bootstrap artifacts, not code errors`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
