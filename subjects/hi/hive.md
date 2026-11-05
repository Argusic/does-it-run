# hive

**Verdict: runs.** Argusic Score 93.8 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aden-hive/hive, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/hive

## Pinned environment

- Project commit: `6193aea7eb064f7536dfedcbe9ff08ad954ac53b`
- Test commit: `6193aea7eb064f7536dfedcbe9ff08ad954ac53b`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 2; wall time 20.4 to 21.1 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 90 | 0.3 | 20.4 | 2 | 1 | [run](https://argusic.com/run/3ac0b964-30ea-408d-9fce-b293f12f10d2) |
| 2 | pass | 97.5 | 17 | 21.1 | 8 | 7 | [run](https://argusic.com/run/a5cf63d5-5f27-49f5-8124-88cb51b48998) |

## What was observed on a clean machine

Attempt 1:

- 0.2 min: `Playwright browser binaries missing`
- `test_live_health_checks.py::TestLiveIntegrationWiring::test_wiring_valid[lusha_api_key] , endpoint mismatch between spec and checker URL`

Attempt 2:

- 1 min: `quickstart.sh exited 1 immediately under TERM=dumb because clear returned nonzero and set -e aborted.`
- 2 min: `The installer's dashboard launch crashed with OSError: [Errno 98] address already in use on 127.0.0.1:8787.`
- 5 min: `Playwright was falsely reported as ready because 'playwright install --dry-run' exits 0 without browsers; three chart tests failed with 'Executable doesn't exist'.`
- 2 min: `The core suite had one failure while a live Hive server held the maintenance lock; the janitor test rejected the active runtime.`
- 2 min: `docs/getting-started.md referenced the nonexistent core/examples/manual_agent.py.`
- 1 min: `'uv run python' returned 127 in the current non-login shell because ~/.local/bin was not on PATH.`
- 1 min: `The first browser-render probe timed out waiting for networkidle because the dashboard keeps an SSE stream open.`
- `System sqlite3, tesseract, and Chrome were absent, and quickstart could not install sqlite3 or tesseract via apt without root.`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
