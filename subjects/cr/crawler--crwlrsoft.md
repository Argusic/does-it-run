# crawler

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/crwlrsoft/crawler, licensed MIT, written in PHP.

Evidence and recordings: https://argusic.com/run/fd6ca519-31e7-4f14-8501-059d37300755

## Pinned environment

- Project commit: `11e0f5f00f2a94d4cb1653c6358aa9b92798c039`
- Test commit: `11e0f5f00f2a94d4cb1653c6358aa9b92798c039`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 1; wall time 26.6 to 26.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 25 | 26.6 | 5 | 5 | [run](https://argusic.com/run/fd6ca519-31e7-4f14-8501-059d37300755) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `PHP and Composer not installed in container`
- 5 min: `Chrome binary missing for headless browser tests`
- 4 min: `short_open_tag=On in static PHP build causes <?xml in test server PHP files to be parsed as code`
- 1 min: `Integration test server not ready after 100ms sleep`
- 4 min: `2 headless-browser-proxy integration tests fail - PHP built-in server cannot act as a real HTTP proxy for Chrome`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
