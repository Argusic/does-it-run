# voidaccess

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/KatrielMoses/voidaccess, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/voidaccess

## Pinned environment

- Project commit: `be276d1219a0af9306d5390b6a07bb23f67f7746`
- Test commit: `be276d1219a0af9306d5390b6a07bb23f67f7746`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 23.6 to 23.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 0.4 | 23.6 | 3 | 3 | [run](https://argusic.com/run/5dcb0e40-7b00-4f27-a801-d1a3c1a06553) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `spaCy model en_core_web_sm not installed, causing 8 dependency relationship extraction tests to fail`
- 2 min: `DATABASE_URL unset caused 2 graph API integration tests to crash with RuntimeError in get_session()`
- 1 min: `test_shodan_rate_limit_cap hung for ~50s due to SHODAN_RATE_LIMIT_DELAY=1.0 causing 50 sequential asyncio.sleep(1) calls`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
