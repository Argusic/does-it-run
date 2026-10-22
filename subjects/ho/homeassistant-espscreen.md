# homeassistant_espscreen

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/MaxGramser/homeassistant_espscreen, licensed AGPL-3.0, written in Python.

Evidence and recordings: https://argusic.com/subject/homeassistant-espscreen

## Pinned environment

- Project commit: `19a95b71810117e2878d06998ea9f128fbf3e108`
- Test commit: `19a95b71810117e2878d06998ea9f128fbf3e108`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 84 to 84 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 64 | 84 | 6 | 6 | [run](https://argusic.com/run/bd4b8016-c087-48af-b758-85233f2baeda) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `Python externally-managed-environment prevented pip install`
- 3 min: `C++ test_settings_screen.cpp fails with -Wdangling-reference on g++ 13`
- 2 min: `C++ test_alert_overlay.cpp fails with -Wparentheses on && within ||`
- 5 min: `Editor tests/build fail: crypto.hash not available in Node 18`
- 5 min: `Python server tests fail: /assets/ directory missing`
- `3 editor tests flaky timeout at 5000ms in resource-constrained environment`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
