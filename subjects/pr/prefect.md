# prefect

**Verdict: runs.** Argusic Score 96 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/PrefectHQ/prefect, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/prefect

## Pinned environment

- Project commit: `148e99781fb05df258d3efddb5ef4fee0b61c9f2`
- Test commit: `148e99781fb05df258d3efddb5ef4fee0b61c9f2`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run, run with mocked services
- Valid runs: 2; wall time 21.8 to 38.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 2 | 21.8 | 0 | 0 | [run](https://argusic.com/run/5b5f455a-7678-4167-8185-cb521751412d) |
| 2 | pass with mocks | 92 | 3 | 38.6 | 3 | 3 | [run](https://argusic.com/run/b1c86312-a31d-462a-b639-960410b3c7e1) |

## What was observed on a clean machine

Attempt 2:

- `Redis connection failure in test_redis.py::test_read_write_path_from_host`
- `Block standards image URL 404 in test_has_a_valid_image[CustomWebhookNotificationBlock]`
- `CLI profile prompt matching in test_populate_defaults_with_existing_profiles`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
