# FunClip

**Verdict: runs.** Argusic Score 100 of 100 (the mean of the recorded run scores; a timeout is not scored).

Project: https://github.com/modelscope/FunClip, licensed MIT, written in Python.

Evidence and recordings: https://argusic.com/subject/funclip

## Pinned environment

- Project commit: `2a954d4fbad6a57a5271390be4eb43f80d201b60`
- Test commit: `2a954d4fbad6a57a5271390be4eb43f80d201b60`
- Worker image digest: `sha256:cdd920bce7839e4d5ee566bccfa91f8cd7e91a1ae507c6cbe94dffde7808dd1c`
- Worker type: cpu
- Test depth: real run
- Valid runs: 3; wall time 4.2 to 48.6 minutes
- Methodology: version 1.4, https://argusic.com/methodology

## Runs

| Attempt | Status | Score | Install (min) | Wall (min) | Errors observed | Errors resolved | Run page |
|---|---|---|---|---|---|---|---|
| 1 | pass | 100 | 16 | 16.3 | 1 | 1 | [run](https://argusic.com/run/c3ad6ca8-e5fd-440e-905c-0baf9301053d) |
| 1 | pass | 100 | 4 | 4.2 | 1 | 1 | [run](https://argusic.com/run/8bf58dc7-d4f0-4af2-8309-28cfabd64701) |
| 3 | pass | 100 | 8.2 | 48.6 | 4 | 4 | [run](https://argusic.com/run/6cdefaed-16a3-4cb9-94b0-292993b9bf51) |

## What was observed on a clean machine

Attempt 1:

- 3 min: `TypeError in gradio_client.utils._json_schema_to_python_type when additionalProperties is a boolean (pydantic 2.13 / gradio-client 1.3.0 incompatibility)`

Attempt 1:

- 1 min: `litellm not installed but required by 14 tests in test_litellm_api.py`

Attempt 3:

- 0.1 min: `Debian's PEP 668 prevents system-wide pip install; must use a venv`
- 0.5 min: `litellm and pytest missing from requirements.txt but required by tests`
- 0.3 min: `Gradio 4.44.1 has a json_schema_to_python_type crash on / route`
- 0.2 min: `videoclipper.py CLI stage 2 crashes with AttributeError: no 'lang' attribute`

These are observations of what the environment printed, not a statement about the project's quality. Full logs and the terminal recording of each run are on the run pages above.
