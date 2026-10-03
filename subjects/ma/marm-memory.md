# marm-memory

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/Lyellr88/marm-memory, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/marm-memory

## Pinned environment

- Project commit: `0b4013de9e854fccd211d7fdb8e35ff6596ec4a1`
- Test commit: `0b4013de9e854fccd211d7fdb8e35ff6596ec4a1`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 24.5 to 57.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 29.5 | 24.5 | 4 | 4 | [run](https://argusic.com/run/9e169290-f73d-4583-9ad2-41e018cbb86c) |
| 2 | pass | 100 | 10 | 57.3 | 4 | 4 | [run](https://argusic.com/run/be44d449-c5e1-4727-b999-cf1fed8845af) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `pip install failed due to externally-managed-environment (Debian restriction)`
- 0.5 min: `Script scripts/bundle-concept-model.py not found at repo root - only in marm-mcp-server/scripts/`
- 1 min: `concept_model check failed because settings.py looks for bundled model inside the package tree, but pip installed from a different location`
- `17 CBM graph engine errors - codebase-memory-mcp binary singleton conflict (different cache dir)`

Attempt 2:

- 5 min: `test_http_foreground_reaches_health_then_stops , 'stop' without '--force' fails when run from a different subprocess (PID mismatch with foreground runtime)`
- 3 min: `test_status_endpoint_mirrors_the_availability_gates , '/.dockerenv' exists, causing 'in_container()' → True, backend is always ''none''`
- 2 min: `test_websocket_admits_keyless_loopback_without_a_session , Same container detection blocks the WebSocket`
- 5 min: `test_a_queued_write_from_a_foreign_loop_would_hang , Python 3.12 asyncio.Future.set_result uses call_soon (not threadsafe), causing a race; test asserted it must always hang`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
