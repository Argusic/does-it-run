# tox

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/tox-dev/tox, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/tox

## Pinned environment

- Project commit: `f46060e29701fc5595eaece61ffbf405787c7d59`
- Test commit: `f46060e29701fc5595eaece61ffbf405787c7d59`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 39 to 39 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.2 | 39 | 6 | 6 | [run](https://argusic.com/run/be513147-5775-4cde-a824-03fdc39d83ed) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `test_config_requires: dev version 0.1.dev1 doesn't satisfy tox>=4, provisioning fails against fake pip index`
- 2 min: `doc test from docs/how-to/usage.rst:2007: requires=["tox>=4.20"] triggers provisioning against fake pip index`
- 1 min: `doc test from docs/reference/config.rst:342: INI requires = tox >= 4.20 triggers provisioning`
- 1 min: `test_manpage_renders_sections, test_manpage_name_not_empty, test_manpage_header_shows_tox: man command is a stub in container printing 'minimized' instead of rendering`
- 1 min: `test_schema_tombi_lint: shutil.which('tombi') returns None because .venv/bin not on PATH`
- 1 min: `test_provision_acquires_file_lock: tox<4.14 doesn't trigger provisioning for dev version 0.1.dev1`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
