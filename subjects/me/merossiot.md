# MerossIot

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/albertogeniola/MerossIot, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/merossiot

## Pinned environment

- Project commit: `4fc819384086b2eae31e11c11871c5aef319654f`
- Test commit: `4fc819384086b2eae31e11c11871c5aef319654f`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 19.3 to 19.3 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 0.25 | 19.3 | 2 | 2 | [run](https://argusic.com/run/bc496ae0-7c39-4a1d-b49d-e2f295a75d16) |

## What was observed on a clean machine

Attempt 1:

- `All 24 test files require real Meross cloud credentials and real Meross IoT hardware , MEROSS_EMAIL, MEROSS_PASSWORD, and devices like smart plugs/bulbs must exist on the account`
- `Tests use AioHTTPTestCase with @unittest_run_loop decorators that are deprecated in aiohttp 3.12+ (63 deprecation warnings)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
