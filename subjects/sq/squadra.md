# squadra

**Verdict: could not verify.** Argusic Score 20 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dagoSte/squadra, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/squadra

## Pinned environment

- Project commit: `5081a06ae054bc80072d8109ee2ef088b52513c3`
- Test commit: `5081a06ae054bc80072d8109ee2ef088b52513c3`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, no run possible
- Valid runs: 2; wall time 22.5 to 50.2 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | 0 | 50.2 | 7 | 7 | [run](https://argusic.com/run/5b888bce-b92e-40fb-89c4-47a3ea60bafd) |
| 2 | fail | 20 | n/a | 22.5 | 0 | 0 | [run](https://argusic.com/run/c949e4d3-c358-4284-be3a-bcd6a06c37b4) |

## What was observed on a clean machine

Attempt 1:

- `Install requires clean git state (dirty due to test fixes)`
- 5 min: `Container umask 0002 causes group-writable temp dirs, breaking plugin directory permission checks`
- 3 min: `TZ=Europe/Rome required for date-based contract fixtures (chart/locale tests)`
- 1 min: `test_usage_cache.py hardcoded /private/tmp (macOS-only)`
- 3 min: `test_registry_checkpoint.py flaky on fast filesystems where timestamp ns does not change for same-size writes`
- 5 min: `Number formatting with Italian locale (1.000 vs 1000) broke chart contract regexes`
- `memoranda_cases tests need external plugins (not part of core squadra)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
