# sprite-gen

**Verdict: runs.** Argusic Score 60 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/aldegad/sprite-gen, licensed Apache-2.0, written in Python.

Evidence and recordings: https://argusic.com/subject/sprite-gen

## Pinned environment

- Project commit: `b725baa5aad026f183e2083275b441f2db225c48`
- Test commit: `b725baa5aad026f183e2083275b441f2db225c48`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: no run possible, real run
- Valid runs: 2; wall time 11.2 to 74.8 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | fail | 20 | n/a | 11.2 | 0 | 0 | [run](https://argusic.com/run/0579f7a0-a57d-4d0f-b00d-f68c35531062) |
| 2 | pass | 100 | 1.2 | 74.8 | 2 | 2 | [run](https://argusic.com/run/ee57806a-fbd4-4963-abc8-a19229124fc9) |

## What was observed on a clean machine

Attempt 2:

- 2 min: `7 video tests failed: img2webp not found on PATH (libwebp CLI tool for WebP output)`
- 1 min: `1 pitch-crosscheck test timed out: pyproject.toml default pytest timeout 120s is too short for this test (~210s needed)`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
