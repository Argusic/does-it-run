# hyperresearch

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/jordan-gibbs/hyperresearch, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/hyperresearch

## Pinned environment

- Project commit: `7790041c8705568effea2b018048160c89f848f4`
- Test commit: `7790041c8705568effea2b018048160c89f848f4`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 2; wall time 3.2 to 20.4 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 2.5 | 3.2 | 0 | 0 | [run](https://argusic.com/run/1bb4ee12-4516-443f-ae1a-b8caf8dbc658) |
| 2 | pass with mocks | 92 | 20.6 | 20.4 | 1 | 1 | [run](https://argusic.com/run/47747c5a-2615-4feb-8d5d-f7543cc282e8) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `test_stripping_is_per_instance_not_global and test_opt_out_keeps_crawl4ai_launch_flags failed because crawl4ai 0.9.5 removed --ignore-certificate-errors flags from _build_browser_args and build_browser_flags (they are now conditionally adde`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
