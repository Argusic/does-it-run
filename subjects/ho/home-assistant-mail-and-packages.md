# Home-Assistant-Mail-And-Packages

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/moralmunky/Home-Assistant-Mail-And-Packages, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/home-assistant-mail-and-packages

## Pinned environment

- Project commit: `f2a8ecfedb5627a8e7a1871ce7948e50c77e1142`
- Test commit: `f2a8ecfedb5627a8e7a1871ce7948e50c77e1142`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 56.1 to 56.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 15 | 56.1 | 6 | 6 | [run](https://argusic.com/run/ea2fd88f-e398-4e68-b608-560700f133e3) |

## What was observed on a clean machine

Attempt 1:

- 8 min: `pip install -r requirements_test.txt failed building numpy on Python 3.12 (old setuptools/pyproject.toml incompatibility)`
- 3 min: `config_entry.version = 4 in async_migrate_entry fails on HA 2025.1.4 (version is now a frozen attr)`
- 1 min: `config_entry.options = config_entry.data fails (options is a frozen attr)`
- 5 min: `mock_listdir fixture patched os.listdir globally, breaking HA loader's pathlib.Path.iterdir() which uses os.listdir internally, causing 'Integration not found'`
- 1 min: `.called_with() is not a valid mock assertion in Python 3.12+`
- 0.5 min: `entry.version = 2 fails (version is a frozen attr)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
