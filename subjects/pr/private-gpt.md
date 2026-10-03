# private-gpt

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/zylon-ai/private-gpt, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/private-gpt

## Pinned environment

- Project commit: `065814007608a95a6160102c370f6ea52ba290d6`
- Test commit: `065814007608a95a6160102c370f6ea52ba290d6`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run, run with mocked services
- Valid runs: 3; wall time 42 to 50.5 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | timeout | none | n/a | 42 | 0 | 0 | [run](https://argusic.com/run/4b5fadde-36c8-4a89-a5d0-0daa0ecd1775) |
| 1 | pass | 100 | 10 | 50.5 | 5 | 5 | [run](https://argusic.com/run/063cc481-8df2-496a-91e0-7c61254d18b7) |
| 2 | timeout | none | 2.5 | 43.9 | 3 | 3 | [run](https://argusic.com/run/4a44ff97-3bf8-4ce9-8b06-98a759712e34) |

## What was observed on a clean machine

Attempt 1:

- 1 min: `Python 3.11 required but 3.12 present in container`
- 5 min: `Missing libmagic system library (python-magic dependency)`
- 2 min: `settings-mock.yaml had no model definitions, server could not register models`
- `Mock profile not loaded from APP_ENV env var - profiles use PGPT_PROFILES`

Attempt 2:

- 3 min: `libmagic C library missing (python-magic requires system libmagic1)`
- 0.5 min: `celery module not found in core dependency group`
- 0.5 min: `pika module not found (RabbitMQ library)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
