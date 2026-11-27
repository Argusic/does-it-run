# emhass

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/davidusb-geek/emhass, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/emhass

## Pinned environment

- Project commit: `0ebd7e7abb299055dd0f001867462f525889dbd6`
- Test commit: `0ebd7e7abb299055dd0f001867462f525889dbd6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.6 to 25.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4.5 | 25.6 | 3 | 3 | [run](https://argusic.com/run/31ec77fc-6ea9-4182-a8c8-5b0b9373bdc1) |

## What was observed on a clean machine

Attempt 1:

- 15 min: `Open-Meteo timestamp parsing failed with cached JSON containing ISO 8601 strings (not Unix timestamps)`
- 5 min: `Solcast rate limiter persisted between test runs, causing test_get_weather_forecast_solcast_multiroofs_method_mock to fail`
- 5 min: `Two multi-battery optimization pinned regression tests failed due to HiGHS 1.16.0 solver version differences producing different optimal solutions`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
