# phone-harness

**Verdict: runs with mocks.** Argusic Score 92 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/phone-harness/phone-harness, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/run/a63e40e6-9540-4e95-a72b-f44a3f768a5c

## Pinned environment

- Project commit: `ddf2a744666a9629b705d8a91cd4b53010feadfc`
- Test commit: `ddf2a744666a9629b705d8a91cd4b53010feadfc`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: run with mocked services
- Valid runs: 1; wall time 25.7 to 25.7 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass with mocks | 92 | 4 | 25.7 | 3 | 3 | [run](https://argusic.com/run/a63e40e6-9540-4e95-a72b-f44a3f768a5c) |

## What was observed on a clean machine

Attempt 1:

- 2 min: `uv not installed in container; install.md's primary path unavailable`
- 3 min: `project's test mock (FakeControl.PNG in tests/test_cloud.py) served a corrupt PNG: ffmpeg failed with 'inflate returned error -3'`
- 4 min: `control mock lacked documented ops (screen.text, input.text, apps.launch), so helpers screen()/type_text()/open_app() raised Unsupported`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
