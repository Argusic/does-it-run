# helium

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/mherrmann/helium, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/helium

## Pinned environment

- Project commit: `624f729746f7a742df1c407accbd0d4a30f49167`
- Test commit: `624f729746f7a742df1c407accbd0d4a30f49167`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 14.7 to 33 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.5 | 33 | 2 | 2 | [run](https://argusic.com/run/cf5bed49-8f5a-43e4-9d08-7e00540f4ead) |
| 2 | pass | 100 | 3 | 14.7 | 3 | 3 | [run](https://argusic.com/run/385a14b7-e9b0-4e6e-87f4-af58121bae92) |

## What was observed on a clean machine

Attempt 1:

- 12 min: `test_write_into_input_type_date: send_keys() on <input type=date> produces empty value in Chrome 154`
- 4 min: `KillServiceAtExitChromeTest fails: InSubProcess uses __module__ which lacks package prefix when discovered by unittest`

Attempt 2:

- 1 min: `Chrome session not created: Chrome instance exited when started via helium.start_chrome in container`
- 1 min: `test_write_into_input_type_date failed: writing '23.08.2024' into <input type=date> with lang=de-DE produced empty value in Chrome 157`
- 1 min: `test_kill_service_at_exit failed: subprocess python -m api.test_kill_service_at_exit_chrome raised ModuleNotFoundError: No module named 'api'`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
