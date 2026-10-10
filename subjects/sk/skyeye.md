# skyeye

**Verdict: could not verify.** Argusic Score 35 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/dromara/skyeye, licensed MIT, written in Java.

Evidence and recordings: https://argusic.com/subject/skyeye

## Pinned environment

- Project commit: `6db63a9bcb13560740b963eadd8821c4a1bbf1bb`
- Test commit: `6db63a9bcb13560740b963eadd8821c4a1bbf1bb`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible
- Valid runs: 2; wall time 24.4 to 26 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 26 | 0 | 0 | [run](https://argusic.com/run/f9909f96-ca2d-48b8-a3b6-32e1595e2736) |
| 2 | fail | 50 | 24 | 24.4 | 3 | 3 | [run](https://argusic.com/run/351c52b8-c557-4f80-bb7d-2240ffc8af31) |

## What was observed on a clean machine

Attempt 2:

- 15 min: `Missing proprietary parent module skyeye-common-rest which provides the framework foundation for all business modules`
- 3 min: `xxl-job-admin failed to start: hardcoded /data/applogs/xxl-job/ path not writable and H2 driver class not bundled`
- 2 min: `skyeye-seata requires Nacos running at localhost:9000 (no mock stood up) and MySQL for DB store mode`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
